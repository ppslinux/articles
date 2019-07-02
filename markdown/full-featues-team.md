前后端分离团队的资源浪费
===

我最近的项目，团队都是以前端、后端两个分离的形式。作为一个大前端，不论是在 Web 开发的时候，还是开发 Android 应用的时候，经常遇到：

 - 后端 API 产能不免，供给不上的问题
 - 后端 API 出现 BUG，需要等待修复的问题
 - 后端 API 发生了修改，没有通知到前端，showcase 的时候发现了 bug
 - ……

这一系列的问题，让我觉得特别不开心，我浪费了大把地青春在等后端写代码。而联想起很早以前的全功能型团队，我不禁要写一篇文章吐槽一下，WTF，前后端分离团队的资源浪费。

前后端分离团队
---

全功能型开发团队
---

全功能型开发团队是一个**胶水团队**，用一个更好的词就是**精益团队**，团队里的成员可以**独立地处理**大部分的前后端问题。它并非指每个成员都同时擅长前后端，而是在前后端里各有所长。但是，对于业务问题来说，前后端的编码并没有太大的区别。

当一个擅长前端的开发人员，遇到复杂的后端问题，就会找团队里相应的后端开发人员来解决。同理，当一个擅长后端的开发人员，遇到复杂的前端问题，就会找团队里相应的前端开发人员来解决。

我工作的第一个团队是一个全功能型团队，在这个团队里没有前后端之分：**Only Developer**。只是 Developer 分成了：

 - 擅长前端的 Developer 
 - 擅长后端的 Developer 

又或者是：

 - 往前端发展的 Developer
 - 往后端发展的 Developer

在这个 10 个开发人员的团队里，每个开发人员，即是一个前端开发，又是一个后端开发，还有些人充当了临时的 Ops 或者 DevOps 的角色。在一段时间里，我们还尝试着让开发人员拥有测试、业务分析技能，但是我们失败了——Developer is Deverloper，脱离一线就相当的困难。

前后端分离团队的资源浪费
---

与前后端团队相比，一个全功能型团队接触到新的任务时，他接到的是一个开发后端 API、前端 UI 的任务。而不是一个后端 API，又或者仅仅是一个前端 UI 的 story。

### 设计不当导致的浪费

两种不同的团队类型，意味着全功能型团队的成员：

 - 节省了大量的时间在 API 沟通上
 - 可以设计出符合前端 UI 的 API
 - 遇到 Bug 时，可以快速地修复

而在一个前后端分离团队里，他们需要：

 - 花费时候在制定 API 的接口上
 - 设计出的接口，可能并不适合前端使用
 - 遇到 Bug 的时候，修复完后，需要前端或者后端配合

### 进度不一致导致的浪费

可是当前后端进度出现不一致的时候，特别是后端进度落后于前端的时候，会在后期导致大量地返工，并且有大量地开发人员在等待另外一端的实现。

当后端完成开发时，前端去集成代码，遇到一些 Bug，又进一步地需要等待后端去修复这些 Bug。

### 沟通不畅导致的浪费

对于那些前、后端不在同一地方开发的团队来说，他们可能使用 API 文档或者契约来沟通。而在开发的过程中，有一些补充的修改，在即时通信软件上通知了，但是执行的人忘了这回事。那么，就会进一步地导致各式的沟通问题（撕逼）。

总之言之，全功能型开发团队好。

什么阻碍了全功能型开发团队
---

但是要实施全功能型开发团队一点儿也不容易，你要遇到合适的人、合适的项目，还要有适合的领导。

然后，团队就可以关注于技术沟通，和提升技术水平上。

### 技术沟通

在我司我们采用的是开放式办公，任何时候你遇到任何遇到，你都可以轻松 Touch 到团队的每一个人。

对，这种类似于网吧的布局。

那么，剩下的唯一担心的可能就是代码质量了。请注意两个点：

 - 单元测试。即使是不擅长后端，足够的 Test Case，也能提升代码的质量。
 - 适当地结对编程。当一个不擅长后端的成员，刚接触项目时，适合时间的结对编程可以提升他的后端能力。同理于前端能力。
 - Code Review。代码检视，对于不擅长后端的人来说，仍然是一个相当好的成长机会。

在大部分的公司里，基本上很难做到上面三点中的**任意一点**，所以更难实现这种类似的团队。而当我们尝试去建立这样的团队，那么帮助他人成长就是永远的主题。