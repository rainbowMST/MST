# 面试题汇总

## 建议（非常不错的建议）

1. 基础。 不管是哪个方向, 基础很重要。就比如iOS, objc的方方面面都必须了解。
2. 全面。 有些东西, 虽然不见得能答好, 但你至少应该懂。
3. 设计模式。 主流的那些设计模式非常有必要了解。
4. 算法。 这个不是说恶补能补好的。建议大家长期积累。另外推荐<剑指offer>这本书。同时, 可以在这里线上答题: 牛客网-剑指offer
5. 简历一定要真实! 基本上面试官都是围绕简历展开交流的。懂或不懂, 一问就知道, 没必要搬起石头砸自己的脚
6. 提前准备。比如自我介绍, 项目介绍, 职业规划等等。基本都是必问的题目，能提前准备就提前准备好。
7. 开源, 分享, 积累。 我一直认为, 分享和开源是程序员进步的不二法门。 我建议每个程序员都应该有自己的Github, 有自己的博客。就这几次面试来说, 博客和Github帮了我多。 网易面试官直言, 他们认真看过我的Github, 微信HR问我要CSDN博客ID, 说她很感兴趣。帮助别人, 也是帮助自己。
8. 沟通。有时候一个问题, 可能不懂, 甚至题目都不理解。不要害怕, 主动与面试官沟通。我在网易面试的时候, 关于全拼算法的实现, 我当时连全拼都没一个完整的概念, 它要满足哪些条件更加不清楚。我跟面试官坦诚我不懂这个概念, 与他们的一步步沟通中实现了自己的算法。 所以沟通, 远比闷头写, 到头来还可能错误来的实在。
9. 自信。 能得到面试机会, 最起码证明, 你很优秀。 我觉得自信很重要。 如果一开始, 就表现的慌慌张张, 畏首畏尾, 那么不管是你自己的发挥, 还是面试官对你的看法, 我觉得都不会很好。

## 面试题

1、经典面试题：

* [招聘一个靠谱的iOS(01-29)](面试题收集/招聘一个靠谱的iOS【30-55】.md)
* [招聘一个靠谱的iOS(30-55)](面试题收集/招聘一个靠谱的iOS【01-29】.md)

2、大公司面试题：

* [招聘_大公司1-算法](面试题收集/招聘_大公司1-算法.md)
* [招聘_大公司2-iOS-汇总](面试题收集/招聘_大公司2-iOS-汇总.md)
* [招聘_大公司2-iOS-综合](面试题收集/招聘_大公司2-iOS-综合.md)
* [招聘_大公司2-iOS-多线程](面试题收集/招聘_大公司2-iOS-多线程.md)

3、面试题汇总

* [面试题10-算法](面试题收集/面试题10-算法.md)
* [面试题21-网络](面试题收集/面试题21-网络.md)
* [面试题31-设计模式](面试题收集/面试题31-设计模式.md)
* [面试题33-基础](面试题收集/面试题33-基础.md)
* [面试题33-进阶](面试题收集/面试题33-进阶.md)
* [面试题34-综合](面试题收集/面试题34-综合.md)
* [面试题35-源码解读](面试题收集/面试题35-源码解读.md)
* [面试题40-Swift](面试题收集/面试题40-Swift.md)

4、智力题

* [智力题1-答案](面试题收集/智力题1-答案.md)

## 其他人面试总结

### 一、头条-面试总结

【哎这里又丢人了有木有。面试的时候千万别立flag！面试官小哥哥可能看我说排序的时候很流利，在出算法题的时候就停顿了一小会，我就说了句，“其实我准备的很仓促，算法题也就简单刷了刷。” 面试官：你刷过算法啊那这个绝对没问题！】然后我就遇到了这个没见过的东西。没（you）写（hua）完（hen）整(lan)。最后在面试官的提示下，根据新思路说了下自己的想法就过了。
可能是因为比较赶时间吧，关于OC的问题不是很多。这时候也出现了网络波动。也就没有做别的代码题了。到了问答环节。

头条总结：头条一直都是视频面，而且是一条龙服务。总体来说感觉不错，反正主要就是需要基础足够扎实，不过之前听说的会手撕算法我倒是运气好没有碰到，就一面写了一道算法题。三面面试官等了一会儿没有来，约到了第二天(毕竟大佬都比较忙)。

