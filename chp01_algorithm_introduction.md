## 第1章 算法简介
<br/>


### 算法
<br/>
算法广义上定义为解决问题的流程和步骤，狭义上定义为**完成任务的有穷指令序列**，计算机专业中专指后者。
具有下列五个特性：

- **确定性**：每一条指令在计算机执行时是明确的，无异议；

- **可行性**：每一条指令能被计算机执行；

- **输入**：有0，1，2或多个输入；

- **输出**：至少有1个输出；

- **有穷性**：每一条指令执行的次数是有穷的。
<br/>


### 计算机相关概念
<br/>

**计算过程**不满足有穷性，可以永远执行下去。例如：死循环（所有正整数求和），**操作系统**。
<br/>

**编程**是算法的实现过程。
算法基于**数据结构**实现，**程序**是算法的实现结果，在面向过程中，程序=算法+数据结构。
**进程**是程序的运行状态，程序是静态的，进程是动态的。
<br/>
**软件**包括程序，数据和文档。
**硬件**指物理设备。
<br/>


### 算法性能
<br/>
算法性能体现在**运行效率**(时间)和**存储效率**（空间）。随着存储硬件价格的降低，人们更加关注**算法的运行效率**。
使用**计算量函数**细致地衡量算法的性能，使用**渐进复杂度**粗略地衡量算法的性能。
更关注算法的**平均运行情况**和**最坏运行情况**。
<br/>

#### 计算量函数
<br/>
用**问题规模**表示**算法基本运算量**的**函数**。时间复杂度用**T(n)**(或**T(n,m)**等)来表示。
$$
\begin{array}{l}
{T(n)=5 n} 
\\ {T(n)=7 \log n} 
\\ {T(n)=3 n \log n} 
\\ {T(n)=4 n^{3}}
\\ {T(n)=2^{n}} 
\\ {T(n, m)=2(n+m)}
\end{array}
$$
![时间复杂度比较](https://raw.githubusercontent.com/JerryQiang/algorithm/master/res/imgs/chp01_algorithm_introduction/function_complexity_comparation.png)
<br/>




#### 最坏时间复杂度
<br/>
渐近时间复杂性，表示算法时间复杂度的上界，用${\mathrm{T}(\mathrm{n})=\mathrm{O}(\mathrm{f}(\mathrm{n}))} $符号表示。
$$
\begin{array}{l}
\\ \exist \ c>0, n_{0} \in N^+
\\ \text{使得}n \geq n_{0}时，\text{总有}T(n) \leq c * f(n)
\\ \therefore {\mathrm{T}(\mathrm{n})=\mathrm{O}(\mathrm{f}(\mathrm{n}))} 
\end{array}
$$
<br/>


#### 最好时间复杂度
<br/>
渐近时间复杂性，表示算法时间复杂度的下界，用$\Omega(\mathrm{f}(\mathrm{n}))$符号表示。
$$
\begin{array}{l}
\\ \exist \ c>0, n_{0} \in N^+
\\ \text{使得}n \geq n_{0}时，\text{总有}T(n) \geq c * f(n)
\\ \therefore {\mathrm{T}(\mathrm{n})=\Omega(\mathrm{f}(\mathrm{n}))} 
\end{array}
$$
<br/>




#### 平均时间复杂度
<br/>
渐近时间复杂性，表示算法时间复杂度的上界和下界，用${\Theta}(\mathrm{f}(\mathrm{n}))$符号表示。
$$
\begin{array}{l}
\\ \exist \ c_{1}>0,\ c_{2}>0, n_{0} \in N^+
\\ \text{使得}n \geq n_{0}时，\text{总有}T(n) \leq c_{1} * f(n)，T(n) \geq c_{2} * f(n)
\\ {\mathrm{T}(\mathrm{n})=\mathrm{\Theta}(\mathrm{f}(\mathrm{n}))}
\end{array}
$$
<br/>

![时间复杂度记号图例](https://raw.githubusercontent.com/JerryQiang/algorithm/master/res/imgs/chp01_algorithm_introduction/function_complexity_mark.png)