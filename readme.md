## 🧠 bGZo's Second Brain
- Hello there👋.
- My nickname is *bGZo*, actual name is *Feng Hua*, you could call me *hua*, or *hx*
- Wish you have a fun time. That would be my pleasure.
- ## 📢 Logseq Announcements
  - Logseq is just a graph-driven note app[^toc-is-hard-thing], which means linearity support is downside during several alternatives, like [obsidian](https://obsidian.md/).
  - Logseq is not perfect, which means a lot of bugs still existed on different versions[^bug-on-logseq] . So the half life of following rules could be short, I'll try my best to select evergreen tree. [^maintain-soft-rules]
  - ### Classify / Index [^as-non-work-flow]
    - [[work]] that solve blz problem
      collapsed:: true
      - skills
        - tech stack
          - programming language
        - soft skill
          - communication
          - speech
        - language
      - project & side-project
    - non-work **space time** which could spend on
      collapsed:: true
      - [[life]] with self problems (\* required absolutely)
        - like living, health, privacy, sex.
        - especially on **relationship** with your family and lover.
      - [[creation]] that exclude consuming, while doing something real.
      - [[inbox]] that collect, classify, link and **delete** info you token.
        - looking [anime] [comic]
        - playing [game]
        - reading [galgame] [book]
        - listening [music] [podcast]
        - drawing [pixel]
        - improving [productivity] with following devices
          - [[operating-system]]
            - [[windows]]
              - wsa
              - wsl
            - [[linux]]
              - archlinux
                - steamdeck
              - minit
            - [[android]]
              - OneUI SamsungTabS8
            - [[ios]]
              - iPhone
          - browsers
  - ### Store
    - Considered working business info, this part should not open-source, so this deserves with private repository.
    - Then you should take care avoiding [[weekly/1198-wrong-second-brain]] , because your note system should not really be your "repository", which always make your system grow up with high entropy increases, then leading one ending: trash / garbage.
    - So just deal problem with project management way, under certain deadline, that would help you get rid of info overtake, and focus on your business again.
  - ### Soft Rules
    wikipedia:: https://en.wikipedia.org/wiki/Soft_law
    - **Page naming**: use `-` to connect two word rather blank for **readable url**.
      - Don't add the `[[]]` in `page_name`
    - **Properties**: keep order, dictionary is best.
    - **Template**: **Every main page should have a template**, just put them on page properties with collapsed is fine. Then, **all template properties should extend `page`**, and keep adding less properties as much as possible.
    - **Tags**: **`#[[]]` instead of `#`**. They would be popped menu friendly, while editing again.
    - **Namespce**: delay your use of namespaces until you have refined your understanding of how they might suit your workflows. [^namespace-usage]
      - **Use plural of noun while placing something under namespace**, like book, using `books/xxx`instead of `book/xxx`, which could give you a chance to sepreate from each other.
        - I believe when I want to talk book, I would type `book`, then when I want to someone between them, I would type `books`.
      - All name under namespace should use alias to be redirected.
        - the pain of renaming on git is high, which means the history would be lost at all.
        - Secondly, without alternatives now is, the working of alias on logseq, should not appear on graph, because so much more properties, or connect. That would be mess without ability to hide. [^alias-should-more-power]
    - **Page speed performance**:
      - Control the usage of plugin
        - The memory using by logseq is huge after start plugin
        - Debug memory usage on electron is difficult.
      - Control the usage of graph.
        - **NOT ALL IN ONE**. Separate them to different pages.
        - Otherwise the whole graph would be huge
          collapsed:: true
          - ![](https://raw.githack.com/bGZo/assets/dev/2024/20241011235342.png)
          - ![](https://raw.githack.com/bGZo/assets/dev/2024/20241011235415.png)
- ## 🖥 Rebuild
- windows
  ```shell
  rm "$env:appdata\Logseq" -r
  ```
- ## © Copyright
- Copyright 2022 - 2024 [bGZo](https://github.com/bGZo). All rights reserved. The contents is licensed under a [CC-BY-SA](https://creativecommons.org/licenses/by-sa/4.0/); the code is under [MIT](https://github.com/bGZo/blog/blob/main/LICENSE) licence. The contents and comments are copyright their respective authors, submission implies license to publish on this web site.
  ![http://creativecommons.org/licenses/by-sa/4.0/](https://i.creativecommons.org/l/by-sa/4.0/88x31.png) ![https://notbyai.fyi/](https://raw.githack.com/bGZo/assets/dev/2024/Written-By-Human-Not-By-AI-Badge-white.svg)
---
- [^alias-should-more-power]: via: https://discuss.logseq.com/t/enhancement-of-aliases/14466, Towards non-native speakers in English, `alias` is a little bit interesting, more aliases makes graph more complex, which links every node duplicately. This is really funciton need to be enhanced.
- [^toc-is-hard-thing]: via: https://discuss.logseq.com/t/outline-overview-for-sidebar/740/20, I choose use namespace instead of content side bar.
- [^maintain-soft-rules]: Maybe the flow you have to change in next version, or the problem maybe solved, it's really not have too much value.
- [^as-non-work-flow]: If you are a student, or someone else, the work could be something you worked for living. Whether they should separate with space time, there are a thousand Hamlets in a thousand people's eyes. At least in China, space time always conflicts with work, so talking about that is always ambiguous...
- [^bug-on-logseq]: https://discuss.logseq.com/t/pasting-photos-increases-the-size-of-the-image-file-massively/9363
- [^namespace-usage]: https://www.logseqmastery.com/blog/logseq-namespaces, https://discuss.logseq.com/t/outline-overview-for-sidebar/740/19