--

 一面面试官比较年轻帅气，大概是个24岁的小哥，说话挺温柔的，由于是第一次面试，本来很紧张的，然而气氛不那么严肃，
紧张感就没那么强烈了。上来显示自我介绍（上午临时编了一段。。）

一面可以说是面试的非常好，面试官友好，问的问题我前不久正好研究了下。

1. DNS的话，计算机网络上面讲的比较详细了。我对这个记得比较熟，多级DNS服务器，每一级DNS服务器如何去缓存，缓存刷新时长。详细就看下书上。
2. HTTPDNS，当他问到这个的时候，（笑）到我装逼的时候了。
3. 加快网络连接，对于tcp来说当然是长链接呀，最最基本的。当然上面的HTTPDNS也是一种优化方法，还有就是http2，以及http2支持的长链接的缺点，具体怎么回答的记不清了，不过基本回答的很详细了，包括几种新协议（非标准）的对比，
4. 维持tcp长链接就是客户端每隔一定时间向服务端发送心跳包，表面连接还活着。
5. 怎么发送心跳包。。我不知道。因为没实际写过。
6. 当然是手动布局效率高，因为自动布局其实每一个约束条件相当于一个方程，最后系统来解多元一次方程组从而计算出frame


一面的面试官对我还是非常满意的，问我在项目中使用自动布局还是手动布局，我说我使用自动布局，他就说，他们以前
也是使用自动布局，但是自动布局有很多坑（我没踩到过。。。），同时考虑到效率，他们现在项目都是手动布局。

二面我感觉自己面的非常糟糕，后来整个面试过程非常紧凑，后来听他们说有可能是压力面。
总的来说，每一个问题都有回答一点，然而回答的也不完全。二面结束，也没有有通知我下一次
了，然后面试官好像还很赶时间似的结束了面试。我当时觉得肯定GG了。

三面真的是个惊喜，因为二面结束我都已经放弃了，自我觉得紧张且回答的很烂（后来想想其实也没想象那么烂，压力是扛住了的，只是说网络方面的基础还是不够而已）。吃过饭早早的躺在床上吹逼，突然一个电话，让我打开电脑面试。。
三面面试官大概35岁以上了。态度和蔼，给人感觉是个leader。

三面面试过程主要在谈项目，怎么去解决项目中遇到的问题。
三面面试结束，面试官让我等hr面，托学长问了下，hr说后面和我聊下就没问题了，一周内联系我，但是考虑到我要6月份才能入职，可能提前半个月到一个月才能发offer（也就是5月中以后了）。。。还想着还没开始的春招就提前结束的（后来才知道，我投的不是校招实习生，，是社招实习生，这样，校招还能内推一波吧，再加上网申，感觉还有两次机会的样子）

### 二、美团-面试总结

美团一二面都是很基础的iOS，没面都会有两道手写代码，很简单，比如刷过剑指offer的一点问题。【美团】

总结：美团是视频面，要求手写代码。主要还是问iOS方面的经验吧，算法题很简单也很常见，感觉春招面试算法题基本都是那些常见的，从我这份面试题中也可以看出，很多重复的。那道智力题想清除了也不算难。其它就是一些必备的iOS基础和计网基础吧。

总结：这是我表现得最差的一轮面试吧，美团是我春招面的第一家公司，但是说实话当时准备得还不是很充分，也可以说没有面试经验吧，很多面试官问的问题我都没有get到面试官的点，不过这一面对广度深度都有要求，我面得有点懵逼，以为是一面表现得好二面故意压力面，结果并不是，猝。

### 三、阿里-面试总结

总结：阿里一面算是一次中规中矩的一场面试吧，从介绍项目开始，然后由浅入深，主要考察iOS基础，面试官说我表现得不错，这次面试的时候我还在搜狐实习（捂脸）

总结：阿里的面试效率是真的不提了，二面和一面间隔时间可能相差了一个月吧，我已经从北京回到了学校开始上课了，而且这次面试感觉有点奇怪，最后那道迷之算法题我们也有讨论，实在没搞懂计算两点间的距离的算法还能怎样优化，面试结束后我问了面试官最优解是怎样的，面试官告诉我没有最优，只有更优（微笑脸）

总结：三面面试官主要就聊了一些具体场景问题和一些基础，基础我觉得没太大问题。面试过程中我讲到一些东西发现面试官听不懂，才知道面试官是做安卓的，问一些问题其实有点让我无语，但是总的来说还是回答过来了，感觉也没有太大问题，但是后面还是被挂了，很无奈。

