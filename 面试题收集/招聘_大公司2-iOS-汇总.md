# 大公司面试汇总-iOS

* [iOS：属性](#ios属性)
   * [属性的关键字【百度、阿里、头条】](#属性的关键字百度阿里头条)
   * [property的默认参数【头条】](#property的默认参数头条)
   * [iOS中属性是怎么实现的【阿里】](#ios中属性是怎么实现的阿里)
   * [Category支持添加属性与成员变量吗【阿里】](#category支持添加属性与成员变量吗阿里)
   * [assign可以用于OC对象吗【头条】](#assign可以用于oc对象吗头条)
   * [weak什么时候用【网易】](#weak什么时候用网易)
   * [weak如何实现自动赋nil / weak 为什么能解除循环引用【头条、网易】](#weak如何实现自动赋nil--weak-为什么能解除循环引用头条网易)
   * [unsafe_unretained , weak, assign 区别【网易】](#unsafe_unretained--weak-assign-区别网易)
   * [copy和strong的区别【头条】](#copy和strong的区别头条)
   * [为什么不可变对象要用copy【头条】](#为什么不可变对象要用copy头条)
   * [什么时候深复制，什么时候浅复制【阿里】](#什么时候深复制什么时候浅复制阿里)
* [iOS：KVO/KVC](#ioskvokvc)
   * [了解KVO吗【阿里】](#了解kvo吗阿里)
   * [KVO的实现原理(addObserver的底层实现)【美团、阿里、头条、网易】](#kvo的实现原理addobserver的底层实现美团阿里头条网易)
   * [KVC的底层实现机制【美团、阿里、头条】](#kvc的底层实现机制美团阿里头条)
   * [如果让你设计KVO, 要怎么设计【阿里】](#如果让你设计kvo-要怎么设计阿里)
   * [通知和KVO区别【网易】](#通知和kvo区别网易)
   * [Delegate 的优缺点](#delegate-的优缺点)
   * [Notification 的优缺点](#notification-的优缺点)
   * [KVO 的优缺点](#kvo-的优缺点)
   * [Block 的优缺点](#block-的优缺点)
   * [了解delegate吗?并介绍【阿里】](#了解delegate吗并介绍阿里)
   * [在什么情况使用Notification【阿里】](#在什么情况使用notification阿里)
   * [通知不在 dealloc 中 removeObserver，为什么会崩溃 【网易】](#通知不在-dealloc-中-removeobserver为什么会崩溃-网易)
* [iOS：内存](#ios内存)
   * [OC中对象的结构【腾讯】](#oc中对象的结构腾讯)
   * [内存结构，包括类和整个App的。App的生命周期【网易】](#内存结构包括类和整个app的app的生命周期网易)
   * [了解iOS内存管理吗【网易、百度、阿里、头条】](#了解ios内存管理吗网易百度阿里头条)
   * [ARC和MRC。iOS内存管理跟GC的区别。【美团】](#arc和mrcios内存管理跟gc的区别美团)
   * [一个iOS app，在内存中除了会使用到堆区和栈区，还会使用到什么区【头条】](#一个ios-app在内存中除了会使用到堆区和栈区还会使用到什么区头条)
   * [内存中堆与栈的区别【头条】](#内存中堆与栈的区别头条)
   * [什么时候在栈中什么时候在堆中【头条】](#什么时候在栈中什么时候在堆中头条)
   * [只用栈实现一个队列【头条】](#只用栈实现一个队列头条)
   * [如何检测应用是否卡顿【腾讯】](#如何检测应用是否卡顿腾讯)
   * [为什么OC不能像下面这样实例一个对象：1. class A;2. A a;【头条】](#为什么oc不能像下面这样实例一个对象1-class-a2-a-a头条)
   * [各种布局方式。只用frame，在横屏或者有电话时界面改变如何重设布局。【网易】](#各种布局方式只用frame在横屏或者有电话时界面改变如何重设布局网易)
   * [AutoReleasepool 的 倾倒方法 和 release 方法的区别 【网易】](#autoreleasepool-的-倾倒方法-和-release-方法的区别-网易)
   * [Autorelease pool的实现原理【阿里】](#autorelease-pool的实现原理阿里)
   * [release 和 autorelease 区别【网易】](#release-和-autorelease-区别网易)
   * [autorelease 和 @autorelease区别【网易】](#autorelease-和-autorelease区别网易)
   * [release 和 drain 的区别](#release-和-drain-的区别)
   * [ARC是什么？objc是如何记录引用计数的。GC机制有无了解。 【京东】](#arc是什么objc是如何记录引用计数的gc机制有无了解京东)
* [iOS：Block](#iosblock)
   * [三种Block【阿里】](#三种block阿里)
   * [Block和delegate的比较【阿里】](#block和delegate的比较阿里)
   * [Block和通知的区别，分别适用什么场景【腾讯】](#block和通知的区别分别适用什么场景腾讯)
   * [了解循环引用吗【网易】](#了解循环引用吗网易)
   * [Block的循环引用、如何解决、原理【阿里】](#block的循环引用如何解决原理阿里)
   * [block修改外部变量值，block是否会循环引用，怎么解决【阿里】](#block修改外部变量值block是否会循环引用怎么解决阿里)
   * [__block什么时候用【网易】](#__block什么时候用网易)
   * [在block里面, 对数组执行添加操作, 这个数组需要声明成 __block 吗【网易】](#在block里面-对数组执行添加操作-这个数组需要声明成-__block-吗网易)
   * [在block里面, 对NSInteger进行修改, 这个NSInteger是否需要声明成__blcok【网易】](#在block里面-对nsinteger进行修改-这个nsinteger是否需要声明成__blcok网易)
* [iOS：Runloop/Runtime](#iosrunloopruntime)
   * [Runloop【网易】](#runloop网易)
   * [了解runtime吗【网易】](#了解runtime吗网易)
   * [Runtime什么时候用【网易】](#runtime什么时候用网易)
   * [消息发送和转发机制(消息调用的过程)，SEL和IMP。【美团、网易、阿里】](#消息发送和转发机制消息调用的过程sel和imp美团网易阿里)
   * [介绍一下Runtime怎么工作的？还能做些什么？【头条】](#介绍一下runtime怎么工作的还能做些什么头条)
   * [谈谈你对Objective-C的动态绑定理解？【京东】](#谈谈你对objective-c的动态绑定理解京东)
   * [如果想要删除自己的一段代码，如何删除（在程序执行的过程中删除）【美团】](#如果想要删除自己的一段代码如何删除在程序执行的过程中删除美团)
* [iOS：其他](#ios其他)
   * [多态【腾讯】](#多态腾讯)
   * [有序和无序set实现原理区别【网易】](#有序和无序set实现原理区别网易)
   * [NSArray、NSSet、NSDictionary的效率【头条】](#nsarraynssetnsdictionary的效率头条)
   * [存一个通讯录，包括增删改查，用什么数据结构【腾讯】](#存一个通讯录包括增删改查用什么数据结构腾讯)
   * [事务的特征【阿里】](#事务的特征阿里)
   * [持久化，iOS中数据持久化的几种方式【阿里】](#持久化ios中数据持久化的几种方式阿里)
   * [做过数据库没，Core Data【网易】](#做过数据库没core-data网易)
   * [你项目中的数据具体缓存怎么做的。【阿里】](#你项目中的数据具体缓存怎么做的阿里)
   * [layoutIfNeeded和setNeedsLayout的区别【头条】](#layoutifneeded和setneedslayout的区别头条)
   * [如何让一个label靠左，一个label靠右，然后右边的label能够完全显示【美团】](#如何让一个label靠左一个label靠右然后右边的label能够完全显示美团)
   * [使用自动布局，把三个view横向等宽等间距（与父view边距也相等）排列。【头条】](#使用自动布局把三个view横向等宽等间距与父view边距也相等排列头条)
   * [自动布局（设置约束）和手动布局（设置frame）的优缺点，哪个效率高，为什么？【头条】](#自动布局设置约束和手动布局设置frame的优缺点哪个效率高为什么头条)
   * [中途还讨论了Masonry的约束应该写在哪里，我说应该写在layoutSubViews，他说会调用多次，然后争论了一会儿【阿里】](#中途还讨论了masonry的约束应该写在哪里我说应该写在layoutsubviews他说会调用多次然后争论了一会儿阿里)
   * [如何扩大view的响应范围【美团】](#如何扩大view的响应范围美团)
   * [浅拷贝和深拷贝的区别【阿里】](#浅拷贝和深拷贝的区别阿里)
   * [数组的浅拷贝与深拷贝【头条】](#数组的浅拷贝与深拷贝头条)
   * [数组copy后里面的元素会复制一份新的吗【头条】](#数组copy后里面的元素会复制一份新的吗头条)
   * [上线APP的crash收集。【网易】](#上线app的crash收集网易)
   * [iOS7之后, 蓝牙的围栏功能【阿里】](#ios7之后-蓝牙的围栏功能阿里)
   * [UIView做动画方法的底层实现 【网易】](#uiview做动画方法的底层实现-网易)
   * [Tableview上拉下拉刷新的原理【美团】](#tableview上拉下拉刷新的原理美团)
   * [断点的实现方式，app是如何停止在断点的【网易】](#断点的实现方式app是如何停止在断点的网易)
   * [动画掉帧，CADisPlayLink，Core graphics 【网易】](#动画掉帧cadisplaylinkcore-graphics-网易)
   * [如何通过一个view查找它所在的ViewController【美团】](#如何通过一个view查找它所在的viewcontroller美团)
   * [AFN，URLSession，相互关系。【网易】](#afnurlsession相互关系网易)
   * [Pod update和pod install的区别【头条】](#pod-update和pod-install的区别头条)
   * [静态库和动态库区别【网易】](#静态库和动态库区别网易)
   * [Ipa 文件内容【网易】](#ipa-文件内容网易)
   * [App签名【网易】](#app签名网易)
   * [程序执行的过程【美团】](#程序执行的过程美团)
   * [iOS里面的事件响应链【头条、美团】](#ios里面的事件响应链头条美团)
   * [id ,NSObject, id区别【网易】](#id-nsobject-id区别网易)
   * [NSObject 和 《NSObject》的区别，为什么要有后者 【网易】](#nsobject-和-nsobject的区别为什么要有后者-网易)
   * [delegate转block怎么处理，比如把 NSURLConnection 的delegate转成block。【美团】](#delegate转block怎么处理比如把-nsurlconnection-的delegate转成block美团)
   * [OC允许多继承吗，要用什么方式实现多继承【阿里】](#oc允许多继承吗要用什么方式实现多继承阿里)
   * [异步下载如何实现【阿里】](#异步下载如何实现阿里)
   * [说说Cell重用原理，Cell重用机制具体怎么实现【阿里】](#说说cell重用原理cell重用机制具体怎么实现阿里)
   * [不用框架，谈谈你如何处理图片缓存以及优化【阿里】](#不用框架谈谈你如何处理图片缓存以及优化阿里)
   * [异步网络图片加载的设计思路。【京东】](#异步网络图片加载的设计思路京东)
   * [异步网络接口的缓存机制。【京东】](#异步网络接口的缓存机制京东)
   * [谈谈面向对象的含义【京东】](#谈谈面向对象的含义京东)


## iOS：属性

### 属性的关键字【百度、阿里、头条】

1. **原子性**---------nonatomic 特质
2. **读/写权限**------readwrite(读写)、readonly (只读)
3. **内存管理语义**---assign、strong、 weak、unsafe_unretained、copy
4. **方法名**--------getter= 、setter=

### property的默认参数【头条】

1. **基本数据类型**：atomic、readwrite、assign
2. **Objective-C 对象**：atomic、readwrite、strong

### iOS中属性是怎么实现的【阿里】

@property = ivar + getter + setter;
“属性” (property)有两大概念：ivar（实例变量）、存取方法（access method ＝ getter + setter）。
“属性” (property)作为 Objective-C 的一项特性，主要的作用就在于封装对象中的数据。 Objective-C 对象通常会把其所需要的数据保存为各种实例变量。实例变量一般通过“存取方法”(access method)来访问。

### Category支持添加属性与成员变量吗【阿里】

一般不支持添加属性，但是可以通过运行时特性来关联属性

category 使用 @property 也是只会生成 setter 和 getter 方法的声明
如果我们真的需要给 category 增加属性的实现，需要借助于运行时的两个函数：
1. objc_setAssociatedObject
2. objc_getAssociatedObject

### assign可以用于OC对象吗【头条】

assign：简单赋值，不更改索引计数（Reference Counting）对基础数据类
assign生成的成员变量是用__unsafe_unretained 修饰的 Cat * __unsafe_unretained _cat;
__unsafe_unretained : 所指向的对象销毁后，仍旧指向已经销毁的对象
__weak : 所指向的对象销毁后，会自动变成nil指针（空指针），不再指向已经销毁的对象

**assign其实也可以用来修饰对象。**
那么我们为什么不用它修饰对象呢？因为被assign修饰的对象（一般编译的时候会产生警告：Assigning retained object to unsafe property; object will be released after assignment）在释放之后，指针的地址还是存在的，也就是说指针并没有被置为nil，造成野指针。对象一般分配在堆上的某块内存，如果在后续的内存分配中，刚好分到了这块地址，程序就会崩溃掉。

那为什么可以用assign修饰基本数据类型？
因为基础数据类型一般分配在栈上，栈的内存会由系统自己自动处理，不会造成野指针。

assign的内存管理语义，MRC用的时候会有循环引用吗 【网易】

**assign：**设置方法只会执行对“纯量类型”的简单赋值操作
不会造成循环引用，但是可能造成野指针

### weak什么时候用【网易】

1. 在 ARC 中,在有可能出现循环引用的时候，往往要通过让其中一端使用 weak 来解决,
    比如：delegate 代理属性
2. 自身已经对它进行一次强引用,没有必要再强引用一次,此时也会使用 weak,
    自定义 IBOutlet 控件属性一般也使用 weak；当然，也可以使用strong。

### weak如何实现自动赋nil / weak 为什么能解除循环引用【头条、网易】

runtime 对注册的类， 会进行布局，对于 weak 对象会放入一个 hash 表中。 用 weak 指向的对象内存地址作为 key，当此对象的引用计数为0的时候会 dealloc，假如 weak 指向的对象内存地址是a，那么就会以a为键， 在这个 weak 表中搜索，找到所有以a为键的 weak 对象，从而设置为 nil。

### unsafe_unretained , weak, assign 区别【网易】

* **weak** 声明了一个可以自动 nil 化的弱引用。
* **unsafe_unretained** 声明一个弱应用，但是不会自动nil化，也就是说，如果所指向的内存区域被释放了，这个指针就是一个野指针了。
* **assign** 的“设置方法”只会执行针对“纯量类型”，用于非 OC 对象

### copy和strong的区别【头条】

**strong**此特质标明该属性定义了一种拥有关系。为这种属性设定新值时，设置方法会先保留新值再释放旧值，然后再讲新值设置上去。
**copy**此特质所表达的所属关系与strong类似。然而设置方法并不保留新值而是将其拷贝

### 为什么不可变对象要用copy【头条】

用@property声明 NSString、NSArray、NSDictionary 经常使用copy关键字，是因为他们有对应的可变类型：NSMutableString、NSMutableArray、NSMutableDictionary，**他们之间可能进行赋值操作**，为确保对象中的字符串值不会无意间变动，应该在设置新属性值时拷贝一份。

### 什么时候深复制，什么时候浅复制【阿里】

* 把一个对象赋值给一个属性变量，当这个对象变化了，如果希望属性变量变化就使用strong属性，如果希望属性变量不跟着变化，就是用copy属性。
* 如果一般情况下，我们都不希望字串的值跟着NSMutableString变化，所以我们一般用copy来设置string的属性。

## iOS：KVO/KVC

### 了解KVO吗【阿里】

键值观察者模式，用来监听对象属性的变化，可以用来实现一些同步操作

### KVO的实现原理(addObserver的底层实现)【美团、阿里、头条、网易】

生成一个派生类，实际的操作都是针对派生类，只是对用户不可见
setter 两个方法：willChangeValueForKey didChangevlueForKey

* KVO是基于runtime机制实现的
* 当某个类的属性对象第一次被观察时，系统就会在运行期动态地创建该类的一个派生类，在这个派生类中重写基类中任何被观察属性的 setter 方法。派生类在被重写的setter方法内实现真正的通知机制
* 如果原类为 Person，那么生成的派生类名为 NSKVONotifying_Person
* 每个类对象中都有一个 isa 指针指向当前类，当一个类对象的第一次被观察，那么系统会偷偷将 isa 指针指向动态生成的派生类，从而在给被监控属性赋值时执行的是派生类的 setter 方法
* 键值观察通知依赖于 NSObject 的两个方法: `willChangeValueForKey:` 和 `didChangevlueForKey:`；在一个被观察属性发生改变之前， willChangeValueForKey:一定会被调用，这就 会记录旧的值。而当改变发生后，didChangeValueForKey:会被调用，继而 observeValueForKey:ofObject:change:context: 也会被调用。
* 补充：KVO 的这套实现机制中苹果还偷偷重写了 class 方法，让我们误认为还是使用的当前类，从而达到隐藏生成的派生类

[探究KVO的底层实现原理](https://www.jianshu.com/p/829864680648)

### KVC的底层实现机制【美团、阿里、头条】

简单描述：

**1、设置值：**

* 第一步：value key 非空判断
* 第二步：通过 key 来拼接 set 方法，看对象是否实现，如果实现，直接调用 set 方法赋值
* 第三步：如果没有找到 set 方法，那就需要通过运行时方法获取实例变量列表，然后来和 key 进行匹配：
    * 先匹配 下划线 _ 和 key 拼接的实例变量
    * 再匹配 没有下划线 key 的实例变量
    * 如果匹配到就赋值
* 如果没有匹配到，就是那就提示用户，对象没有这个实例变量，无法赋值

**2、取值：**

* 第一步：value key 非空判断
* 第二步：通过 key 来拼接 get 方法，看对象是否实现，如果实现，直接调用 set 方法赋值
* 第三步：如果没有找到 get 方法，那就需要通过运行时方法获取实例变量列表，然后来和 key 进行匹配：
    * 先匹配 下划线 _ 和 key 拼接的实例变量
    * 再匹配 没有下划线 key 的实例变量
    * 如果匹配到就取值，并返回
* 如果没有匹配到，就是那就提示用户，对象没有这个实例变量，无法取值

### 如果让你设计KVO, 要怎么设计【阿里】

底层可能是一个单例，通过键值对的形式来保存添加通知的对象，以及需要执行的方法，传递的参数

### 通知和KVO区别【网易】

**通知：**更多地用在跨域传值，没有多少关联的情况下使用

但是KVO只能检测类中的属性，并且属性名都是通过NSString来查找，编译器不会帮你检错和补全，纯手敲所以比较容易出

[KVO、Notification、delegate、block 各自的优缺点，效率还有使用场景](https://blog.csdn.net/JGL357/article/details/79085192)

### Delegate 的优缺点

优点：

1. 非常严格的语法，减少维护成本，较强的代码可读性，所有能响应的事件必须在协议中有清晰的定义
2. 编译器能帮你检查是否实现了所有应该实现的方法，不容易遗忘和出错，如果delegate中的一个方法没有实现那么就会出现编译警告/错误
3. 使用delegate的时候，逻辑很清楚，控制流程可跟踪和识别
4. 在一个controller中可以定义多个协议，每个协议有不同的delegate，满足自定义开发需求，可选必选有较大的灵活性。
5. 没有第三方要求保持/监视通信过程，一旦出现问题，那我们可以比较方便的定位错误代码。
6. 能够接受调用的协议方法的返回值，意味着delegate能够提供反馈信息给controller
7. 减少代码的耦合性，使事件监听和事件处理相分离。 

缺点:

1. 需要定义很多代码：1.协议定义；2.controller的delegate属性；3.在delegate本身中实现delegate方法定义，实现委托的代码过程比较繁琐。
2. 在释放代理对象时，需要小心的将delegate改为nil。一旦设定失败，那么调用释放对象的方法将会出现内存crash
3. 在一个controller中有多个delegate对象，并且delegate是遵守同一个协议，但还是很难告诉多个对象同一个事件，不过有可能，委托的易用性将大大降低。
4. 当实现跨层传值监听的时候将加大代码的耦合性，并且程序的层次结构将变的混乱。
5. 要注意防止强循环引用

### Notification 的优缺点

**他是一个单例对象，允许当事件发生的时候通知一些对象，满足控制器与一个任意的对象进行通信的目的**

优点：

1. 代码量少，实现比较简单
2. 一个对象发出的通知，多个对象能进行反应，一对多的方式实现很简单
3. 传值方便快捷，Context自身携带相应的内容。

缺点：

1. 编译期不会接茬通知是否能被正确处理
2. 释放注册的对象时候，需要在通知中心取消注册，否则将出现不可预见的crash
3. 调试的时候，程序的工作以及控制流程难跟踪
4. controller和观察者需要提前知道通知名称、UserInfo dictionary keys。如果这些没有在工作区间定义，那么会出现不同步的情况
5. 当使用者向通知中心发送通知的时候，并不能获得任何反馈信息。
6. 需要一个第三方的对象来做监听者与被监听者的中介，管理controller和观察者的联系

### KVO 的优缺点

**KVO有显著的使用场景，当你希望监视一个属性的时候，我们选用KVO**

优点：

1. 能够提供一种简单的方法实现两个对象间的同步。例如：model和view之间同步；
2. 能够对非我们创建的对象，即内部对象的状态改变作出响应，而且不需要改变内部对象（SDK对象）的实现；
3. 能够提供观察的属性的最新值以及先前值；
4. 用key paths来观察属性，因此也可以观察嵌套对象；
5. 完成了对观察对象的抽象，因为不需要额外的代码来允许观察值能够被观察

缺点：

1. 我们观察的属性必须使用strings来定义。因此在编译器不会出现警告以及检查；
2. 对属性重构将导致我们的观察代码不再可用；
3. 复杂的“IF”语句要求对象正在观察多个值。这是因为所有的观察代码通过一个方法来指向；
4. 当释放观察者时不需要移除观察者。

### Block 的优缺点

优点：

1. block也就是代码块，在很多调用中使用block都会使得代码的逻辑更加清晰。
2. block可以不进行命名，或者存储在临时变量之中；所以在只需要调用一次，或者在同一函数内多次调用的地方，使用block会比较方便。
3. 当然，block也可以存储在属性之中，进行多次调用；这么使用的时候，一定要注意判断block不为nil。
4. 语法简洁，实现回调不需要显示的调用方法，代码更为紧凑。
5. 增强代码的可读性和可维护性。
6. 配合GCD优秀的解决多线程问题。

缺点:

1. Block中得代码将自动进行一次retain操作，容易造成内存泄露。 
2. Block内默认引用为强引用，容易造成循环引用。


### 了解delegate吗?并介绍【阿里】


### 在什么情况使用Notification【阿里】


### 通知不在 dealloc 中 removeObserver，为什么会崩溃 【网易】

通知中心对响应者observer是使用unsafe_unretained修饰，当响应者释放会出现野指针，如果向野指针发送消息造成崩溃

对象可能已经被销毁了，就会访问野指针，然后崩溃

## iOS：内存

### OC中对象的结构【腾讯】

**objc_object** 是一个包含 isa 指针的结构体
![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121111847.png)

**NSObject** 就是一个包含 isa 指针的结构体
![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121111814.png)

**Class** 也是一个包含 isa 指针的结构体
![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121111758.png)

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121112037.jpg)

[Objective-C对象模型及应用](https://blog.devtang.com/2013/10/15/objective-c-object-model/)

### 内存结构，包括类和整个App的。App的生命周期【网易】

### 了解iOS内存管理吗【网易、百度、阿里、头条】

iOS：ARC和MRC，自动引用计数和手动引用计数
Mac OS：GC 

（我简单说了下MRC ARC，栈堆的区别和怎么回收）

### ARC和MRC。iOS内存管理跟GC的区别。【美团】

在java中有个垃圾回收器，什么是垃圾回收器？
就是在程序运行的期间，垃圾回收器会不断的去扫描堆中的对象是否无人使用。如果无人使用就会回收了。

ARC在编译的时候就会在合适的地方插入retain, release,autorelease,在运行的时候没有东西去进行实时检查，它插入的代码可以在对象没有人用的时候，引用计数器就会变为0.一旦变为0就会被销毁了。

如果在java中有一段代码是Person * p=[Person new]; p=nil，这个对象什么时候被回收？不一定，因为这要看垃圾回收器有没有扫描到这里。

### 一个iOS app，在内存中除了会使用到堆区和栈区，还会使用到什么区【头条】

* 1、栈区（stack）由编译器自动分配释放   ，存放函数的参数值，局部变量的值等。其操作方式类似于数据结构中的栈。  
* 2、堆区（heap）一般由程序员分配释放，   若程序员不释放，程序结束时可能由OS回收，注意它与数据结构中的堆是两回事，分配方式倒是类似于链表，呵呵。  
* 3、全局区（静态区）（static）—，全局变量和静态变量的存储是放在一块的，初始化的全局变量和静态变量在一块区域，   未初始化的全局变量和未初始化的静态变量在相邻的另一块区域，程序结束后由系统释放。  
* 4、文字常量区   —常量字符串就是放在这里的。   程序结束后由系统释放  
* 5、程序代码区—存放函数体的二进制代码。  

### 内存中堆与栈的区别【头条】

1. 申请方式：
    * 栈：由系统自动分配。例如，声明在函数中一个局部变量 int b; 系统自动在栈中为b开辟空间
    * 堆：需要程序员自己申请，并指明大小，在C中 malloc 函数，如p1 = (char *)malloc(10)；在C++中用new运算符，如p2 = (char *)malloc(10)。但注意p1、p2本身是在栈中的
2. 申请后系统的响应：
    * 栈：只要栈的剩余空间大于所申请空间，系统将为程序提供内存，否则将报异常提示栈溢出。
    * 堆：首先应该知道操作系统有一个记录空闲内存地址的链表，当系统收到程序的申请时，会遍历该链表，寻找第一个空间大于所申请空间的堆结点，然后将该结点从空闲结点链表中删除，并将该结点的空间分配给程序，另外，对于大多数系统，会在这块内存空间中的首地址处记录本次分配的大小，这样，代码中的delete语句才能正确的释放本内存空间。另外，由于找到的堆结点的大小不一定正好等于申请的大小，系统会自动的将多余的那部分重新放入空闲链表中。
3. 申请大小的限制：
    * 栈：在Windows下,栈是向低地址扩展的数据结构，是一块连续的内存的区域。这句话的意思是栈顶的地址和栈的最大容量是系统预先规定好的，
    * 堆： 堆是向高地址扩展的数据结构，是不连续的内存区域。
4. 申请效率的比较：
    * 栈：栈由系统自动分配，速度较快。但程序员是无法控制的。
    * 堆：堆是由new分配的内存，一般速度比较慢，而且容易产生内存碎片，不过用起来最方便.
5. 堆和栈中的存储内容：
    * 栈：在函数调用时，第一个进栈的是主函数中后的下一条指令（函数调用语句的下一条可执行语句）的地址，然后是函数的各个参数，在大多数的C编译器中，参数是由右往左入栈的，然后是函数中的局部变量。
    * 堆：一般是在堆的头部用一个字节存放堆的大小。堆中的具体内容有程序员安排。

程序的内存大概分为下面几个部分：

* 1、栈区（stack）由编译器自动分配释放   ，存放函数的参数值，局部变量的值等。其操作方式类似于数据结构中的栈。  
* 2、堆区（heap）一般由程序员分配释放，   若程序员不释放，程序结束时可能由OS回收，注意它与数据结构中的堆是两回事，分配方式倒是类似于链表，呵呵。  
* 3、全局区（静态区）（static）—，全局变量和静态变量的存储是放在一块的，初始化的全局变量和静态变量在一块区域，   未初始化的全局变量和未初始化的静态变量在相邻的另一块区域，程序结束后由系统释放。  
* 4、文字常量区   —常量字符串就是放在这里的。   程序结束后由系统释放  
* 5、程序代码区—存放函数体的二进制代码。  

[内存中堆（heap）与栈（stack）的区别](https://blog.csdn.net/ironyoung/article/details/41682167)
[内存中的堆和栈到底是什么](https://www.jianshu.com/p/52b5a1879aa1)

### 什么时候在栈中什么时候在堆中【头条】

* 栈：    
    * 1、临时变量名
    * 2、字符串
    * 3、对象的变量名，保存在栈中
* 堆：
    * 1、对象的值保存在堆中
* 123456\\\\0在常量区，number在栈上：NSString *number = @"123456";
* Swift 中引用类型存储在 “堆” 上，值类型存储在 “栈” 

### 只用栈实现一个队列【头条】
栈：  先进后出
队列：先进先出

栈1作为存储空间，以栈2作为临时缓冲区。 
入队时，将元素压入栈1。 
出队时，将栈1的元素逐个“倒入”（弹出并压入）栈2，将栈2的顶元素弹出作为出队元素，之后再将栈2剩下的元素逐个“倒回”栈1。

优化： 
在出队时，将s1的元素逐个“倒入”s2时，原在s1栈底的元素，不用“倒入”s2（即只“倒”s1.Count()-1个），可直接弹出作为出队元素返回。这样可以减少一次压栈的操作。

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121133807.jpg)

[使用两个栈(stack)实现一个队列（queue）](https://blog.csdn.net/Nathan1987_/article/details/78729882)

### 如何检测应用是否卡顿【腾讯】

[质量监控-卡顿检测](http://sindrilin.com/2017/03/24/blocking_observe.html)

* JPFPSStatus：监测当前操作的fps
* PerformanceMonitor：
    * 先注册观察RunLoop，并添加到 Common 模式下，在子线程监控时长 开启一个持续的loop用来进行监控
    * 假定连续5次超时50ms认为卡顿(当然也包含了单次超时250ms)
    * 两个runloop的状态，BeforeSources和AfterWaiting这两个状态区间时间能够检测到是否卡顿
    * 还可以上传服务器，方便线上监测

### 为什么OC不能像下面这样实例一个对象：1. class A;2. A a;【头条】

### 各种布局方式。只用frame，在横屏或者有电话时界面改变如何重设布局。【网易】

最初的手动布局
自动布局
XIB、StoryBoard

可以判断用户手机的状态，然后进行重新布局

### AutoReleasepool 的 倾倒方法 和 release 方法的区别 【网易】

自动释放池内的对象，在出释放池的时候会被自动释放掉
release 是 MRC 管理手动管理内存的时候，主动去让引用计数减一的

### Autorelease pool的实现原理【阿里】

autorelease 本质上就是延迟调用 release ，那 autoreleased 对象究竟会在什么时候释放呢？

autoreleasepool 以一个队列数组的形式实现,主要通过下列三个函数完成.

```
objc_autoreleasepoolPush
objc_autoreleasepoolPop
objc_autorelease
```
看函数名就可以知道，对 autorelease 分别执行 push，和 pop 操作。销毁对象时执行release操作。

[Objective-C Autorelease Pool 的实现原理](http://blog.leichunfeng.com/blog/2015/05/31/objective-c-autorelease-pool-implementation-principle/)

### release 和 autorelease 区别【网易】

只是引用计数减一的时机不同而已，autorelease会在对象的使用真正结束的时候才做引用计数减一

**release** 会立即引用计数减一
**autorelease** 延迟释放，会先把对象标记起来可以 release，然后在一个运行循环结束再来进行 release 操作

### autorelease 和 @autorelease区别【网易】

我们的程序在main()调用的时候会自动调用一个autorelease，然后在每一个 Runloop， 系统会隐式创建一个Autorelease pool，这样所有的release  pool会构成一个象CallStack一样的一个栈式结构，在每一个Runloop结束时，当前栈顶的 Autorelease  pool（main()里的autorelease）会被销毁，这样这个pool里的每个Object会被release。

可以把autorelease  pool理解成一个类似父类与子类的关系，main()创建了父类，每个Runloop自动生成的或者开发者自定义的autorelease  pool都会成为该父类的子类。当父类被释放的时候，没有被释放的子类也会被释放，这样所有子类中的对象也会收到release消息。

那什么是一个Runloop呢？ 一个UI事件，Timer call， delegate call， 一个鼠标事件,键盘按下(MAC OSX),或者iphone上的触摸事件，异步http连接下后当接收完数据时，都会是一个新的Runloop。

作者：点滴滴
链接：https://www.jianshu.com/p/a2464d51f34b
來源：简书
简书著作权归作者所有，任何形式的转载都请联系作者获得授权并注明出处。

### release 和 drain 的区别

* 在引用计数环境下，使用[pool release]或[pool drain]效果是相同的
* **但是**drain仅适用于max os高版本，低版本不适用，
* 而release通用，其它并无太大差别。

### ARC是什么？objc是如何记录引用计数的。GC机制有无了解。 【京东】
只要从 isa 的ex_retain 位记录 引用计数加1，并且当引用计数不够时会使用sidetable进行额外记录即可。GC我猜想是考知识面，因为macOS在之前开发中都是使用垃圾回收，而现在苹果放弃了GC在所有开发上的运用，都换做ARC内存管理方式。 
（面试官赞赏底层看的比较细，转问算法。由于我有acm经历，可能问题较难）第一题是给定Tag，在一个View中查询所有Tag为给定的View。

## iOS：Block

### 三种Block【阿里】

首先引用《Objective-C高级编程》Blocks章节中的第一句话：**Blocks是对C语言的扩充功能**。

* 而且OC是建立在C语言基础上之上，添加了面向对象机制的一门编程语言。
* 所以不要再说block的实现原理是C++的函数指针了，正确答案是：block的实现原理是C语言的函数指针。 
* **函数指针**即函数在内存中的地址，通过这个地址可以达到调用函数的目的。
* Block是NSObject的子类，拥有NSObject的所有属性，所以block对象也有自己的生命周期，生存期间也会被持有和释放。

Block有三种：

1. NSGlobalBlock 静态区（全局区）block，这是一种特殊的bloclk，因为不引用外部变量而存在。另外，作为静态区的对象，它的释放是有操作系统控制的，这一点我们最后再聊。 
    1. 全局定义的，方法里面定义的而不是参数形式，也属于静态Block
2. NSStackBlock 栈区block，位于内存的栈区，一般作为函数的参数出现。 
3. NSMallocBlock 堆区block，位于内存的堆区，一般作为对象的property出现。

如果一个blcok引用了外部变量是栈block，则其不引用外部变量就成为了静态blcok。 
如果一个block引用了外部变量是堆block，则其不引用外部变量就成为了静态block。

[iOS block之三种block](https://blog.csdn.net/Mo_Mo123/article/details/77923634)

### Block和delegate的比较【阿里】

1. delegate运行成本低，block的运行成本高。
    1. block出栈需要将使用的数据从栈内存拷贝到堆内存，当然对象的话就是加计数，使用完或者block置nil后才消除。delegate只是保存了一个对象指针，直接回调，没有额外消耗。就像C的函数指针，只多做了一个查表动作。
2. 从使用场景区别block和delegate
    1. 有多个相关方法。假如每个方法都设置一个 block, 这样会更麻烦。而 delegate 让多个方法分成一组，只需要设置一次，就可以多次回调。当多于 3 个方法时就应该优先采用 delegate。当1，2个回调时，则使用block。
    2. delegate更安全些，比如: 避免循环引用。使用 block 时稍微不注意就形成循环引用，导致对象释放不了。这种循环引用，一旦出现就比较难检查出来。而 delegate 的方法是分离开的，并不会引用上下文，因此会更安全些。
    3. Block 是一种轻量级的回调，能够直接访问上下文，使用块的地方和块的实现地方在同一个地方，使得代码组织更加连贯
    4. Delegate 相对来说是重量级的回调
    4. delegate回调返回的参数被限制在了 NS 类的范围内，数量也很有限
3. 共同点：Block 和 Delegate 中的方法都可以理解成回调函数，当某件事情发生的时候取执行一段代码片段

[iOS中block和delegate的区别(面试必问)](https://blog.csdn.net/u010670946/article/details/71340711)

### Block和通知的区别，分别适用什么场景【腾讯】

Block：一对一的通信
Block更加简洁，不需要定义繁琐的协议方法，但通信事件比较多的话，建议使用Delegate；
通知：一对多、多对一的通信

* Block
    * 相互关联的两个对象之间进行传值，使用 Block 可以简化传值操作
* 通知：
    * 1、很多控制器都需要知道一个事件，应该用通知；
    * 2、相隔多层的两个控制器之间跳转

### 了解循环引用吗【网易】

对象之间相互强引用就会造成循环引用，使得对象内存得不到释放

### Block的循环引用、如何解决、原理【阿里】

**发生原因**：循环引用的造成原因就是相互强引用
**解除原理**：去掉相互强引用的其中一条强引用，改为弱引用

而解决该问题的方式是在MRC下定义：
__block typeof(self) weakself =self;
在ARC下定义：
__weak typeof(self) weakself =self;

```
__weak typeof (self) weakSelf = self; 
model.block = ^(){
    //再来一次 __strong 就比较严谨了，可以避免self在 Block 外面已经被释放了但是Block还没执行完
    __strong typeof (weakSelf) strongSelf = self;
    if (!strongSelf) return; //这里最好加上判断
    XXXXXX
}
```

**解释：**在里面是用__strong的原因是因为防止block在执行的时候外部的self对象被释放掉了。这时候block内部的weakSelf就会为nil。所以block内部要有一个强指针指向self对象，当block代码执行完了之后释放。这里__strong可以省略（系统默认），为了可读性可以写。

```
#ifndef weakify
    #define weakify(o)   __typeof__(o) __weak o##__weak_ = o;
    #define strongify(o) __typeof__(o##__weak_) __strong o = o##__weak_;
#endif

weakify(self);
success:^(AFHTTPRequestOperation *operation, id responseObject) {
    strongify(self);
    if (!self__weak_) return ;
   //...................
}
```

* weakify(self); 创建一个指向self的弱引用
* strongify(self); 当加上修饰符strong时，获取self引用，当别处把“self”释放掉，但调用该“self”的block如果仍然没有执行结束，那么系统就会等待block执行完成后再释放，对该“self”在block中的使用起到了保护作用。当block执行结束后会自动释放掉。
* if (!self__weak_) return ; ** 进行判断，如果在执行strongify(self)之前“self已经被释放掉了，则此时self=nil，所以直接return即可”**

[block解决循环引用详细解释](https://www.jianshu.com/p/4384a42778bc)

### block修改外部变量值，block是否会循环引用，怎么解决【阿里】

可能会，如果修改的是引用了Block的对象，可能会产出循环引用
使用 
__weak typeof(self) weakself =self;
__strong typeof (weakSelf) strongSelf = self;
组合使用可以避免 循环引用

### __block什么时候用【网易】

```
int b = 0;
void (^blo)() = ^{
    NSLog(@"Input:b=%d",b);
};
b = 3;
blo(); //输出Input:b=0
```

虽然我们在调用blo之前改变了b的值，但是输出的还是Block编译时候b的值，所以截获瞬间自动变量就是：在Block中会保存变量的值，而不会随变量的值的改变而改变

```
int b = 0;
void (^blo)() = ^{
    b = 3;
};
```

👆这段代码编译出错，编译器提示的大概就是不能在Block中改变变量的值。因为在Block中截获了变量的瞬间值以后就不能再改变变量的值，如果想要在Block中改变变量的值，那么我们只需要在变量声明的时候加上__Block修饰符，

```
NSMutableArray *array = [[NSMutableArray alloc]init];
void (^blo)() = ^{
    [array addObject:@"Obj"];
};
```

为什么呢，因为我们只是对截获的变量进行了操作，而没有进行赋值，所以对于截获变量，可以进行操作而不可以进行赋值。

[iOS-Block的使用你看我啊](https://www.jianshu.com/p/ce238bd58d5b)

### 在block里面, 对数组执行添加操作, 这个数组需要声明成 __block 吗【网易】

不需要，只要不是进行赋值造成

### 在block里面, 对NSInteger进行修改, 这个NSInteger是否需要声明成__blcok【网易】

需要，否则会报错
![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121144537.png)

>Block 不允许修改外部变量的值，这里所说的外部变量的值，指的是栈中指针的内存地址。__block 所起到的作用就是只要观察到该变量被 block 所持有，就将“外部变量”在栈中的内存地址放到了堆中。进而在block内部也可以修改外部变量的值。

## iOS：Runloop/Runtime

### Runloop【网易】

一般来讲，一个线程一次只能执行一个任务，执行完成后线程就会退出。如果我们需要一个机制，让线程能随时处理事件但并不退出，通常的代码逻辑是这样的：

```
function loop() {
    initialize();
    do {
        var message = get_next_message();
        process_message(message);
    } while (message != quit);
}
```
这种模型通常被称作 Event Loop。 Event Loop 在很多系统和框架里都有实现，比如 Node.js 的事件处理，比如 Windows 程序的消息循环，再比如 OSX/iOS 里的 RunLoop。实现这种模型的关键点在于：如何管理事件/消息，如何让线程在没有处理消息时休眠以避免资源占用、在有消息到来时立刻被唤醒。

所以，RunLoop 实际上就是一个对象，这个对象管理了其需要处理的事件和消息，并提供了一个入口函数来执行上面 Event Loop 的逻辑。线程执行了这个函数后，就会一直处于这个函数内部 "接受消息->等待->处理" 的循环中，直到这个循环结束（比如传入 quit 的消息），函数返回。

OSX/iOS 系统中，提供了两个这样的对象：NSRunLoop 和 CFRunLoopRef ：

* CFRunLoopRef 是在 CoreFoundation 框架内的，它提供了纯 C 函数的 API，所有这些 API 都是线程安全的。
* NSRunLoop 是基于 CFRunLoopRef 的封装，提供了面向对象的 API，但是这些 API 不是线程安全的。


### 了解runtime吗【网易】

Runtime：指一个程序在运行（或者在被执行）的状态。也就是说，当你打开一个程序使它在电脑上运行的时候，那个程序就是处于运行时刻。在一些编程语言中，把某些可以重用的程序或者实例打包或者重建成为“运行库"。这些实例可以在它们运行的时候被连接或者被任何程序调用。

`Objective-C`中`Runtime`：是一套比较底层的纯C语言API，属于1个C语言库，包含了很多底层的C语言API。在我们平时编写的OC代码中, 程序运行过程时，其实最终都是转成了runtime的C语言代码。

### Runtime什么时候用【网易】

1、动态创建一个类(比如KVO的底层实现)
2、动态地为某个类添加属性\方法, 修改属性值\方法
3、遍历一个类的所有成员变量(属性)\所有方法
4、使用 Method Swizzing 黑魔法的时候

### 消息发送和转发机制(消息调用的过程)，SEL和IMP。【美团、网易、阿里】

**消息发送**
在Objective-C中，使用对象进行方法调用是一个消息发送的过程（Objective-C采用“动态绑定机制”，所以所要调用的方法直到运行期才能确定）

objc在向一个对象发送消息时，runtime库会根据对象的 isa 指针找到该对象实际所属的类，然后在该类中的方法列表以及其父类方法列表中寻找方法运行，然后在发送消息的时候，objc_msgSend方法不会返回值，所谓的返回内容都是具体调用时执行的。那么，回到本题，如果向一个 nil 对象发送消息，首先在寻找对象的 isa 指针时就是0地址返回了，所以不会出现任何错误。

**转发机制**

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121150802.png)

1. 消息转发第一步：resolveInstanceMethod，动态方法解析，如果自己已经实现对该消息的处理则跳转处理方法，如果没有则进入第二步
2. 消息转发第二步：forwardingTargetForSelector 是否有备用的消息接受者，没有进行到第三步
3. 消息转发第三步：forwardInvocation 完整的消息转发
4. 消息转发第四步：调用doesNotRecognizeSelector：消息未能处理，抛出异常，默认的实现是抛出异常。

[Objective-C 消息发送与转发机制原理](http://yulingtianxia.com/blog/2016/06/15/Objective-C-Message-Sending-and-Forwarding/)

**SEL**：类成员方法的指针，但不同于C语言中的函数指针，函数指针直接保存了方法的地址，但SEL只是方法编号。
也就是说方法编号SEL最后还是要通过Dispatch table表寻找到对应的IMP，IMP就是一个函数指针，然后执行这个方法
**IMP**是 ”implementation” 的缩写，一个函数指针，它是 Objetive-C 方法(method)实现代码块的地址，可像C函数一样直接调用。通常情况下我们是通过 [object method:parameter] 或 objc_msgSend() 的方式向对象发送消息，然后 Objective-C 运行时(Objective-C runtime)寻找匹配此消息的IMP，然后调用它；但有些时候我们希望获取到IMP进行直接调用。

### 介绍一下Runtime怎么工作的？还能做些什么？【头条】

这里面写的很详细：[iOS模式详解runtime面试工作](https://blog.csdn.net/qq_36819141/article/details/75125648)

### 谈谈你对Objective-C的动态绑定理解？【京东】 

具体方法的调用从编译时推迟到了运行时，编译的时候不知道对象可能调用那个方法，根据运行时的状态参数来进行判断

个人回答方向是从 runtime 机制切入，对所有的 Object、Class 都进行对象化封装，对 clang 对 objc 的结构体改写转换来分析这个问题的。然后引入了 isa 指针和 swizzling method 等相关知识。（故意挖坑，因为自己在这方面比较擅长） 

### 如果想要删除自己的一段代码，如何删除（在程序执行的过程中删除）【美团】

提示：编译链接的过程

## iOS：其他

### 多态【腾讯】

面向对象有三大特性，封装、继承和多态。

封装就是将一类事物的属性和行为抽象成一个类，使其属性私有化，行为公开化，提高了数据的隐秘性的同时，使代码模块化。这样做使得代码的复用性更高。**模块复用**

继承则是进一步将一类事物共有的属性和行为抽象成一个父类，而每一个子类是一个特殊的父类--有父类的行为和属性，也有自己特有的行为和属性。这样做扩展了已存在的代码块，进一步提高了代码的复用性。**代码复用**

如果说封装和继承是为了使代码重用，那么多态则是为了实现接口重用。多态的一大作用就是为了解耦--为了解除父子类继承的耦合度。如果说继承中父子类的关系式IS-A的关系，那么接口和实现类之之间的关系式HAS-A。简单来说，多态就是允许父类引用(或接口)指向子类(或实现类)对象。很多的设计模式都是基于面向对象的多态性设计的。**接口复用**


### 有序和无序set实现原理区别【网易】

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121153711.png)

有序使用

### NSArray、NSSet、NSDictionary的效率【头条】

* NSArray是对象的有序集合(可存储不同类型的对象),在内存中存储位置是连续的
* NSSet是对象的无序集合(可存储不同类型的对象),在内存中存储方式是不连续的
* NSDictionary是键值对的集合(可存储不同类型的对象),注意key在整个字典中是唯一的,若多个key相等,也只能取出一个

如果insert的效率高，下次get的时候效率就低，比如无序的Array，插入的时候O（1），查找的时候就变O（N）。
如果想要查找的速度快，比如排序过的Array，查找的速度在O（logN），插入的时候就必须要保持Array有序这一特性O（N）。
所以插入和查找是鱼与熊掌

hash方法的返回值是一个NSUInteger，这个值往往和对象在内存当中的存储位置直接相关，也就是说我们可以通过这个值以O（1）的复杂度快速读取到某个对象来判断相等性

hash可以更加高效快速的判断一个对象是否存在集合当中

[NSArray,NSDictionary,NSSet 当中的算法知识](http://ios.jobbole.com/90323/)

### 存一个通讯录，包括增删改查，用什么数据结构【腾讯】

数组➕字典就可以实现简单地实现

### 事务的特征【阿里】

一．什么是事务：
事务是应用程序中一系列严密的操作，所有操作必须成功完成，否则在每个操作中所作的所有更改都会被撤消。也就是事务具有原子性，一个事务中的一系列的操作要么全部成功，要么一个都不做。 
事务的结束有两种，当事务中的所以步骤全部成功执行时，事务提交。如果其中一个步骤失败，将发生回滚操作，撤消撤消之前到事务开始时的所以操作。 

事务四大特征：原子性，一致性，隔离性和持久性(ACID)

1. 原子性：事务是数据库的逻辑工作单位，事务中包含的各操作要么都做，要么都不做 
2. 一致性： 事务执行的结果必须是使数据库从一个一致性状态变到另一个一致性状态。因此当数据库只包含成功事务提交的结果时，就说数据库处于一致性状态。如果数据库系统 运行中发生故障，有些事务尚未完成就被迫中断，这些未完成事务对数据库所做的修改有一部分已写入物理数据库，这时数据库就处于一种不正确的状态，或者说是 不一致的状态。 
3. 隔离性：一个事务的执行不能其它事务干扰。即一个事务内部的操作及使用的数据对其它并发事务是隔离的，并发执行的各个事务之间不能互相干扰。 
4. 持续性：也称永久性，指一个事务一旦提交，它对数据库中的数据的改变就应该是永久性的。接下来的其它操作或故障不应该对其执行结果有任何影响。 

### 持久化，iOS中数据持久化的几种方式【阿里】

1. Plist文件（属性列表）
2. Preference（偏好设置）
3. NSKeyedArchiver（归档）
4. SQLite 3
5. CoreData
6. KeyChain 保存敏感账号密码

### 做过数据库没，Core Data【网易】

有使用过，但是没有直接只用 Core Data
Core Data 的直接操作

### 你项目中的数据具体缓存怎么做的。【阿里】

属性列表，KeyChain，归档，都有使用

### layoutIfNeeded和setNeedsLayout的区别【头条】

* **layoutSubviews：**更新布局总会重新触发layoutSubviews方法，继承于UIView的子类重写，进行布局更新，刷新视图。如果某个视图自身的bounds或者子视图的bounds发生改变，那么这个方法会在当前runloop结束的时候被调用。为什么不是立即调用呢？因为渲染毕竟比较消耗性能，特别是视图层级复杂的时候。这种机制下任何UI控件布局上的变动不会立即生效，而是每次间隔一个周期，所有UI控件在布局上的变动统一生效并且在视图上更新，苹果通过这种高性能的机制保障了视图渲染的流畅性。
* **setNeedsLayout：**标记为需要重新布局，异步调用layoutIfNeeded刷新布局，不立即刷新，在下一轮runloop结束前刷新，对于这一轮runloop之内的所有布局和UI上的更新只会刷新一次，layoutSubviews一定会被调用。
* **layoutIfNeeded：**如果有需要刷新的标记，立即调用layoutSubviews进行布局（如果没有标记，不会调用layoutSubviews）。

[setNeedsLayout与layoutIfNeeded的区别](https://www.jianshu.com/p/d46bcc656e04)

### 如何让一个label靠左，一个label靠右，然后右边的label能够完全显示【美团】

需要根据情况进行判断，如果左边设置一个固定的最小值
或者实时计算右边label能显示的内容

### 使用自动布局，把三个view横向等宽等间距（与父view边距也相等）排列。【头条】

Easy

### 自动布局（设置约束）和手动布局（设置frame）的优缺点，哪个效率高，为什么？【头条】

自动布局
优点：适配方便
缺点：比较耗性能

手动布局
优点：适配麻烦
缺点：写代码麻烦

手动布局无须进行后续计算，直接进行渲染

### 中途还讨论了Masonry的约束应该写在哪里，我说应该写在layoutSubViews，他说会调用多次，然后争论了一会儿【阿里】

我觉得不能设置在 layoutSubViews,

### 如何扩大view的响应范围【美团】

重写 hitTest 方法，或者 PonitInside 方法

* 让视图不相应事件，重写 hitTest 方法

### 浅拷贝和深拷贝的区别【阿里】

一个拷贝指针地址，一个进行对象拷贝复制出另外一份

### 数组的浅拷贝与深拷贝【头条】

具体使用还是要看情况吧

### 数组copy后里面的元素会复制一份新的吗【头条】

其实并不会，数组本身保存的就是元素的指针地址

```
//实现数组元素拷贝的方式一：
[[NSMutableArray alloc] initWithArray:arr1 copyItems:YES]

//实现数组元素拷贝的方式二：
for (Model *model in arr) {
  [arr1 addObject:[model copy]];//这里的copy,就是将arr数组里的每一个对象拷贝一份.
   //所以Model对象实现- (id)copyWithZone:(nullable NSZone *)zone方法
}
```

[参考：iOS 数组元素的深拷贝](https://www.jianshu.com/p/976070ac4949)

### 上线APP的crash收集。【网易】

使用腾讯Bugly进行收集，开始配置好Shell脚本，打包的时候就会自动上传.syb文件
然后可以实现在线就解析出崩溃日志

### iOS7之后, 蓝牙的围栏功能【阿里】

所谓iBeacons，就是一种使用蓝牙低能耗进行微定位的技术，它允许iOS设备使用蓝牙4.0获取位置数据。也就是说，配备iBeacons技术的iOS设备就相当于位置数据的接收方和发送方，在蓝牙时代里进行着数据的互联。

iBeacon的出现让地理定位能够更加精确——从几百米的精度提高到了一米甚至半米。这个精细度非常高的地理围栏，终于可以让很多的实际物体都有条件具有了定义自己地理位置标识的能力

[iOS蓝牙开发之iBeacon篇(一)](https://sevencho.github.io/archives/1f6c5df3.html)

### UIView做动画方法的底层实现 【网易】

* 逐帧动画：类似于上面提到的手绘翻页方式，我们可以将这个水杯在每帧画面中的位置一一找出来，这样实现动画的方式就叫作 逐帧动画
* 关键帧动画：是指的广义上的一种动画制作方式，并不仅指 CAKeyframeAnimation，CABasicAnimation的实现方式也属于 关键帧动画

动画的本质
继续用上面的简单例子：一个 UIView 从 (0,0) 匀速移动到 (100,0)的动画，动画总时间是0.25秒。
假设我们基于 60 FPS 来显示动画，那么在0.25秒内就应该有15帧画面，在每帧画面中，这个 UIView 的 x坐标，每次应移动 100/15 的距离。
如果我们每隔 0.25/15 秒刷新一次UIView 的 x 坐标，那么就能实现这个动画效果了。
对于 x坐标而言，每帧的位置就可以通过一个基于时间变化量的函数来求得：x=f(t) 。

所以，一个动画的本质，就是动画对象（这里是 UIView）的状态，基于时间变化的反应了。
简单说，就是给定任意一个时刻，如果你都能得到这个动画对象的位置和、形状等等属性，你就能实现这个动画了。
属性值的变化，既可能是位置、透明度、旋转角度等的变化，也包括形状的改变，比如从一条直线变化成一个圆圈，目标就是要得到变化过程中特定时刻的中间态。

1.00 秒   60 帧动画
0.25 秒   15帧动画
每个帧移动的距离就是  100 / 15  =  距离
x = f(t)
给定任意时刻，动画对象的位置和形状等属性，就可以实现一个简单的动画。。。

[解析 iOS 动画原理与实现](https://www.jianshu.com/p/13c231b76594)

### Tableview上拉下拉刷新的原理【美团】

核心就是监听 contentOffset.y 的值
下拉： contentOffset.y 减小
上拉： contentOffset.y 增大

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121170538.png)

[UITableView的上拉加载更多和下拉刷新原理](https://blog.csdn.net/zhuming3834/article/details/49446953)

### 断点的实现方式，app是如何停止在断点的【网易】

CPU有一个单独的执行序列，会一条指令一条指令的顺序执行。要处理类似IO或者硬件时钟这样的异步事件时CPU就要用到中断。硬件中断通常是一个专门的电信号，连接到一个特殊的“响应电路”上。这个电路会感知中断的到来，然后会使CPU停止当前的执行流，保存当前的状态，然后跳转到一个预定义的地址处去执行，这个地址上会有一个中断处理例程。当中断处理例程完成它的工作后，CPU就从之前停止的地方恢复执行。

[调试器工作原理（2）：实现断点](http://blog.jobbole.com/23632/)

### 动画掉帧，CADisPlayLink，Core graphics 【网易】



### 如何通过一个view查找它所在的ViewController【美团】

情况一：向上递归寻找父视图，判断父视图是否是ViewController
情况二：View在Cell上，就需要找到TableView，进而找到ViewController

### AFN，URLSession，相互关系。【网易】

### Pod update和pod install的区别【头条】

**pod install：**执行该命令时，如果Podfile.lock文件存在, 则直接从此文件中读取框架信息并且它会只下载Podfile.lock文件中指定的版本安装。对于不在Podfile.lock文件中的pod库，pod install命令会搜索这个pod库在Podfile文件中指定的版本来安装；如果Podfile.lock不存在, 则会读取Podfile文件内的框架信息，然后执行下载并且根据下载好的框架信息, 生成Podfile.lock文件。
**pod update：**只有当你想要更新pod库的版本时才使用pod update；它不管Podfile.lock是否存在, 都会读取Podfile文件的的框架信息去下载安装，下载好之后, 再根据下载好的框架信息, 生成Podfile.lock文件

**pod install使用：**
1、这个是第一次在工程里面使用pods的时候使用，并且，也是每次你编辑你的Podfile（添加、移除、更新）的时候使用。
2、当你在你的Podfile里面添加了一个库的时候，你应该使用pod install，而不是pod update
3、每个人从共享库把项目下载下来之后, 都会执行pod install 命令安装，而不是选择 pod update，这样是为了保证大家使用的第三方框架版本一致。
**pod update使用：**
1、你应该使用pod update去更新某个特定的库，或者所有的库（在Podfile的限制中）
2、你应该使用pod update PODNAME去只更新某个特定的库（检查是否有新版本，并尽可能更新到新的版本）
3、如果以后大家需要统一升级第三方框架, 那么每个人在执行 pod update

[英文：官方文档](https://guides.cocoapods.org/using/pod-install-vs-update.html)
[中文：使用 pod install 还是 pod update ？](https://www.jianshu.com/p/a977c0a03bf4)

### 静态库和动态库区别【网易】

**静态库：**链接时，静态库会被完整地复制到可执行文件中，被多次使用就有多份冗余拷贝
**系统动态库：**链接时不复制，程序运行时由系统动态加载到内存，供程序调用，系统只加载一次，多个程序共用，节省内存
![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121000808.png)

系统的.framework是动态库，我们自己建立的.framework一般都是静态库

**a与.framework有什么区别？**
.a是一个纯二进制文件，.framework中除了有二进制文件之外还有资源文件。
.a文件不能直接使用，至少要有.h文件配合，.framework文件可以直接使用。

[ios静态库与动态库的区别](https://www.jianshu.com/p/2f16bf7b0009)

### Ipa 文件内容【网易】

1. 二进制的可执行文件
2. 苹果签名
3. 苹果证书
4. 各种资源文件：icon、第三方Bundle、国际化文件等

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121160554.png)

### App签名【网易】

[如何理解 iOS 的签名证书机制](https://juejin.im/entry/58ff10bf1b69e60058abb6b8)
[iOS App 签名的原理](http://blog.cnbang.net/tech/3386/)

### 程序执行的过程【美团】

1. 加载dyld(Apple 的动态链接器)到App进程(dyld的全称是dynamic loader，它的作用是加载一个进程所需要的image，dyld是开源的。)
2. 加载动态库（包括所依赖的所有动态库） 
3. Rebase：修正内部(指向当前mach-o文件)的指针指向
4. Bind：修正外部指针指向
5. 初始化Objective C Runtime 
6. 其它的初始化代码

[iOS 程序启动流程解密](https://www.jianshu.com/p/d08732c84ebb)
[深入理解iOS App的启动过程](https://blog.csdn.net/Hello_Hwc/article/details/78317863)
[sunnyxx大神：iOS 程序 main 函数之前发生了什么](https://blog.sunnyxx.com/2014/08/30/objc-pre-main/)

### iOS里面的事件响应链【头条、美团】

1. **事件的响应**：显示被触摸的视图，看自己能否响应，然后依次到父视图…..到 UIWindow，直到被抛弃
2. **事件的处理**：父视图，到子视图，依次寻找，直到没有子视图，然后自己就是事件的处理者
3. 事件需要先**响应**，然后再**处理**，一个来回操作：子视图到父视图，父视图再到子视图


当发生事件响应时，必须知道由谁来响应事件。在 iOS 中，由响应者链来对事件进行响应。

所有事件响应的类都是 UIResponder 的子类，响应者链是一个由不同对象组成的层次结构，其中的每个对象将依次获得响应事件消息的机会。**当发生事件时**，事件首先被发送给第一响应者，第一响应者往往是事件发生的视图，也就是用户触摸屏幕的地方。事件将沿着响应者链一直向下传递，直到被接受并做出处理。一般来说，第一响应者是个视图对象或者其子类对象，当其被触摸后事件被交由它处理，如果它不处理，事件就会被传递给它的视图控制器对象 ViewController（如果存在），然后是它的父视图（superview）对象（如果存在），以此类推，直到顶层视图。接下来会沿着顶层视图（top view）到窗口（UIWindow 对象）再到程序（UIApplication 对象）。如果整个过程都没有响应这个事件，该事件就被丢弃。一般情况下，在响应者链中只要由对象处理事件，事件就停止传递。

我们可以通过 [responder nextResponder] 找到当前 responder 的下一个 responder，持续这个过程到最后会找到 UIApplication 对象

-- 

应用如何找到最合适的控件来处理事件？

1.首先判断主窗口（keyWindow）自己是否能接受触摸事件
2.判断触摸点是否在自己身上
3.子控件数组中从后往前遍历子控件，重复前面的两个步骤（所谓从后往前遍历子控件，就是首先查找子控件数组中最后一个元素，然后执行1、2步骤）
4.view，比如叫做fitView，那么会把这个事件交给这个fitView，再遍历这个fitView的子控件，直至没有更合适的view为止。
5.如果没有符合条件的子控件，那么就认为自己最合适处理这个事件，也就是自己是最合适的view。

UIView不能接收触摸事件的三种情况：

1. 不允许交互：userInteractionEnabled = NO
2. 隐藏：如果把父控件隐藏，那么子控件也会隐藏，隐藏的控件不能接受事件
3. 透明度：如果设置一个控件的透明度<0.01，会直接影响子控件的透明度。alpha：0.0~0.01为透明。

-- 

![](https://image-1258017831.cos.ap-guangzhou.myqcloud.com/20181121171910.png)

事件处理的整个流程总结：

>1. 触摸屏幕产生触摸事件后，触摸事件会被添加到由UIApplication管理的事件队列中
>2. UIApplication会从事件队列中取出最前面的事件，把事件传递给应用程序的主窗口，这时候执行事件传递流程 找到一个最合适的视图来处理触摸事件。（这时候如果某一个view上添加了手势，且该手势能响应对应事件，则走手势的响应，根据手势的设置来决定是否阻断下面的步骤，但是事件传递过程依旧。如没有或者不能响应则继续走下面步骤）
>3. 最合适的view会调用自己的touches方法处理事件 如果需要的话可以把事件顺着响应者链条向上抛。

[iOS响应链(Responder Chain)](https://www.jianshu.com/p/4155c9ffe1a8)

### id ,NSObject, id<NSObject>区别【网易】


### NSObject 和 《NSObject》的区别，为什么要有后者 【网易】


### delegate转block怎么处理，比如把 NSURLConnection 的delegate转成block。【美团】

* 添加 Block 属性

### OC允许多继承吗，要用什么方式实现多继承【阿里】

不允许
**原因：**这是因为消息机制名称查找发生在运行时而非编译时，很难解决多个基类可能导致的二义性问题

实现多继承：

* 1、组合的方式：把需要继承的基类，作为属性添加到类中，这样就可以调用基类的方法
* 2、delegate和protocol：将C类需要继承的方法以及属性在ClassA和ClassB中各自声明一份协议，C类遵守这两份协议，同时在C类中实现协议中的方法以及属性
* 3、消息转发（快速转发和标准转发）：当向某个对象发送消息，但runtime system在当前类以及父类中都找不到对应方法的实现时，runtime system并不会立即报错使程序崩溃，而是依次执行下列步骤
* 4、类别（category）：通过category实现“单继承”

### 异步下载如何实现【阿里】

让耗时的操作在子线程中执行，下载完毕再到主线程中更新UI

### 说说Cell重用原理，Cell重用机制具体怎么实现【阿里】

**重用原理：**当滚动列表时，部分UITableViewCell会移出窗口，UITableView会将窗口外的UITableViewCell放入一个对象池中，等待重用。当UITableView要求dataSource返回UITableViewCell时，dataSource会先查看这个对象池，如果池中有未使用的UITableViewCell，dataSource会用新的数据配置这个UITableViewCell，然后返回给UITableView，重新显示到窗口中，从而避免创建新对象

cellForRowAtIndexPath
 [tableView dequeueReusableCellWithIdentifier:CellIdentifier];

### 不用框架，谈谈你如何处理图片缓存以及优化【阿里】

### 异步网络图片加载的设计思路。【京东】
根据 sdwebimage 三方库的源码对其进行分析。尤其是 Category 对于URL的关联对象、operation 的 hash 表管理、download 方法的 cache、disk 查询方式这三个地方。（面试官是很满意的） 
 
### 异步网络接口的缓存机制。【京东】
这个LZ曾经没有接触过，我只是用白纸画了一个流程图。用更新个人信息的功能为例，切记加入时间戳、考虑有无网络环境、引入 sync 同步性问题即可。 
 
### 谈谈面向对象的含义【京东】
这个问题听到以后出乎意料。我理解成面试官在考察基础知识，便通过面向对象的三大特点来展开描述，并且用  objc 和 cpp 进行解释。并且与面向过程进行对比。（吹水题，不要冷场就好。） 


 



