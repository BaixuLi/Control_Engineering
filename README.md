# Control_Engineering
## Process control
* 控制系统中的三个基本操作：测量、决策、执行。
* 控制系统的设计目标：对于任意的外部干扰（DV），通过调节操作变量（MV）以使被控变量（CV）维持在设定值。
* 过程控制四大参数：温度、压力、流量、液位/料位。
* 被控过程增益三部分：符号、数值与单位。

## Electrical control
* 380V是线电压，转换成相电压要除以根号3(Y型连接)
* 交流电动机与直流电动机工作原理大致相似，都是基于电磁感应原理。
* 同步电机历来是以转速与**电源频率**保持严格同步著称的。
* 同步电动机变频调速的电压频率特性与异步电动机变频调速相同，最好是保持**每极磁通量**为额定值不变
* 同步电机没有像异步电机那样的多种调速方法。在同步电机的变压变频调速方法中，从频率控制的方式来看可分为他控变频调速和自控变频调的方式来看，可分为**他控变频调速**和**自控变频调速**两类。 
* 他控变频同步电动机调速系统变频器的**输出频率**与**转子转速或位置**无直接的关系；控制系统**结构简单**，可以同时实现多台同步电机调速。若控制不当，仍然会造成**失步**。
* 从电机本身看，自控变频同步电机是一台同步电机，可以是永磁式的，容量大时也可以用励磁式的。把电机和逆变器、转子位置检测器BQ合起来看，如同是一台直流电机。从外部看来，改变**直流电压**，就可实现调速，相当于直流电机的调压调速。
* **电力电子逆变器**和**转子位置检测器**就相当于电子式换向器。
* 无刷直流电机实质上是一种特定类型的永磁同步电机，转子磁极采用瓦形磁钢经转子磁极采用瓦形磁钢，经专门的磁路设计，可获得梯形波的**气隙磁场**，**感应电动势**也是梯形波的。 
* 无刷直流电机控制思想: 根据**转子位置**控根据转子位置控制定子电流**相位**和**幅值**
* PWM逆变器输出电压为**调制方波**序列，并按直流PWM的方法对方波进行调制，同时完成**变压变频**功能。 
* **直流励磁**与**电枢反应**合成起来产生气隙磁链
* 只要保证**气隙磁链**恒定，控制定子电流的转矩分量就可以方便灵活地控制同步电机的电磁转矩
* 正弦波永磁同步电动机具有定子三相分布绕组和永磁转子，在磁路结构和绕组分布上保证定、转子绕组中的感应电动势具有正弦波形，外施的定子电压和电流也应为**正弦波**。
* 永磁同步电机可以与一般的电励磁同步电机等效，唯一的差别是虚拟励磁电流恒定唯一的差别是**虚拟励磁电流**恒定。 
* 当负载增加时，**定子电流**增大，使定子磁链和反电动势加大，迫使定子电压升高。**定子电压矢量**和**电流矢量**的夹角也会增大，造成**功率因数**降低