### 三、四-面试总结

好像没多少问题了，记不太清，然后他说完了，我感觉好快，以为要挂了，就强行讲了些runloop和性能优化的东西，然后他说好了，你和下一轮面试官再说吧

总结：k神前一天晚上帮我推的简历，第二天就接到电话了，效率还是比较高。打电话的时候我正在上课，面试官上来就要开始面试，我约到了晚上。这次面试其实表现得也不够好，前两个问题有点没get到面试官想问的点，问得很快。最后面试官突然说他问完了，我很虚，以为自己是挂了，然后给面试官说面试是不是太快了，iOS方面的东西好像都没怎么问。面试官说如果你觉得你还有什么没用展现出来的，你就说说吧，然后我强行讲了一些性能优化方面的东西，因为这是我唯一准备的了解得稍微有点深的东西了。最后还没讲完，面试官直接告诉我让我和下一轮面试官再讲。我不知道如果后面我不强行讲的话，这一面会不会挂，所以很多事情还是需要我们自己努力去争取机会的。

总结：主要还是基础，腾讯是真的喜欢问计网和数据结构。这一轮面试我可以说是裸面了，那几天都在放飞自我，因为那时候已经拿了头条offer，也没有其它想法了，就想着随便面面吧，不过也无所谓。还好面试的时候还能进入状态，虽然面得不是特别好，不过基本上还是能答出来，最后的二叉树遍历，由于平常都想的是递归，一直没怎么注意非递归的实现，我卡了一会儿，还好最后还是想出来了（请不要嘲笑我）。
中间有个小插曲，就是过了几天我在公众号上面查发现我的状态已经挂了，都已经“心灰意冷”了，结果昨天收到一个广东深圳的电话，当时心里就挺激动的，接通后果然是腾讯的HR，意外惊喜。

### 五、百度-面试总结

全是问得iOS方面的问题，问得真的很细，需要基础很扎实，对各个机制真的足够理解，不然确实有点难回答。我只列举一下大概方向，这些东西也是iOS开发必须掌握的基础吧

总结：开始是把我推给的一个偏网络层做C++的部门，所以面试基本都是计算机基础，也讲了一些iOS的东西，但是我猜面试官可能也不是做iOS的。本来打算问我C++，我果断说自己没怎么写过C++，如果问C++我肯定hold不住。

总结：这一面是把我转到做APM的那个组后面的，感觉面试官时间很急，面得有些突兀，不过没有太大的问题，所以基本就让我过了吧。

总结：本来前一面面完都说我技术面已经通过了，我还很诧异，结果发现是搞错了，所以补了这一面，就是考察一下我iOS方面的能力到底是否有水分吧。问得很细，确实需要基础足够扎实才行。

写在最后

以上的面试题肯定是不完整的，只能根据我的印象记录我能想起来的了，而且即时是一个看似简单的题，你如果没有真正弄明白它的原理的话，在面试过程中你也很有可能被问懵，所以一定要打好基础，要知其然并知其所以然。如果你能把上面的问题搞得很清楚的话，我觉得BAT的offer应该都是没有问题的。当然有时候面试还是要看一点运气的，所以我们还需要抓住每一次面试机会。希望面试的同学一切顺利。


## 其他

### 提交 md 注意说明

如果需要换行，行尾必须要有两个空格

### 使用到的命令

批量处理命令：
`ls -1 .../Desktop/MST01/面试题收集 | sed 's/\.app//g' > .../Desktop/NameList.text`

快速添加目录导航：
https://github.com/ekalinin/github-markdown-toc

./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/招聘_大公司1-算法.md > 01.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/招聘_大公司2-iOS-汇总.md > 02.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/招聘_大公司2-iOS-综合.md > 03.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/招聘_大公司2-iOS-多线程.md > 04.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/智力题1-答案.md > 05.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题10-算法.md > 06.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题21-网络.md > 07.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题31-设计模式.md > 08.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题33-基础.md > 09.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题33-进阶.md > 010.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题34-综合.md > 011.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/面试题35-源码解读.md > 012.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/招聘一个靠谱的iOS(01-29).md > 013.text
./gh-md-toc /Users/xxx/Desktop/MST01/面试题收集/招聘一个靠谱的iOS(30-55).md > 014.text


















