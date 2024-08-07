# STM简介

        扫描隧道显微镜（STM）是基于量子隧穿效应，利用隧穿电流特性工作的一种能够实现原子级分辨率成像的显微镜。

        通过将导电探针悬停在通电样品表面几纳米处进行栅格扫描，监测隧穿电流变化情况，扫描隧道显微镜能够实现样品表面形貌成像[1]。由于隧穿电流随距离指数性变化的特征，扫描隧道显微镜能够达到0.1nm的横向分辨率与0.01nm的垂直分辨率[2]。

# 量子隧穿效应

***推导仅供参考，若有错误，欢迎指正。**

***不想看推导部分的可直接看最后的结论。**

        在经典力学中，在一维情况下，总能量为E的电子在位置为x处的运动情况可以用以下公式表示：

$$
E=\frac{1}{2} m v^2+V(x)
$$

        其中，m为电子质量，v为电子速度，V(x)为与电子位置x处有关的势能。由式子(2.1)可知，只有当E>Ep时，电子才具有正值的速度。因此，若某一位置势能Ep1>E时，电子将不可能到达该位置。

        德布罗意在1924年提出电子如光的波粒二象性一样，具有波的性质，并且电子的波长λ可以通过公式(2.2)描述：

$$
E=\frac{h}{p}
$$

其中，h为普朗克常量，p为电子动量。

        可以将扫描隧道显微镜的势能模型简化为下图所示的一维形式，探针与样品间的间隙被描述为方势垒，其中红色横线为电子能量：

![98e9932244c229f4809f8dd125fce3ca.png](media/98e9932244c229f4809f8dd125fce3ca.png)

即势能可以通过公式描述为：V(x)=0(x<a, x>a), V(x)=V_1(a<x<b)

        在量子力学中，电子将被满足薛定谔方程的波函数ψ(x)描述。此处讨论电子在一维定态下量子隧穿的情况，设电子的势能方程为：

$$
V=V(x)
$$

此时波函数也只和空间坐标有关：

$$
\psi=\psi(x)
$$

在定态情况下，不含时薛定谔方程取这样的形式：

$$
\frac{d^2 \psi}{d x^2}+\frac{\hbar^2}{2 m}(E-V) \psi=0
$$

其中：

$$
ℏ=\frac{h}{2π}
$$

        在扫描隧道显微镜工作时，电子可视为从探针区域射向势垒，但由于电子能量小于势垒，在经典力学角度上电子不可能跨过势垒到达样品处，即在样品与探针间不可能存在电流。

        从经典力学角度对电子存在性上进行分析，可将空间区域分为经典允许区与经典禁区。当电子位于探针区域时，此时的电子总能量大于所处位置势能E>V，从经典力学的角度上看，电子能够位于该区域，即经典允许区。当电子处于真空区域时，电子的总能量小于所处位置势能E<V，从经典力学的角度上看电子不可能运动到该区域，即经典禁区。

        在经典允许区中，V=0，薛定谔方程表示为：

$$
\psi^{\prime \prime}+\frac{2 m E}{\hbar^2} \psi=0
$$

设：

$$
\frac{2 m E}{\hbar^2}=k^2
$$

则方程变为：

$$
\psi^{\prime \prime}+k^2 \psi=0
$$

该微分方程的通解为：

$$
\psi_1(x)=A \sin (k x+\delta), \delta<\pi
$$

在经典禁区中的薛定谔方程为：

$$
\psi^{\prime \prime}-\frac{2 m}{\hbar^2}(V-E) \psi=0
$$

设：

$$
\frac{2 m}{\hbar^2}(V-E)=\beta^2
$$

因为E<V1，所以β为实数。此时经典禁区的薛定谔方程变为：

$$
\psi^{\prime \prime}+k^2 \psi=0
$$

该方程的形式解为：

$$
\psi \sim e^{\pm \beta x}
$$

        可见，在经典力学中不可能出现电子的真空势垒中，在量子力学中仍然存在概率分布，并且其以指数形式衰减。

        即对于如势垒模型图描述的模型中，电子将有概率穿过真空势垒，并在样品区域产生透射波。这种电子能够穿透比其能量更高的势垒的效应即量子隧穿效应。

        通过对该模型的边界条件以及连续条件可求解[3][4][5]得到隧穿电流与真空势垒的关系为：

$$
I \propto e^{-2 \kappa d}
$$

 其中：

$$
\kappa=\frac{\sqrt{2m(V-E)}}{\hbar}
$$

        d为探针样品间距。从公式可以看出，当进入隧穿距离后，探针与样品间距与隧穿电流呈指数关系。当探针样品间距离变化0.1nm左右时，隧穿电流大小将改变一个量级[6]，这也为扫描隧道显微镜的超高分辨率提供了理论基础。

# 参考文献

[1].    Lounis S. Theory of scanning tunneling microscopy[J]. arXiv preprint arXiv:1404.0961, 2014.

[2].    Bai C. Scanning tunneling microscopy and its application[M]. Springer Science & Business Media, 2000.

[3].    Baird D, Shew A. Probing the history of scanning tunneling microscopy[J]. Discovering the nanoscale, 2004, 2: 145-156.

[4].    Merzbacher E. Quantum mechanics[M]. Jones & Bartlett Publishers, 1961.

[5].    曾谨言. 量子力学导论[M]. 第二版. 北京大学出版社, 2001.

[6].    王琦. 高稳定扫描隧道显微镜的研制与应用[D].  中国科学技术大学,2014.