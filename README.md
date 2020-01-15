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
* 基频以下采用**带定子压降补偿的恒压频比**控制方式，基频以上采用电压恒定的控制方式
* 励磁绕组和电枢绕组相互独立，忽略电枢反应或通过补偿绕组抵消电枢反应，励磁和电枢各自产生磁动势空间相差**90度**，无交叉耦合，通过**励磁电流**控制磁通，通过**电枢电流**控制**电磁转矩**。
* 沿励磁磁极的轴线为d轴，与d轴正交的是q轴，d坐标系固定在转子上，与转子同步旋转。 
* 定子与转子之间的位置是变化的，互感是**角位移**的函数
* 三相绕组A、B、C和两相绕组之间的等效变换，称作三相坐标系和两相正交坐标系间的变换，简称3/2变换。变换原则：变换前后**磁动势**相等。
* 两相静止绕组，通以两相平衡交流电流，产生旋转磁动势。如果令两相绕组转起来，且旋转角速度等于**合成磁动势**的旋转角速度，则两相绕组通以直流电流就产生空 动势的旋转角速度，则两相绕组通以直流电流就产生空间旋转磁动势
* **转子励磁磁动势**和**定子电枢反应磁动势**转矩分量相互作用所产生的转矩，是同步电动机主要的电磁转矩
* 第二项是由凸极效应造成的磁阻变化在电枢反应磁动势作用下产生的转矩，称作反应转矩或磁阻转矩；第三项是电枢反应磁动势与阻尼绕组磁动势相互作用的转矩。
* 同步电机是非线性、强耦合的多变量系统，若考虑**阻尼绕组**的作用和**凸极效应**时，动态模型更为复杂
* **交-交变压变频器**虽然在结构上只有一个变换环节，省去了中间直流环节，看似简单，但所用的器件数量很多，控制复杂。
* **交-直-交变压变频器**主回路只有一套可控功率电路，具有结构简单、控制方便的优点；当电动机工作在回馈制动状态时能量不能回馈至电网，造成直流侧电压上升，称作**泵升电压**
* 采用**直流母线**供电给多台逆变器，可以减少整流装置的电力电子器件，逆变器从直流母线上汲取能量，还可以通过直流母线来实现能量平衡，提高整流装置的工作效率
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
