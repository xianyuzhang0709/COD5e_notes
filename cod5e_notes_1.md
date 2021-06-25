# Ch01-Computer Abstraction and Technology

测验1：

|            |                                     |   访问时间   |        价格         |    volatile易失性    |                  用于                  |
| :--------: | :---------------------------------: | :----------: | :-----------------: | :------------------: | :------------------------------------: |
|  主存储器  | DRAM（Dynamic Random Access Memory) |  快（50ns）  |    贵（$5~10/G）    |     易失性存储器     |    保持运行中的程序。集成电路形式。    |
| 二级存储器 |        闪存（flash memory）         | 中（5~50μs） |   中（$0.75~1/G）   | 非易失性半导体存储器 |  保存两次运行之间的程序和数据。PMDs。  |
|            |        磁盘（magnetic disk）        | 慢（5~20ms） | 便宜（$0.05~0.1/G） |    非易失性存储器    | 保存两次运行之间的程序和数据。服务器。 |

* cache——缓存，一种小而块的存储器，一般作为DRAM的缓冲，采用另一种存储技术（静态随机访问存储器，集成电路形式的存储器，比DRAM快，集成度更低），速度更快，不那么密集，价格比DRAM贵。cache一般作为大而慢的存储器的缓冲。

* 1s = 1000ms（毫秒）；1ms = 1000μs（微秒）；1μs = 1000ns（纳秒）；1ns = 1000ps（皮秒）。
* DRAM比闪存快100~1000倍，比磁盘快10w~40w倍。

### 1.6.3 CPU Performance and Its Factors

**CPU execution time** for a program = **CPU clock cycles** for a program x **CPU clock cycle time**

* 一个程序的**CPU执行时间** = **cycle次数** x **一次cycle的时间**

* **CPU clock cycle time** = 1/**clock rate**（时钟频率的倒数）
* CPU clock cycle time即时钟周期，即一次脉冲的时间，单位为秒。

### 1.6.4 Instruction Performance

**CPU clock cycles** = **Instructions** for a program x **Average clock cycles per instruction**

* 一个程序的**CPU clock cycles次数** = 这个程序的**指令数** x 平均每个指令有多少个cycle次数

* CPI，即平均每个指令有多少个cycles次数，单位为时钟周期数（cycles）。

### 1.6.5 The classic CPU Performance Equation

**CPU time** = **Instructions** x **CPI** x **clock cycle time**

* Instructions: 执行某程序所需的总指令数



