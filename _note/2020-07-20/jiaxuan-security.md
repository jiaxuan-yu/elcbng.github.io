| layout | title    | author     | data   |
| ------ | -------- | ---------- | ------ |
| note   | security | jiaxuan.yu | 2020.8 |

[TOC]

﻿﻿﻿﻿﻿﻿﻿﻿[网络安全](https://baike.baidu.com/item/%E7%BD%91%E7%BB%9C%E5%AE%89%E5%85%A8)

### 网络安全：

网络系统的**硬件**、**软件**及其系统中的**数据**受到保护，不因偶然的或恶意的原因而遭到破坏、更改、泄漏，系统连续可靠正常地运行，**网络服务**不中断。

##信息安全：
包括信息的**保密性**、**真实性**和**完整性**

### 安全隐患：

1.Internet开放、无控制结构，hacker入侵系统，窃取破坏数据，盗用特权

2.数据传输局域TCP/IP通信协议进行，缺乏安全措施

3.通信业务多用Unix，存在安全脆弱性

4.应用层无有力协议

5.电子邮件存在被拆看、误投和伪造的可能性

6.计算机病毒可通过公共匿名FTP文件传送、也可以通过邮件和邮件的附加文件传播

**攻击形式**：
**中断**以*可用性*作为攻击目标，毁坏系统资源，使网络不可用

**截获**以*保密性*作为攻击目标，非授权用户通过某种手段获得对系统资源的访问

**修改**以*完整性*作为攻击目标，非授权用户不仅获得访问而且对数据进行修改

**伪造**以*完整性*作为攻击目标，非授权用户将伪造的数据插入正常传输的数据中

### 解决方案：

1.入侵检测系统部署

2.漏洞扫描系统

3.网络版杀毒产品部署

##网安措施：
包括网络安全、保护应用服务安全和保护系统安全，考虑安全防护的物理安全、防火墙、信息安全、web安全、媒体安全等

### 加密技术：

[对称密码体制和非对称密码体制](https://www.cnblogs.com/Leo_wl/p/10714011.html)

加密技术是*电子商务*采取的基本安全措施，交易双方可根据需要在*信息交换*的阶段使用分为**对称加密**和**非对称加密**

**对称加密**：

又称*私钥加密*

>特点：接发双方用同一密钥去加密和解密数据

>优势：速度快，计算少，效率高

>缺点：安全性没保证，密钥管理负担大，成本高，加密和认证缺乏签名功能

>工作方式：*分组加密*、*序列加密*

>加密算法：DES、3DES、AES

**非对称加密**：

>特点：A（生成2把密钥，其一为公钥）----(公钥）--->B(加密信息）-------->A（私钥解密）

>优势：安全性高

> 缺点：耗时长，速度慢，只适合少量数据加密

>加密算法：RSA、Elgamal、背包算法、Rabin、D-H、ECC（椭圆曲线加密算法）

**分组加密**的四种工作模式：**ECB**、**CBC**、**CFC**、**OFB**
___
___

### HTTP与HTTPS

[HTTP与HTTPS](https://blog.csdn.net/xiaoming100001/article/details/81109617)

**HTTP**：是互联网上应用最为广泛的一种网络协议，是一个客户端和服务器端请求和应答的标准（TCP），用于从WWW服务器传输超文本到本地浏览器的传输协议，它可以使浏览器更加高效，使网络传输减少。
>特点：**无状态**、**无连接**、**基于请求和响应**、**简单快速、灵活**、通信使用明文、请求和响应不会对通信方进行确认、**无法保护数据的完整性**

>优势：高效、成本较低


**HTTPS**：是以安全为目标的HTTP通道，简单讲是HTTP的安全版，即HTTP下加入SSL层，HTTPS的安全基础是SSL，因此加密的详细内容就需要SSL。
>特点：**内容加密**、**验证身份**、**保护数据完整性**

>优势：较安全

>缺点：SSL证书需购买申请，需绑定IP，耗电加载时间长，成本高

---

---

### VT

Virtualization Technology (虚拟化)

**优点**：

- 整合资源：
  - 背景：数据爆炸式增长；云计算技术不断普及；目前各大企业对计算机硬件资源的利用率不足20%，资源浪费严重；
  - 方法：服务器虚拟化技术在原应用保持不变基础上，集中在某一计算机服务器中，提升资源利用率，降低各项硬件投入，节约成本。
- 低能耗：
  - 背景：信息时代，云计算技术备受推广；
  - 方法：虚拟化技术可模拟出不同场景，实现对计算机系统中各种硬件及软件的全面系统检查，发现问题立即出现在界面上，提醒相关人员及时处理，从而达到降低能耗，绿色发展的目的。
- 降低运营成本：
  - 背景：服务商不断运营转型，集约化对成本控制提出更高要求，投资精细化，企业实现IT化运行的关键在于集中对数据中心的投资（1.计算机硬件和许可服务支持的投资；2.计算机系统运维的成本投资，通过计算机服务器虚拟化技术能充分发挥服务器的性能）；
- 应用更加平坦化：数据中心平台逐年增加，计算机服务器应用愈加复杂，不同平台在具体运行过程中，需要充分考虑不同操作系统和中间件的层面问题。服务器虚拟化能有效解决此类问题，将应用和硬件平台相互隔离，实现了跨平台。

**特性**：

- 分区：
  - 可以在一台物理机上运行多个操作系统；
  - 可以在虚拟机之间分配资源；
- 隔离：
  - 可以在硬件级别进行故障和安全隔离；
  - 可以利用高级资源控制功能保持性能
- 封装：
  - 可以将虚拟机的完整状态保存到文件中；
  - 移动和复制虚拟机就像移动和复制文件一样轻松；
- 独立于硬件：
  - 可以将任意虚拟机调配或迁移到任意物理服务器上。

**类型**：

- 服务器虚拟化：支持将多个操作系统作为高效的虚拟机在单个物理服务器上运行。

  优势：

  - 提高IT效率；
  - 降低运维成本；
  - 更快地部署工作负载；
  - 提高应用性能；
  - 提高服务器可用性；
  - 消除服务器数量剧增情况和复杂性；

- 网络虚拟化：完全复制物理网络，提供逻辑网络连接设备和服务，支持应用在虚拟网络上运行，并具有更大的运维优势，可实现虚拟化的所有硬件独立性。

- 桌面虚拟化：将桌面部署为代管服务，IT组织能更快地响应变化的工作场所需求和新出现的机会，将虚拟化桌面和应用快速、轻松交付给分支结构、外包和离岸员工以及移动员工。

---

#### Intel VT

Virtualization Technology (虚拟化)

[Intel VT]( [https://baike.baidu.com/item/Intel%20VT/2091588?fromtitle=%E8%99%9A%E6%8B%9F%E5%8C%96&fromid=547949](https://baike.baidu.com/item/Intel VT/2091588?fromtitle=虚拟化&fromid=547949) )

[VMM]( [https://baike.baidu.com/item/%E8%99%9A%E6%8B%9F%E6%9C%BA%E7%9B%91%E8%A7%86%E7%A8%8B%E5%BA%8F?fromtitle=VMM&fromid=7047240](https://baike.baidu.com/item/虚拟机监视程序?fromtitle=VMM&fromid=7047240) )

- 目的：解决纯软件虚拟化解决方案在可靠性、安全性和性能上的不足。

- 前身：2005年8月，针对硬件辅助虚拟化的Vanderpool技术；2005年11月，Intel将其改为VT。

- 方式：将一台计算机虚拟为多台逻辑计算机。

- 对象：服务器，Internet，桌面，存档空间。

- 技术：针对处理器、芯片组、网络的IntelVT-x、IntelVT-d和IntelVT-c技术。

  -  IntelVT-x：增强处理器的VT虚拟化技术。
    - 作用：
      1. 使得在一台物理服务器内可以同时运行多个操作系统；
      2. 能够降低（甚至消除）多个虚拟机操作系统之间的资源争夺和限制，从硬件上极大地      改善虚拟机的安全性和性能，有助于提高基于软件的虚拟化解决方案的灵活性与稳定性；
      3. 可以消除VMM（Virtual Machine Monitor虚拟机监视器）参与虚拟机“中断”请求的处理与特定指令的执行，这样VMM操作和控制虚拟机时，将更加快速、可靠和安全；
      4. 具备迁移特性，可为IT投资提供有力保护，并进一步提高故障切换、负载均衡、灾难恢复和维护的灵活性。
    - 包括：IntelVTFlexPriority 、IntelVTFlexMigration 、ExtendedPage Tables;
      1. IntelVTFlexPriorty(灵活优先级)：处理器执行任务时，收到其他设备或应用发出的请求或“中断”命令；处理器的一个寄存器专用来监控任务优先级，最大程度上减少对性能的影响。
      2. IntelVTFlexMigration(灵活迁移)：虚拟机在无需停机的情况下，将运行中的虚拟机在物理服务器之间迁移；**注意**：在不同产商、不同型号的处理器之间迁移，可能由于指令集不同而出现故障或问题。
      3. ExtendedPage Table(扩展页表)：为了降低实现内存虚拟化的难度和提升内存虚拟化的性能，ExtendedPage Tables直接在硬件上支持内存虚拟机内存的逻辑地址->虚拟机内存的物理地址->物理服务器内存的物理地址的两次转换。
    - 产品： Pentium、Celeron、Corei3、Corei5、Corei7、Core2Duo、CoreSolo、Core2Extreme、Core2Quad、Xeon、Quark、Atom、Itanium。

  - IntelVT-d：支持直接I/O访问的IntelVT虚拟技术。

    - 作用：
      1. 通过VMM将特定I/O设备安全分配给特定虚拟机来实现，减少VMM参与管理I/O流量的工作；
      2. 每个I/O设备在系统内存中都有一个专用区域，只有该I/O设备及分配到该设备的虚拟机才能对内存区进行访问；加速数据传输，消除大部分的性能开销；
      3. VMM分配后，数据直接在虚拟机与其分配的I/O设备之间进行传输；加快了I/O的流动。减少VMM活动及服务器处理器的负载；
      4. 由于特定设备或虚拟机的I/O数据内存区不能被其他硬件或虚拟机访问，系统的安全性和可用性也得到了增强。

  - IntelVT-c：支持网络连接的Intel虚拟化技术。

    - 作用：

      1. 用户对虚拟化I/O设备的要求在显著提高，通过将广泛的硬件辅助特性集成到I/O设备（该设备用于保持服务器与数据中心网络、存储基础设施及其它外部设备的连接）中，IntelVT-c可针对虚拟化进一步优化网络；
      2. 大幅提高交付速度，减少VMM与服务器处理器的负载。

    - 包括：VMDq(虚拟机设备队列)、VMDc(虚拟机直接互连)。

      1. VMDq（虚拟机设备队列）：最大限度提高I/O吞吐率。

         > 传统服务器虚拟：VMM必须对每个单独的数据包进行分类，并将其发送到相应的虚拟机，占用大量的处理器周期；

         > - VMDq：专用硬件执行分类功能，VMM只负责将预分类的数据包组发送到相应的虚拟机，降低I/O延迟，使处理器获得更多的可用周期来处理业务应用。使虚拟机应用达到接近物理服务器的吞吐率。

      2. VMDc（虚拟机直接互连）：大幅提升虚拟化性能。

         > VMDc支持虚拟机直接访问网络I/O硬件，绕过了VMM交换机，提升I/O性能，减少服务器处理器的负载，提升虚拟机性能。

---

---

### 服务器

[服务器]( [https://baike.baidu.com/item/%E6%9C%8D%E5%8A%A1%E5%99%A8/100571](https://baike.baidu.com/item/服务器/100571) )

- 服务器是计算机的一种，比普通计算机运行更快、负载更高、价格更贵；在网络中为其它客户机提供计算或者应用服务。

- 特性：

  1. 具有高速的CPU运算能力、长时间的可靠运行、强大的I/O外部数据吞吐能力及更好的扩展性；

  2. 具备响应服务请求、承担服务、保障服务的能力；

  3. RASUM衡量标准。

     > - 可靠性（Reliability）:所选服务器能满足长期稳定工作的要求，不能经常出问题；
     >
     > - 可用性（Availability）:通常要求服务器永不中断，持续为用户提供连接服务，直到报废。要求各配件质量过关，采取必要的技术和配置措施（如硬件冗余、在线诊断等）；
     >
     >   > - 硬件冗余：电脑执行底层是101010的机器码，在实际运行中难免因为电子偏移而导致无法执行的片段，这些错误片段堆积在内存里，多了的化系统就会死机或重启，所以专业的服务器、图形工作站等都会配置检验内存，校验内存会自动调整出错的地方（比如把1变成0，把0变成1）；
     >   > - 软件冗余：一个小小的异常导致程序进入一种死循环的状态；系统已经无法去对这种状态有任何动作了，所以操作底层的线层会报出问题并用更高级的权限去强行关闭它。
     >
     > - 可扩展性（Scalability）:
     >
     >   > - 原因：信息时代变化快，要保持前期投资能未后期充分利用；
     >   > - 要求：通常要求服务器上具备一定的可扩展空间和冗余件（如磁盘阵列架位、PCI和内存条插槽位等）；
     >   > - 体现：硬盘扩扩充，CPU可升级，系统支持多种可选主流操作系统等。
     >
     > - 易使用性（Usability）:
     >
     >   > - 原因：服务器相对PC机来说复杂许多，特别是其软件系统配置；软件系统一多，可能造成服务器使用性能下降，管理人员无法有效操纵；
     >   > - 体现：服务器易操作，用户导航系统完善，机箱设计人性化，有关键恢复功能，有操作系统备份，有足够的培训支持等。
     >
     > - 易管理性（Manageability）:
     >
     >   > - 原因：服务器可能出故障；
     >   > - 要求：有必要的避免出错的措施，以及时发现问题，出故障能及时得到维护；
     >   > - 目的：减少出错机会，大大提高服务器维护的效率；管理人员轻松管理，高效工作；
     >   > - 体现：有智能管理系统，有自动报警功能，有独立于系统的管理系统，有液晶监视器等。

- 结构：CPU，硬盘，内存，系统，系统总线等。

- 分类：

  > - 体系结构：
  >
  >   > - IA架构服务器：采用CISC体系结构，即复杂指令集体系结构
  >   >   1. 特点是指令较长，指令的功能较强，单个指令可执行的功能较多；
  >   >   2. 可以通过增加运算单元，使一个指令所执行的功能能够同时并行执行，从而提高运算能力。
  >   >   3. 采用开放体系结构
  >   > - RISC架构服务器：采用精简指令集CPU
  >   >   1. 特点是采用定长指令，使用流水线执行指令；
  >   >   2. 处理器设置不同处理单元执行指令的不同阶段；
  >   >   3. 优点是使CPU有并行处理指令的能力，使处理器在单位时间内处理更多的指令。
  >
  > - 规模不同：（较老的分类方法）工作组服务器、部门服务器、企业服务器。
  >
  > - 功能不同：
  >
  >   > - 文件/打印服务器：最早的服务器种类，可以执行文件存储和打印机资源共享的服务；
  >   > - 数据库服务器：广泛应用在商业系统中，运行一个数据库系统，用于存储和操纵数据，向连网用户提供数据查询、修改服务；
  >   > - WEB服务器：完成主页的存储和传送；
  >   > - E-MAIL服务器：电子邮件服务；
  >   > - NEWS服务器：新闻组服务；
  >   > - PROXY服务器；

- 外形：机构式，刀式，塔式，机柜式。
- 安全问题：
  1. 服务器所处运行环境（主要包括运行温度和空气湿度）；
  2. 正确的网络服务器安全维护意识（有效的安全维护措施，正确的防火墙软件）；
  3. 服务器系统漏洞过多：计算机网络本身具有开放自由的特性，对系统安全造成威胁；某些不法人员可能借助系统漏洞对缓存区进行信息查找，然后攻击计算机系统，造成信息泄露风险，计算机运行系统也会遭到破坏。
- 维护保养：        
  1. 注重机房环境的建设：（首要环节），保证充足的空间，机房隔断，防火防静电；控制机房温度湿度，完善电子检测系统；
  2. 做好硬件维护工作：扩容？拆卸和更新服务器设备是务必让设备处于断电状态并进行接地处理；定期除尘；电源系统保护；
  3. 维护好服务器软件：巡检，补丁？扩展，备份；
  4. 电力的控制与保障；
  5. 密码管理：密码的管理与更换，密码专业性；在日常检查中，做好统计，关闭一些不太使用的端口。

---

---



