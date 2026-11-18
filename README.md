我在做 Croon。起初我想知道，搭 Agent 框架时由开发者做的那些决定，有多少可以留到任务开始以后，交给 Agent 自己做？

在 [croon-app](https://github.com/Thooer/croon-app) 里，主 Agent 叫 W0。它可以看到任务以后，写一个合适的帮手，再像调用工具一样调用它。我最感兴趣的是，W0 造这个帮手用的，正是当初造出 W0 自己的那个操作。既然构造 Agent 可以成为 Agent 手里的一件工具，那么安排协作的方式，也不必在写框架时就全部定下来。

顺着这个想法往下做，先要回答的是：W0 写下的程序用什么来运行？这是 [croon-lang0](https://github.com/Thooer/croon-lang0) 的工作。它采用模型熟悉的 Python 写法，但把程序能接触的外部世界限定在明确交给它的工具里。再往下一层，谁有权造一个 Agent，又能把哪些权利交给它，不能由一段刚生成的代码自己说了算。这是 [croon](https://github.com/Thooer/croon) 内核要管的事。

我希望有一天，看到一种值得借鉴的 Agent 框架，能直接在 Croon 上写出它最有意思的那部分，让它跑起来。再往后，我想把这件事也交给一个跑在 Croon 上的 Agent。

对了，除了 Croon，我也对做游戏和写游戏引擎很感兴趣。
