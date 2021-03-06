> 此文档是鄙人对大三上课程的一些简陋看法，旨在帮助他人更清晰地认知大三上的生活，以更有效地规划时间，不当之处请多指教~

<!-- TOC -->

- [数字信号处理DSP](#数字信号处理dsp)
    - [课程](#课程)
    - [实践](#实践)
    - [应试](#应试)
- [数字通信原理](#数字通信原理)
    - [课程](#课程-1)
    - [实践](#实践-1)
    - [应试](#应试-1)
- [信息论](#信息论)
    - [课程](#课程-2)
    - [应试](#应试-2)
- [数字系统设计](#数字系统设计)
    - [课程](#课程-3)
    - [实践](#实践-2)
    - [应试](#应试-3)
- [专业选修课](#专业选修课)
    - [软件工程](#软件工程)
    - [微波技术（射频）](#微波技术射频)
- [实验课](#实验课)
    - [数字系统设计实验](#数字系统设计实验)
    - [通信原理实验](#通信原理实验)
    - [射频实验](#射频实验)
- [资料](#资料)
- [致谢](#致谢)

<!-- /TOC -->
### 数字信号处理DSP
#### 课程
14级课程由于某些原因转移到大三下，内容为对数字信号的分析和处理，包括《信号与系统》的离散部分，加入DFT、FFT信号变换方法，IIR、FIR滤波器设计等部分。整个体系结构是工科信号处理的基石，建议大家好好学，区别计算机的信息处理！本人的老师是宁更新，上课按照新视野教材内容讲解，说话比较不清楚让人昏昏欲睡，但是考试知识点会着重讲解，考核与评卷比较松。平时推荐薛洋老师和黄双萍老师的课程，是按照通用教材讲解的，课堂生动易懂，不过关键还是自己多花时间看书，推荐一本十分良心的书《深入浅出数字信号处理》

#### 实践
数字信号处理区别于互联网的信息处理，是对传感器采集的信息进行分析和处理，包括频域分析和设计滤波器等，里面涉及的数学和算法都是十分经典美妙的，对嵌入式硬件和dsp算法有较高要求。举个例子，设计一套判别一个西瓜好坏的方案，常用的办法是敲打西瓜听音响，分析声音的频域和过滤杂音，再判断西瓜好坏。其中，抓取敲声需要硬件adc设计，分析和过滤需要dsp算法，再将整套算法转换为芯片又需要硬件设计。顺带一提，根据敲声判别好坏估计只有30%准确率，得结合瓜蒂、色泽等信息判别，利用线性模型、决策树等机器学习算法进行数据处理，能大大提高准确率，这类似于互联网的信息处理。

#### 应试
难度：5颗星

平时：理解不难但知识点较多，要下苦功夫跟上老师进度

备考：掌握知识点不算难，但是考试会考偏和挖坑，所以复习的时候尽可能多复习些重要知识点。出试卷的形式是每位老师负责一部分题目，最后结合起来成为试卷。一方面总体试题难度增加，另一方面老师无法提前得知重点，只有认真且全面地学习才能保证好分数。有份手抄卷可以参考见末尾的资料链接~

### 数字通信原理
---
#### 课程
学习数字信号传输的过程：抽样-》量化-》各类数字调制方式（区分通信电子线路的模拟调制）-》基带传输&&频带传输-》信道均衡-》最佳接收-》定时&&同步&&判决，此外还有扩频和信道复用技术，涉及《信号与系统》知识并且是概率论重灾区。课程跟华工新版教材的《数字通信原理》紧密相连，而与名气较大的樊昌信《通信原理》有较大差别，因此建议购买学校新版教材，另外推荐看国外教材《数字通信》，以及华为工程师所写的[深入浅出通信原理连载](http://forum.c114.net/thread-394879-1-1.html "深入浅出通信原理连载")，一股老学究风味~ 李波老师讲课挺好的，缺点是赶进度语速有点快。
#### 实践
数字通信原理和接下来说的信息论，课程工程性质不强，主要是理论推导，可以使用万能的matlab做OFDM干扰均衡仿真等通信研究（matlab带有通信工具包）。通信工程中一般会利用FPGA并行处理的特点，大规模地、快速地处理信号数据，通信算法和matlab写的差不多，所以不必要特地用FPGA实现。

#### 应试
难度：5颗星

平时：理解课程知识点不算特别难，但知识量大且学时少，掌握各知识点细节很不容易，而出卷人喜爱广泛地挖坑和深入探讨（余翔宇老师风格--），建议平时认真听课完成作业，重要知识点做标记。

备考：知识量大，建议收集好考试重点。多留些时间复习，熟悉各种概念，小题不容易做对，大题有计算、推导重要公式或者结论、画框图等。一些往年题型可以参考回忆版试卷（资料包附有）

### 信息论
---
#### 课程
与数字信号处理互补，内容是为提高通信效率和质量，对传输信号进行信源编码（最大熵、霍夫曼）和差错控制编码（线性分组码、循环码、卷积码）。名气很大的《信息论基础》by Thomas M.Cover 内容过多且较难，相比之下华工老师的ppt和教材更适合本科学习，推荐一本闲书《信息简史》

#### 应试
难度：3颗星

平时：目前各班信息论老师似乎都有点乏力，没能把课程讲好，不过课程不难踏踏实实学习就好，通过请教他人和刷作业题等途径来理解知识。

备考：课程虽然是从通信原理抽出两章，但知识点不算少，需要多花点时间复习。试卷小题偏难，大题一般难度，多刷刷往年卷。

### 数字系统设计
---
#### 课程
以数电为基础，学习整个数字系统设计的过程，包括VHDL语言、仿真、综合等，而不是单单学习VHDL语言，解决问题时善于利用状态机。建议追加学习Verilog语言，原因有两个：
- VHDL语言在工程上如同汇编，很难应用到实践中，如果做项目或者实现复杂一点的功能，使用Verilog会方便很多
- 学习Verilog的过程中，会认知到更多概念，比如说阻塞、同步异步等。这是鄙人在期末复习时注意到的，华工教材偏向概括整个设计流程，建议多学习些。

工程性很强的课程，没什么书籍推荐，多上手开发板更好些。李磊老师讲课水平一般，邢晓芬老师（院长夫人）讲课非常好。
#### 实践
> 没有真正做过相关工程，如果有行家看到应该明白鄙人说得力不从心，劳烦修正一下

FPGA解决的问题是数字电路的前端验证设计，同时由于其灵活、并行等优秀特性，适合解决高速处理数据等问题，应用在通信高速接口设计、数字信号处理等。浅谈一下几个主流方向，目前如果感兴趣建议找一套开发板学习：
- 仿真验证：试着仿真几种时序比如IIC,SPI,VGA等，能让显示器工作，再去尝试更复杂的协议，一般需要配逻辑分析仪、示波器分析波形。
- 信号处理：灵活强大的FPGA适能快速地适应通信标准并实时地完成大量运算，比如在通信的纠错编码、基带调制解调，以及配合DSP应用在图像编码解码，雷达信号处理，医学信号处理等领域

#### 应试
难度：2颗星

平时：没有作业，认真听讲就好，vhdl语法部分多练代码，系统设计部分多记概念。

备考：考试比较简单，结合课本和ppt复习，刷刷往年卷，熟悉使用状态机并默写完整代码，如果是邢老师出题，注意看课上讲的重点题目。

### 专业选修课
---
#### 软件工程
主要讲解软件工程上的概念和方法，如果没有实战经验可能难以领会。请注意上课、作业和考试不是学院统一的，只看任课老师风格。鄙人的老师是覃健诚，不点名，作业只有一个：小组完成快速原型法实现某软件，考试偏向于出各种画图题。
#### 微波技术（射频）
大概讲的是超高频率下的各类元件的特性、应用，设计射频电路模块比如滤波器、功分器等。考前老师一般会准确地划重点，试卷比较简单，但平时注意理解。
> 如果对射频不感兴趣可以申请退掉的，下学期再选其余的课程补够选修学分即可

### 实验课
---
#### 数字系统设计实验
> 先安利QuartusII 16，界面偏平好看，可以添加CycloneII的设备包（实验室的开发板是这款芯片），一般没问题，要是不成功或者图方便就安装QuartusII 9吧。

共有四次实验，使用vhdl语言和状态机方法做小实验，可以在宿舍先完成，然后在实验室玩弄一下开发板。也许开始不习惯写代码，模仿着慢慢就熟悉了。

期末后有课程设计，大家都会选择万年历，但鄙人觉得要看时序图写一个协议出来才算过关（现实是大家寒假都在玩最后抱佛脚）。鄙人负责写液晶的协议，但实验室提供的开发板液晶部分设计不合理，信号有串扰（另外还听说没有EEPROM的外设），改为用无协的黑金开发板就好。建议学习QuartusII的其余功能，有助于调试，网上有一些指南值得看~

#### 通信原理实验
中规中矩的实验课，使用实验板测量各类数据，跟着老师的步骤来即可。普通班无课程设计，电联班有用matlab仿真编码的课程设计，感兴趣可以了解一下。

#### 射频实验
老师会提供探索性实验和验证性实验两种选择，可以根据自己的规划选择，鄙人选的是探索性实验，同样安利给大家~

探索性实验：需要自行设计滤波器等，平时不用做实验，等理论课老师讲过滤波器后就开始，用软件设计，拿到实验室制版，写论文形式的报告，最后得分会比验证性实验高。得分是次要的，这个过程极大地加深我们对课程的理解，难度又不大花费的时间也不多！

验证性实验：测量实验室板子的数据，跟着老师的步骤走，简单不动脑，最终分数相比会低一些（分数有75+）

> 14级的《数字信号处理》在大三下学习，请前往大三下.md了解具体内容

### 资料
---
最后，是最期待的[资料链接](https://pan.baidu.com/s/1bo2Zgz9)及密码：mi07

### 致谢
---
任何帮忙的朋友都会在致谢中说明

欢迎补充和指正，由衷感激支持的捧油:smile:~
