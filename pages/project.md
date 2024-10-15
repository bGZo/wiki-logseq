icon:: 📂
also:: 项目
created:: [[20230623]]
description:: any undertaking, carried out individually or collaboratively and possibly involving research or design, that is carefully planned to achieve a particular goal.
template:: project
template-including-parent:: false

  - icon:: 📂
    also:: 
    created:: ``ref(date.now.format('YYYYMMDD'))``
    deadline:: ``ref(date.now.format('YYYYMMDD'))``
    description:: 
    tags:: 
    type:: ``'project'``
  - ## ``'DOING ' + ref(c.page.name)``
    - ### Description
      -
      - #### Input
        -
      - #### Output
        -
      - #### Alternatives
        -
      - #### Notes
        -
  - query-table:: false
    #+BEGIN_QUERY
    {:title [:h3 "Tasks related to ``c.page.name``"]
     :query [:find (pull ?b [*])
         :in $ ?current-page
         :where
         [?p :block/name ?current-page]
         [?b :block/marker ?marker]
    [?p :block/alias ?al]
    (or [?b :block/refs ?p] [?b :block/refs ?al])
    (or
         [(= "NOW" ?marker)]
         [(= "DOING" ?marker)]
         [(= "WAITING" ?marker)]
         [(= "LATER" ?marker)]
    )
    (not [?b :block/page ?p])
    ]
     :inputs [:current-page]
      :result-transform (fn [result]
                          (sort-by (fn [b]
                                     (get b :block/priority "Z")) result))
      :breadcrumb-show? false
      :table-view? false
    }
    #+END_QUERY
  - query-table:: false
    #+BEGIN_QUERY
    {:title [:h3 "Checklist"]
     :query (and (todo todo) (page [[``{ c.page.name }``]]))
      :result-transform (fn [result]
                          (sort-by (fn [b]
                                     (get b :block/priority "Z")) result))
      :breadcrumb-show? false
      :table-view? false
    }
    #+END_QUERY
  - ## ↩ Reference
    -
- ## Project
  query-sort-by:: type
  query-sort-desc:: true
  {{query (or (page-property :type project) (page-property :type "product") (not))}}
- ## Archives
  {{query (or (page-property :type project/done) (page-property :type "product/done"))}}
-