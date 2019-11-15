# 编程必备基础

- 计算机组成原理
  - 概述篇
    - 计算机发展史
      - 计算机发展的四个阶段
        - 第一阶段 1946~1957（电子管计算机）：
          - 第二次世界大战是电子管计算机产生的催化剂，为了解密德国海军的密文。
          - 埃尼阿克（ENIAC）
            - 战争使用了飞机和火箭
            - 打得准，则需要计算射击参数
            - 射击参数需要几千次运算才能计算出来
            - 18000 多个电子管
            - 运行耗电量 150千瓦
            - 重量达 30 吨，占地 1500 平方英尺
            - 造价约为 48万美元
          - 集成度小，空间占用大；功耗高，运行速度慢；操作复杂，更换程序需要接线；
        - 第二阶段 1957~1964（晶体管计算机）：
          - 贝尔实验室的三位科学家发明了晶体管
          - 著名的晶体管计算机：TX-0（来自 MIT 林肯实验室）、PDP-1（4k内存，每秒200000指令，配备 512x512的显示器）
          - 集成度相对较高，空间占用相对小；功耗相对较低，运行速度较快；操作相对简单，交互更加方便；
        - 第三阶段 1964~1980（集成电路计算机）：
          - 德州仪器的工程师发明了集成电路（IC），从此以后更多的元件就被集成到了单一的半导体芯片里面使得计算机变得更小、功耗更低、计算速度更快。
          - 当时 IBM 为领头羊，两款计算机卖的很好：7094、1401，主打功能不同，相互也无法兼容，买了的公司不愿意投入两组人力，于是IBM 就推出了兼容的产品 System/360，这就是操作系统的雏形，使得不同的电子元器件，不同电路的计算机都能在同一个操作系统上面运行。
        - 第四阶段 1980~至今（超大规模集成电路计算机）：
          - 一个芯片集成了上百万的晶体管
          - 速度更快体积更小价格更低更能被大众接受
          - 用途丰富：文本处理、表格处理、高交互的游戏与应用
        - 第五阶段：未来的计算机
          - 生物计算机，以蛋白质分子作为主要原材料
          - 量子计算机，遵循量子力学的物理计算机
            - 2013年5月，谷歌和 NASA 发布 D-Wave Two
            - 2017年5月，中国科学院宣布制造出光量子计算机
            - 2019年1月，IBM 展示了世界首款商业化量子计算机
            - 2017年，腾讯组建了量子实验室，阿里巴巴成立了达摩院
      - 微型计算机的发展历史
        - 早期受限于性能，使用的是单核 CPU
          - （1971 ~ 1973）500KHz 频率的微型计算机（字长 8 位）
          - （1973 ~ 1978）高于 1MHz 频率的微型计算机（字长 8 位）
          - （1978 ~ 1985）500MHz 频率的微型计算机（字长 16 位）
          - （1985 ~ 2000）高于 1GHz 频率的微型计算机（字长 32 位）
          - （2000 ~ 至今）高于 2GHz 频率的微型计算机（字长 64 位）
          - 摩尔定律：集成电路的性能，每 18-24 个月就会提升一倍
        - 单核CPU遇到性能瓶颈，多核 CPU
          - （2005）Intel 奔腾系列双核 CPU、AMD 速龙系列
          - （2006）Intel 酷睿四核 CPU
          - Intel 酷睿系列十六核 CPU
          - 服务器领域，Intel 至强系列五十六核 CPU
    - 计算机分类
      - 超级计算机
        - 功能最强、运算速度最快、存储容量最大
        - 多用于国家高科技领域和尖端技术的研究，天气预报、海洋监测、生物制药、科学计算（核聚变核裂变模拟、加密解密算法）
        - 标记他们运算速度的单位是 TFlop/s，1TFlop/s=每秒一万亿次浮点计算，Intel（R）Core（TM）i7-6700k CPU@4.00 GHz：44.87GFlop/s，44.87GFlop/s = 0.01187TFlop/s
        - 截至 2018年11月。世界前三：Summit（美国IBM）、神威太湖之光（中国）、Sierra（美国IBM）。中国前三：神威太湖之光（国家并行计算机工程技术研究中心）、天河二号（国防科大，位于广州大学城-中山大学）、天河一号（国防科大）
      - 大型计算机
        - 又称大型机、大型主机、主机等
        - 具有高性能，可处理大量数据与复杂的运算，银行金融交易的数据、证券交易所的数据处理，人口普查、企业资源规划
        - 在大型计算机市城领域，IBM 占据着很大的份额，COBOL 编程语言
        - IBM Z9，NASA 最后一台大型机，Red Hat Enterprise Linux系统，大型机造价高昂，市场越来越小。
        - 2008年阿里提出去「IOE」行动，I（IBM 服务器提供商），O（Oracle 数据库软件提供商），E（EMC 存储设备提供商），这三者构成了从软件到硬件的企业级数据库系统，当时占领了大部分市城的商业数据库份额。因为「IOE」代表了高维护费用的存储系统，大型机也不够灵活，伸缩性弱，阿里巴巴就开始将海量数据从集中式的 Oracle 切换到了分布式的 MySql 集群，把大型机替换为普通服务器。解决数据库的拓展问题。阿里云 2009 年成立。
      - 迷你计算机（服务器）
        - 也成为小型机，普通服务器
        - 不需要特殊的空调场所
        - 具备不错算力，可以完成较复杂运算
        - 常见制造商：联想、华为、浪潮
        - 普通服务器代替了传统的大型机，成为大规模企业计算的中枢
        - 阿里云腾讯云等等的云厂商都是用这些普通的服务器来构成云服务与数据中心的
      - 工作站
        - 高端的通用微型计算机，提供比个人计算机更强大的性能
        - 类似普通台式电脑，体积较大，性能强劲，主要给图片工作者视频工作者使用。
      - 微型计算机
        - 又称为个人计算机
    - 计算机的体系结构
      - 冯诺伊曼体系：将程序指令和数据一起存储的计算机设计概念结构
        - 早期计算机仅含固定用途程序，改变程序得更改结构重新设计电路，于是就有存储程序指令设计通用电路
        - 必须有一个存储器，存储数据和指令
        - 必须有一个控制器，因为需要存储指令，所以必须知道执行到哪里，下一步该执行什么
        - 必须有一个运算器
        - 必须有输入设备
        - 必须有输出设备
        - 现代计算机都是冯诺依曼机
        - 能够把需要的程序和数据送至计算机中
        - 能够长期记忆程序、数据、中间结果及最终运算结果的能力
        - 能够具备算术、逻辑运算和数据传送等数据加工处理的能力
        - 能够按照要求将处理结果输出给用户
        - 冯诺依曼瓶颈：CPU 和存储器速率之间的问题无法调和，CPU 经常空转等待数据传输
      - 现代计算机结构
        - 现代计算机在冯诺依曼体系结构基础上进行修改
        - 解决 CPU 与存储设备之间的性能差异问题
        - 更高速的存储设备：内存、CPU的寄存器
        - 现代计算机的结构可以理解为以存储器为核心的结构
    - 计算机的层次与编程语言
      - 程序翻译与程序解释
        - 程序翻译是将较为高级的计算机语言通过编译器翻译成较为低级的计算机实际执行的语言。
        - 程序解释是将较为高级的计算机语言通过由较为低级的计算机语言实现的解释器解释成较为低级的计算机实际执行的语言。
        - Java 和 C# 属于翻译+解释型的语言，Java 先编译成 JVM 字节码 然后解释成机器码执行，是在 JVM 虚拟机中编写
      - 计算机的层次与编程语言
        - 实际机器
          - 硬件逻辑层
            - 门、触发器等逻辑电路组成
            - 属于电子工程的领域
          - 微程序机器层
            - 编程语言是**微指令集**
            - **微指令**所组成的**微程序**直接交由硬件执行
          - 传统机器层
            - 编程语言是**CPU 指令集（机器指令）**
            - 编程语言和硬件直接相关
            - 不同架构的 CPU 使用不同的 CPU 指令集
            - 机器指 = 微程序 > 微指令
        - 虚拟机器
          - 系统软件
            - 操作系统层
              - 向上提供了简易的操作界面
              - 向下对接了指令系统，管理硬件资源
              - 操作系统是在软件和硬件之间的适配层
            - 汇编语言层
              - 编程语言是**汇编语言**
              - 汇编语言可以**翻译**成可以直接执行的机器语言，完成翻译过程的程序就是汇编器
            - 高级语言层
              - 编程语言为广大程序员所接受的高级语言
              - 高级语言的类别非常多，有几百种
              - 常见的高级语言有：Python、Java、C/C++、Golang等
          - 应用软件
            - 应用层
              - 满足计算机针对某种用途而专门设计
    - 计算机的计算单位
      - 容量单位
        - 在物理层面，高低电平记录信息
        - 理论上只认识 0/1 两种状态，0/1 称为 bit（比特位）
        - 字节：1Byte = 8 bits，字节和比特位使用的是八进制位，1024=2^10
        - ![容量单位](images/容量单位.png)
        - 硬盘厂商一般用10 进位标记容量
      - 速度单位
        - 网络速度
          - 比如 100M 宽带
          - 为什么电信拉的100M光纤，测试峰值速度只有12M每秒？
          - 网络常用单位为（Mbps）
          - 100M/s = 100Mbps = 100Mbit/s
          - 100Mbit/s = (100/8)MB/s = 12.5MB/s
        - CPU 频率
          - CPU 速度一般体现为 CPU 的时钟频率
          - CPU 时钟频率的单位一般是赫兹（Hz）
          - 主流 CPU 的时钟频率都在 2GHz 以上
          - Hz 其实就是秒分之一，它是每秒钟的周期性变动重复次数的计量
          - Hz 并不是描述计算机领域所专有单位
          - 在 CPU 中使用高低电平表达 0 和 1，所以对于CPU的频率其实表达的就是高低电平在每秒钟变换的次数
          - 2GHz = 2*1000^3Hz = 每秒20亿次
    - 计算机的字符与编码集
      - 字符编码集的历史
        - ASCⅡ 码
          - 使用 7 个 bits 就可以完全表示 ASCII 码
          - 包含 95 个可打印字符
          - 33 个不可打印字符（包括控制字符）
          - 33 + 95 = 128 = 2^7
          - ![ASCII](images/ASCII码.png)
          - 很多应用或者国家中的符号都无法表示，比如数学符号÷ ≠≥≈
        - Extended ASCⅡ 码
          - ![ASCII](images/Extended&#32;ASCⅡ&#32;码.png)
          - 常见的数学运算符
          - 带音标的欧洲字符
          - 其他常用符、表格符等
        - 字符编码集的国际化
          - 欧洲、中亚、东亚、拉丁美洲国家的语言多样性
          - 语言体系不一样，不以有限字符组合的语言
          - 中国、韩国、日本等的语言最为复杂
      - 中文编码集
        - GB2312（1980年发明）：《信息交换用汉字编码字符集——基本集》
        - 一共收录了 7445 个字符
        - 包括 6763 个汉字和 682 个其他符号
        - 1995年，第二套完备的编码集，GBK：《汉字内码扩展规范》，向下兼容 GB2312，向上支持国际 ISO 标准
        - 收录了 21003 个汉字，支持全部中日韩汉字
        - Unicode（兼容全球的字符集）：统一码、万国码、单一码
        - Unicode 定义了世界通用的符号集，规定了符号的二进制代码，UTF-* 实现了编码
        - UTF-8 以字节为单位对 Unicode 进行编码
  - 组成篇
    - 计算机总线：连接计算机不同设备的数据线
      - 总线的概述
        - 是什么，有什么用：
          - USB（Universal Serial Bus 通用串行总线）
          - 提供了对外连接的接口
          - 不同设备可以通过USB 接口进行连接
          - 连接的标准，促使外围设备接口的统一
          - USB、PCI总线、ISA总线、Thunderbolt总线（苹果电脑的）
        - 总线的分类
          - 片内总线（高集成度芯片内部的信息传输线）
            - 芯片内部的总线
            - 寄存器与寄存器之间
            - 寄存器与控制器、运算器之间
          - 系统总线（CPU、主内存、IO设备、各组件之间的信息传输线）
            - 数据总线，总线的位数一般与 CPU 位数相同（32位、64位）
              - 双向传输各个部件的数据信息
              - 数据总线的位数（总线宽度）是数据总线的重要参数
            - 地址总线，用于传输数据的地址，用于数据的寻址，地址总线位数=n，寻址范围：0~2^n
              - 指定源数据或目的数据在内存中的地址
              - 地址总线的位数与存储单元的位数有关
            - 控制总线
              - 用来发出各种控制信号的传输线
              - 控制信号经由控制总线从一个组件发给另一个组件  
              - 控制总线可以监视不同组件之间的状态（就绪/未就绪）
      - 总线的仲裁
        - 为什么需要总线仲裁？为了解决总线使用权的冲突问题
        - 总线仲裁的方法
          - 链式查询
            - 好处：电路复杂度低，仲裁方式简单
            - 坏处：优先级低的设备难以获得总线使用权
            - 坏处：对电路故障敏感（串联电路通病）
          - 计时器定时查询
            - 仲裁控制器对设备编号，并使用计数器累计计数
            - 接收到仲裁信号后，往所有设备发出计数值
            - 计数值与设备编号一致则获得总线使用权
          - 独立请求
            - 每个设备均有总线独立连接仲裁器
            - 设备可单独向仲裁器发送请求和接受请求
            - 当同时收到多个请求信号，仲裁器有权按优先级分配使用权
            - 好处：响应速度快，优先顺序可动态改变
            - 坏处：设备连线多，总线控制复杂
    - I/O 设备
      - 常见的输入输出设备
        - 字符输入设备
          - 键盘
            - 薄膜键盘
            - 机械键盘，根据段落感、声音、压力、键程可分为：黑轴、红轴、青轴（敲击带感）、茶轴
        - 图形输入设备：鼠标、数位板（输入板和压感笔）、扫描仪（将图形信息转换为数字信号）
        - 图形输出设备：显示器（CRT显示器、液晶显示器）、打印机、投影仪
      - 输入输出接口的通用设计
        - 数据线
          - 是 I/O 设备与主机之间进行数据交换的传送线
          - 单向传输
          - 双向传输数据线
        - 状态线
          - IO 设备状态向主机报告的信号线
          - 查询设备是否已经正常连接并就绪
          - 查询设备是否已经被占用
        - 命令线
          - CPU 向设备发送命令的信号线
          - 发送读写信号
          - 发送启动停止信号
        - 设备选择线
          - 主机选择 I/O 设备进行操作的信号线
          - 对连在总线上的设备进行选择
      - CPU 与 IO 设备的通信
        - 程序中断：提供低速设备通知 CPU 的一种异步的方式，CPU 可以高速运转的同时兼顾低速设备的响应
          - 当外围 I/O 设备就绪时，向 CPU 发出中断信号
          - CPU 有专门的电路响应中断信号
        - DMA（直接存储器访问），当主存与 IO 设备交换信息时，不需要中断 CPU，可以提高CPU效率
          - DMA 直接连接主存与 IO 设备
          - DMA 工作时不需要 CPU 参与
          - 硬盘、外置显卡里都有 DMA 设备
    - 存储器
      - 存储器的分类
        - 按存储介质分类可分为：
          - 半导体存储器：存储的元器件是由半导体元器件组成的，例如：内存、U 盘、固态硬盘
          - 磁存储器：金属或者塑料表面涂抹一层磁性材料作为存储介质的存储器，例如：磁带、磁盘
        - 按存取方式分类：
          - 随机存储器（RAM），任何单元都能随机读取、与位置无关
          - 串行存储器，存取的时候与位置有关，按顺序查找
          - 只读存储器（ROM），例如 BIOS、手机固件都是存储在 ROM 里面
      - 存储器的层次结构，平时考虑存储器会考虑什么？读写速度（5400转、7200转）、存储容量、价格。容量+价格=>位价：每比特位价格，用于表达存储器的性价比
        - 缓存：指 CPU 里的寄存器或者高速缓存
        - 主存：计算机里的内存
        - 辅存：计算机里的外部存储设备，比如：磁盘、U盘、移动硬盘
        - ![存储器的层级结构](images/存储器的层级结构.png)
        - 「缓存-主存层级」
          - 原理：局部性原理，指的是 CPU 访问存储器时，无论是**存取指令**还是**存取数据**，所访问的存储单元都**趋于聚集在一个较小的连续区域中**
          - 实现：在 CPU 与主存之间增加一层速度快（容量小）的 Cache
          - 目的：解决主存速度不足的问题
        - 「主存-辅存层次」
          - 原理：局部性原理
          - 实现：主存之外增加辅助存储器（磁盘、SD 卡、U盘等）
          - 目的：解决主存容量不足的问题
    - 计算机的主存储器与辅助存储器，「为什么计算机断电，内存数据会丢失？」、「为什么计算机断电，磁盘数据不会丢失？」
      - 主存储器——内存
        - RAM（随机存取存储器：Random Access Memory）
        - RAM 通过**电容**存储数据，必须隔一段时间刷新一次
        - 如果断电，那么一段时间后将丢失所有数据
        - ![主存储器](images/主存储器.png)
        - 32位系统最多支持 2^32 = 4 * 2^30 = 4GB
        - 32位系统最多支持 2^64 = 2^34 * 2^30 = 2^34GB
      - 辅助存储器——磁盘
        - ![辅助存储器](images/辅助存储器.png)
        - 表面是可磁化的硬磁特性材料
        - 移动磁头径向运动读取磁道信息
        - 先来先服务算法：按顺序访问进程的磁道读写需求
        - 最短寻道时间优先：调度的顺序与磁头当前位置有关，优先访问离磁头最近的磁道
        - 扫描算法（电梯算法）：磁头每次只往一个方向移动，到达一个方向需要服务的尽头再反方向移动
        - 循环扫描算法：只往一个方向读取
      - 计算机的高速缓存
        - 高速缓存的工作原理
          - 字：是指存放在一个存储单元中的二进制代码组合
          - 字块：存储在连续的存储单元中而被看作是一个单元的一组字
          - 命中率是衡量缓存的重要性能指标
          - 理论上 CPU 每次都能从高速缓存取数据的时候，命中率为1
        - 高速缓存的替换策略
          - ![高速缓存替换时机](images/高速缓存替换时机.png)
          - 随机算法
          - 先进先出算法（FIFO）
          - 最不经常使用算法（LFU），优先淘汰最不经常使用的字块，需要额外的空间记录字块的使用频率
          - 最近最少使用算法（LRU），优先淘汰一段时间内没有使用的字块，一般使用双向链表，把当前访问节点置于链表前面（保证链表头部节点是最近使用的）
    - 指令系统
      - 机器指令的形式
        - 主要由两部分组成：操作码、地址码
        - 操作码指明指令所要完成的操作
        - 操作码的位数反映了机器的操作种类
        - 地址码直接给出操作数或者操作数的地址
        - 分三地址指令、二地址指令和一地址指令
        - 零地址指令：在机器指令中无地址码，空操作、停机操作、中断返回操作等
      - 机器指令的操作类型
        - 数据传输
          - 寄存器之间、寄存器与存储单元、存储单元之间传送
          - 数据读写、交换地址数据、清零置一等操作
        - 算术逻辑操作
          - 操作数之间的加减乘除运算
          - 操作数的与或非等逻辑运算
        - 移位操作
          - 数据左移（乘2）、数据右移（除2）
          - 完成数据在算术逻辑单元的必要操作
        - 控制指令
          - 等待指令、停机指令、空操作指令、中断指令等
      - 机器指令的寻址方式
        - 指令寻址：顺序寻址、跳跃寻址
        - 数据寻址：
          - 立即寻址：指令直接获得操作数，无需访问存储器
          - 直接寻址：直接给出操作数在主存的地址，寻找操作数简单，无需计算数据地址
          - 间接寻址：指令地址码给出的是操作数地址的地址，需要访问一次或多次主存来获取操作数
    - 计算机的控制器：协调和控制计算机运行的
      - ![控制器](images/控制器.png)
      - 程序计数器：用来存储吓一跳指令的地址，循环从程序计数器拿出指令，当指令被拿出时，指向下一条指令
      - 时序发生器：电气工程领域，用于发送时序脉冲，CPU 根据不同的时序脉冲有节奏的进行工作
      - 指令译码器：是控制器的主要部件之一，计算机指令由操作码和地址码组成，翻译操作码对应的操作以及控制传输地址码对应的数据
      - 指令寄存器：指令寄存器也是控制器的主要部件之一，从主存或高速缓存存取计算机指令
      - 主存地址寄存器：保存当前 CPU 正要访问的内存单元地址
      - 主存数据寄存器：保存当前 CPU 正要读或写的主存数据
      - 通用寄存器：用于暂时存放或传送数据或指令，可保存 ALU 的运算中间结果，容量比一般专用寄存器要大
    - 计算机的运算器：是用来进行数据运算加工
      - ![运算器](./images/运算器.png)
      - 数据缓冲器
        - 分为输入缓冲和输出缓冲
        - 输入缓冲暂时存放外设送过来的数据
        - 输出缓冲暂时存放送往外设的数据
      - ALU：算术逻辑单元，是运算器的主要组成
        - 可以完成常见的位运算（左右移、与或非等）
        - 算术运算（加减乘除等）
      - 状态字寄存器
        - 存放运算状态（条件码、进位、溢出、结果正负等）
        - 存放运算控制信息（调试跟踪标记位、允许中断位等）
      - 通用寄存器
        - 用于暂时存放或传送数据或指令
        - 可保存 ALU 的运算中间结果
        - 容量比一般专用寄存器要大
    - 计算机指令的执行过程
      - 指令执行过程（取指令→分析指令→执行指令）
      - CPU 的流水线设计
        - 类似工厂的装配线
        - 工厂的装配线使得多个产品可以同时被加工
        - 在同一时刻，不同产品均位于不同的加工阶段
  - 计算篇
    - 进制运算的基本知识
      - 进制运算的基础
        - 进制的概述
          - 进位制是一种记数方式，亦称进位计数法或位值计数法
          - 有限种数字符号来表示无限的数值
          - 使用的数字符号的数目称为这种进位制的基数或底数
          - 八进制
          - 十六进制：[0-9]和A、B、C、D、E、F
          - 二十进制：玛雅文明的玛雅数字，因努伊特的因努伊特数字
          - 六十进制：时间、坐标、角度等量化数据
          - 二进制
        - 二进制运算的基础
    - 二进制数据的表示方法
      - 有符号数与无符号数
        - 使用 0 表示正数，1 表示负数
        - 规定符号位位于数值第一位
        - 原码表示法的缺点：
          - 有两种表示方法：00、01
          - 原码进行运算非常复杂，特别是两个操作数符号不同的时候
          - 判断两个操作数绝对值大小
          - 使用绝对值大的数减去绝对值小的数
          - 对于符号值，以绝对值大的为准
          - 希望找到不同符号操作数更加简单的运算方法
          - 希望找到使用正数代替负数的方法
          - 使用加法操作代替减法操作，从而消除减法
      - 二进制的补码表示法
        - ![补码计算](images/补码计算.png)
      - 二进制的反码表示法
        - ![反码](images/反码.png)
        - 负数的反码等于原码除符号位外按位取反
        - 负数的补码等于反码+1
        - ![反码2](images/反码2.png)
      - 小数的二进制补码表示法
        - ![二进制小数补码](images/二进制小数补码.png)
    - 二进制数据的运算
      - 定点数与浮点数
        - 定点数的表示方法
          - 小数点固定在某个位置的数
        - 浮点数的表示方法
          - 计算机处理的很大程度上不是纯小数或纯整数
          - 数据范围很大，定点数难以表达
          - 浮点数的表示格式
            - ![浮点数](images/浮点数.png)
          - 浮点数的表示范围
            - ![浮点数表示范围](images/浮点数表示范围.png)
            - ![浮点数表示范围2](images/浮点数表示范围2.png)
            - 单精度浮点数：使用 4 字节、32位来表达浮点数（float）
            - 双精度浮点数：使用 8 字节、64位来表达浮点数（double）
          - 浮点数的规格化
        - 定点数与浮点数的对比
          - 当定点数与浮点数位数相同时，浮点数表示的范围更大
          - 当浮点数尾数为规格化数时，浮点数的精度更高
          - 浮点数运算包含阶码和尾数，浮点数的运算更为复杂
          - 浮点数在数的表示范围、精度、溢出处理、编程等方面均优于定点数
          - 浮点数在数的运算规则、运算速度、硬件成本方面不如定点数
      - 定点数的加减法运算
        - 整数加法：`A[补]+B[补]=[A+B][补](mod2^n+1)`
        - 小数加法：`A[补]+B[补]=[A+B][补](mod2)`
        - 数值位与符号位一同运算，并将符号位产生的进位自然丢掉
        - 判断溢出
          - 双符号位判断法
            - 单符号位表示变成双符号位：0=>00,1=>11
            - 双符号位产生的进位丢弃
            - 结果的双符号位不同则表示溢出
        - 整数减法：`A[补]-B[补]=[A+(-B)][补](mod2^n+1)`
        - 小数减法：`A[补]-B[补]=[A+(-B)][补](mod2)`
        - `-B[补]`等于`B[补]`连同符号位按位取反，末位加一
      - 浮点数的加减法运算
        - ![浮点数加减法整个过程](images/浮点数加减法整个过程.png)
        - ![浮点数加减法](images/浮点数加减法.png)
        - 对阶的目的是使得两个浮点数阶码一致，使得尾数可以进行运算
        - 浮点数尾数运算简单，浮点数位数实际小数位与阶码有关，阶码按小阶看齐大阶的原则
        - 尾数求和：使用补码进行运算，减法运算转化为加法运算：`A-B=A+(-B)`
        - ![尾数规格化](images/尾数规格化.png)
        - ![尾数规格化2](images/尾数规格化2.png)
        - 舍入
        - 溢出判断
          - 定点运算双符号位不一致为溢出
          - 浮点运算尾数双符号位不一致不算溢出
          - 因为尾数双符号位可以进行右规
          - 浮点运算主要通过阶码的双符号位判断是否溢出
          - 如果尾数的规格化后，阶码双符号位不一致，则认为是浮点数的溢出
      - 浮点数的乘除法运算
        - ![浮点数乘法](images/浮点数乘法.png)
        - ![浮点数除法](images/浮点数除法.png)
  - 综合实践
    - 双向链表
      - 可以快速找到一个节点的上一个节点
      - 可以快速去掉链表中的某一个节点
      - ![双向链表](images/双向链表.png)
    - FIFO
    - LFU
    - LRU
- 操作系统
  - 基础篇
    - 进程管理
    - 存储管理
    - 文件管理
    - 作业管理
    - Linux 系统
  - 提升篇
    - 线程同步
    - 进程同步
    - 线程、协程
    - 用户态与内核态
    - 上下文切换
  - 综合实践
    - 线程安全
    - 线程池
    - 同步任务
    - 异步任务
- 计算机网络
  - 概述篇
    - 七层模型
    - 四层协议
    - 物理层
    - 数据链路层
    - 底层协议
  - 网络层篇
    - IP 协议
    - ICMP 协议
    - 子网划分
    - 路由算法
    - IPv6
  - 传输层篇
    - TCP 协议
    - UDP 协议
    - 超时重传机制
    - 拥塞避免算法
    - 心跳保活机制
  - 应用层篇
    - HTTP 协议
    - URL 资源
    - HTTP 结构
    - HTTPS 安全
    - HTTP 服务
  - 综合实践
    - 使用线程池
    - IP 报文
    - ICMP 报文
    - TCP 报文
    - UDP 报文

## 环境说明

- Linux 环境：VMWare WorkStation + Linux 虚拟机
- 编程语言：C++、Python

4-2
