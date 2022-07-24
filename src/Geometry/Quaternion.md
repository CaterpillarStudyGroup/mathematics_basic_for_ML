# Quaternion  四元数

此条目介绍的是数学中的四元数。 关于其他用法，请见“四元数（消歧义）”。

四元数乘法表

||1|	i|	j|	k|
|---|---|---|---|---|
|1|	1|	i|	j|	k|
|i|	i|	−1|	k|	−j|
|j|	j|	−k|	−1|	i|
|k|	k|	j|	−i|	−1|

![](图片/11.jpg)

>- "Julia Quaternion 3" by Aiekick  
Aiekick的“Julia Quaternion 3”

在数学中，四元数系统扩展了复数。 四元数由爱尔兰数学家威廉·罗文·Hamilton于 1843 年[1][2] 首次描述，并应用于三维空间的力学。 Hamilton将四元数定义为三维空间中两条有向线的商，[3] 或者等效地，定义为两个向量的商。 [4] 四元数的乘法是不可交换的。

>**[success]**  
**两个向量的商**：最初引入四元数是为了定义向量的除法

四元数一般用以下形式表示

$$
{\displaystyle a+b\ \mathbf {i} +c\ \mathbf {j} +d\ \mathbf {k} }
$$

其中 a、b、c 和 d 是实数； i, j, k 是基本四元数。

四元数用于纯数学，但在应用数学中也有实际用途，特别是用于涉及三维旋转的计算，例如三维计算机图形学、计算机视觉和晶体纹理分析。 [5] 它们可以与其他旋转方法一起使用，例如欧拉角和旋转矩阵，或者作为它们的替代方法，具体取决于应用程序。

In modern mathematical language, quaternions form a four-dimensional associative normed division algebra over the real numbers, and therefore also a domain. The algebra of quaternions is often denoted by H (for Hamilton), or in blackboard bold by $${\displaystyle \mathbb {H} .}$$ It can also be given by the Clifford algebra classifications $${\displaystyle \operatorname {Cl} _{0,2}(\mathbb {R} )\cong \operatorname {Cl} _{3,0}^{+}(\mathbb {R} ).}$$ In fact, it was the first noncommutative division algebra to be discovered.

在现代数学语言中，四元数在实数上**形成一个四维关联范数除法代数，因此也是一个域**。 四元数的代数通常用 H（代表 Hamilton）来表示，或者用黑板粗体表示为 $${\displaystyle \mathbb {H} .}$$ 它也可以由 Clifford 代数分类给出 $${\displaystyle \operatorname {Cl} _{0,2}(\mathbb {R} )\cong \operatorname {Cl} _{3,0}^{+}(\mathbb {R} ).}$$ 其实就是 第一个非交换除法代数被发现。

>**[warning]**  
**关联范数**：？  
**除法代数**：？

According to the Frobenius theorem, the algebra $${\displaystyle \mathbb {H} }$$  is one of only two finite-dimensional division rings containing a proper subring isomorphic to the real numbers; the other being the complex numbers. These rings are also Euclidean Hurwitz algebras, of which quaternions are the largest associative algebra. Further extending the quaternions yields the non-associative octonions, which is the last normed division algebra over the real numbers. (The sedenions, the extension of the octonions, have zero divisors and so cannot be a normed division algebra.)[6]

根据 Frobenius 定理，代数 $${\displaystyle \mathbb {H} }$$ 是仅有的两个包含与实数同构的适当子环的有限维除环之一； 另一个是复数。 这些环也是欧几里得赫维茨代数，其中四元数是最大的结合代数。 进一步扩展四元数产生非结合八元数，这是实数上的最后一个范数除法代数。 （sedenions，八元数的扩展，有零除数，因此不能是规范的除法代数。）[6]

The unit quaternions can be thought of as a choice of a group structure on the 3-sphere S3 that gives the group Spin(3), which is isomorphic to SU(2) and also to the universal cover of SO(3).

单位四元数可以被认为是 3 球体 S3 上的一个群结构的选择，它给出了群 Spin(3)，它与 SU(2) 和 SO(3) 的全覆盖同构。

![](图片/12.png)

Graphical representation of products of quaternion units as 90° rotations in the planes of 4-dimensional space spanned by two of {1, i, j, k}. The left factor can be viewed as being rotated by the right factor to arrive at the product. Visually i ⋅ j = −(j ⋅ i).

四元数单元乘积的图形表示为在4D空间中跨越 {1, i, j, k} 中的两个轴的平面上旋转 90°。 可以看作是左边的因子被右边的因子旋转后得到乘积。 视觉上 i ⋅ j = -(j ⋅ i)。

>**[success]**  
**四元数单元**：unit quaternion：单位四元数，即norm为1的四元数  
quaternion unit:基本四元数，即i,j,k 

- In blue:  蓝色

  -  1 ⋅ i = i (1/i 平面)

  -  i ⋅ j = k (i/k 平面)

- In red:  红色

  -  1 ⋅ j = j (1/j 平面)

  -  j ⋅ i = -k (j/k 平面)

# History  历史

*Main article: History of quaternions*

*主条目：四元数的历史*

![](图片/3.jpg)

都柏林布鲁厄姆（布鲁姆）桥上的四元数牌匾，上面写着：

Here as he walked by   
on the 16th of October 1843  
Sir William Rowan Hamilton  
in a flash of genius discovered  
the fundamental formula for  
quaternion multiplication  
i2 = j2 = k2 = i j k = −1  
& cut it on a stone of this bridge  

四元数由Hamilton于 1843 年引入。 [7] 这项工作的重要前身包括欧拉的四平方恒等式 (1748) 和奥林德罗德里格斯 (Olinde Rodrigues) 通过四个参数对一般旋转进行参数化 (1840)，但这些作者都没有将四参数旋转视为代数。 [8] [9] 卡尔·弗里德里希·高斯也在 1819 年发现了四元数，但这项工作直到 1900 年才发表。[10][11]

Hamilton知道复数可以解释为平面上的点，他正在寻找一种方法来对三维空间中的点做同样的事情。 空间中的点可以用它们的坐标来表示，坐标是三元组的数字，而且多年来他一直知道如何加减三元组的数字。 然而，很长一段时间，他一直被困在乘除法的问题上。 他不知道如何计算空间中两点坐标的商。 事实上，Ferdinand Georg Frobenius 后来在 1877 年证明，实数上的除法代数是有限维和结合的，它不可能是三维的，并且只有三个这样的除法代数： $${\displaystyle \mathbb {R,C} }$$（复数）和 $${\displaystyle \mathbb {H} }$$（四元数），它们的维数分别为 1、2 和 4。

The great breakthrough in quaternions finally came on Monday 16 October 1843 in Dublin, when Hamilton was on his way to the Royal Irish Academy where he was going to preside at a council meeting. As he walked along the towpath of the Royal Canal with his wife, the concepts behind quaternions were taking shape in his mind. When the answer dawned on him, Hamilton could not resist the urge to carve the formula for the quaternions,

四元数的重大突破终于在 1843 年 10 月 16 日星期一在都柏林出现，当时Hamilton正在前往爱尔兰皇家学院的路上，他将在那里主持一次理事会会议。 当他和妻子沿着皇家运河的纤道行走时，四元数背后的概念正在他的脑海中形成。当答案浮出水面时，Hamilton忍不住想写出四元数的公式

$$
{\displaystyle \mathbf {i} ^{2}=\mathbf {j} ^{2}=\mathbf {k} ^{2}=\mathbf {i\,j\,k} =-1}
$$

into the stone of Brougham Bridge as he paused on it. Although the carving has since faded away, there has been an annual pilgrimage since 1989 called the Hamilton Walk for scientists and mathematicians who walk from Dunsink Observatory to the Royal Canal bridge in remembrance of Hamilton's discovery.

进入布鲁厄姆桥的石头，他停在上面。尽管雕刻已经消失，但自 1989 年以来，每年都会举行一次名为“Hamilton步行”的朝圣活动，供科学家和数学家从邓辛克天文台步行到皇家运河桥，以纪念Hamilton的发现。

On the following day, Hamilton wrote a letter to his friend and fellow mathematician, John T. Graves, describing the train of thought that led to his discovery. This letter was later published in a letter to the London, Edinburgh, and Dublin Philosophical Magazine and Journal of Science;[12] Hamilton states:

第二天，Hamilton给他的朋友兼数学家约翰·格雷夫斯写了一封信，描述了导致他发现的思路。 这封信后来发表在给伦敦、爱丁堡和都柏林哲学杂志和科学杂志上。在信中；[12] Hamilton说：

And here there dawned on me the notion that we must admit, in some sense, a fourth dimension of space for the purpose of calculating with triples ... An electric circuit seemed to close, and a spark flashed forth.[12]

在这里，我突然想到，在某种意义上，我们必须承认空间的第四维度，以便用三元组进行计算……电路似乎闭合了，火花闪现。 [12]

>**[success]**  
**必须承认空间的第四维度，以便用三元组进行计算**：通过人为地增加一个维度，来解决原本在低维空间中无法解决的问题，这是一个很好的解题思路，其次坐标系也是这样的原理。

Hamilton called a quadruple with these rules of multiplication a quaternion, and he devoted most of the remainder of his life to studying and teaching them. Hamilton's treatment is more geometric than the modern approach, which emphasizes quaternions' algebraic properties. He founded a school of "quaternionists", and he tried to popularize quaternions in several books. The last and longest of his books, Elements of Quaternions,[13] was 800 pages long; it was edited by his son and published shortly after his death.

Hamilton将具有这些乘法规则的四元数称为四元数，他将余生的大部分时间都用于研究和教授它们。 Hamilton的处理比现代方法更几何，后者强调四元数的代数性质。 他创立了“四元数论者quaternionists”学派，并试图在几本书中普及四元数。 他的最后一部也是最长的一本书《四元数的元素》[13] 长达 800 页； 它由他的儿子编辑，并在他去世后不久出版。

Hamilton去世后，苏格兰数学物理学家彼得·泰特成为四元数的主要成员。 当时，四元数是都柏林的必考科目。在物理和几何也使用向量描述的主题，例如空间运动学和麦克斯韦方程，都完全用四元数来描述。 甚至还有一个专业的研究协会，即四元数协会，致力于研究四元数和其他超复数系统。

从 1880 年代中期开始，四元数开始被 Josiah Willard Gibbs、Oliver Heaviside 和 Hermann von Helmholtz 开发的**矢量分析**所取代。 矢量分析描述了与四元数相同的现象，因此它从有关四元数的文献中大量借用了一些思想和术语。 然而，矢量分析在概念上更简单，符号更清晰，最终四元数在数学和物理学中被贬为次要角色。 这种转变的一个副作用是Hamilton的作品对于许多现代读者来说难以理解。 Hamilton最初的定义是陌生的，他的写作风格冗长且难以理解。

然而，自 20 世纪后期以来，四元数得到了复兴，这主要是由于它们在**描述空间旋转**方面的实用性。 四元数的旋转表示比矩阵的表示更紧凑，计算速度更快。 此外，与欧拉角不同，它们不易受到“万向节死锁”的影响。 因此，四元数被用于计算机图形学、[14][15] 计算机视觉、机器人学、[16] 控制理论、信号处理、姿态控制、物理学、生物信息学、[17][18] 分子动力学、计算机模拟、 和轨道力学。 例如，航天器的姿态控制系统通常以四元数来控制。 由于四元数与二次形式的关系，四元数从数论中得到了另一个推动。 [19]

>**[success]**  
用四元数表示旋转的优势：①比矩阵的表示更紧凑，计算速度更快  
②不易受到“万向节死锁”的影响  
③插值结果更稳定

## Quaternions in physics  物理学中的四元数

P.R. Girard's 1984 essay The quaternion group and modern physics[20] discusses some roles of quaternions in physics. The essay shows how various physical covariance groups, namely SO(3), the Lorentz group, the general theory of relativity group, the Clifford algebra SU(2) and the conformal group, can easily be related to the quaternion group in modern algebra. Girard began by discussing group representations and by representing some space groups of crystallography. He proceeded to kinematics of rigid body motion. Next he used complex quaternions (biquaternions) to represent the Lorentz group of special relativity, including the Thomas precession. He cited five authors, beginning with Ludwik Silberstein, who used a potential function of one quaternion variable to express Maxwell's equations in a single differential equation. Concerning general relativity, he expressed the Runge–Lenz vector. He mentioned the Clifford biquaternions (split-biquaternions) as an instance of Clifford algebra. Finally, invoking the reciprocal of a biquaternion, Girard described conformal maps on spacetime. Among the fifty references, Girard included Alexander Macfarlane and his Bulletin of the Quaternion Society. In 1999 he showed how Einstein's equations of general relativity could be formulated within a Clifford algebra that is directly linked to quaternions.[21]

P.R. Girard 1984 年的文章四元数群和现代物理学[20] 讨论了四元数在物理学中的一些作用。文章展示了各种物理协方差群，即 SO(3)、洛伦兹群、广义相对论群、克利福德代数 SU(2) 和共形群，如何很容易地与现代代数中的四元数群联系起来。 Girard 首先讨论了群表示并代表了晶体学的一些空间群。他着手研究刚体运动的运动学。接下来他用复四元数（biquaternions）来表示狭义相对论的洛伦兹群，包括托马斯岁差。他引用了五位作者，首先是 Ludwik Silberstein，他们使用一个四元数变量的势函数在单个微分方程中表达麦克斯韦方程。关于广义相对论，他表达了龙格-楞次向量。他提到了 Clifford 双四元数（split-biquaternions）作为 Clifford 代数的一个实例。最后，利用双四元数的倒数，吉拉德描述了时空共形映射。在五十篇参考文献中，吉拉德包括亚历山大麦克法兰和他的四元数协会公报。 1999 年，他展示了如何在与四元数直接相关的克利福德代数中制定爱因斯坦的广义相对论方程。 [21]

The finding of 1924 that in quantum mechanics the spin of an electron and other matter particles (known as spinors) can be described using quaternions furthered their interest; quaternions helped to understand how rotations of electrons by 360° can be discerned from those by 720° (the "Plate trick").[22][23] As of 2018, their use has not overtaken rotation groups.[a]

1924 年发现，在量子力学中，电子和其他物质粒子（称为自旋量）的自旋可以用四元数来描述，这进一步激发了他们的兴趣。 四元数有助于理解电子旋转 360° 与 720° 旋转的区别（“板技巧”）。[22][23] 截至 2018 年，它们的使用尚未超过轮换组。[a]

# Definition  定义

A quaternion is an expression of the form

四元数的表达形式为

$$
{\displaystyle a+b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} \ ,}
$$

其中 a、b、c、d 是实数，i、j、k 是可以解释为指向三个空间轴的单位向量的符号。 在实际应用中，如果a、b、c、d之一为0，则省略对应项； 如果a、b、c、d都为零，则该四元数是零四元数，记为0； 如果 b、c、d 中的一个等于 1，则相应的项只写为 i、j 或 k。

Hamilton 将四元数 $${\displaystyle q=a+b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} }$$ 描述为由一个标量部分和 向量部分。 四元数 $${\displaystyle b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} }$$ 称为 q 的向量部分（有时是虚部），并且 a 是 q 的标量部分（有时是实部）。 等于其实部（即其向量部分为零）的四元数称为标量或实数四元数，并用相应的实数标识。 也就是说，实数嵌入在四元数中。 （更准确地说，实数域同构于四元数的一个子集。复数域也同构于三个四元数子集。）[24] 等于其向量部分的四元数称为向量四元数。

The set of quaternions is made a 4-dimensional vector space over the real numbers, with $${\displaystyle \left\{1,\mathbf {i} ,\mathbf {j} ,\mathbf {k} \right\}}{\displaystyle \left\{1,\mathbf {i} ,\mathbf {j} ,\mathbf {k} \right\}}$$ as a basis, by the componentwise addition

四元数集在实数上构成一个 4 维向量空间，以$${\displaystyle \left\{1,\mathbf {i} ,\mathbf {j} ,\mathbf {k} \right\} }{\displaystyle \left\{1,\mathbf {i} ,\mathbf {j} ,\mathbf {k} \right\}}$$ 作为基，使用逐分量的加法

>**[success]**  
逐分量加法：依次对每前分量前的系数做加法操作

$$
{\displaystyle (a_{1}+b_{1}\,\mathbf {i} +c_{1}\,\mathbf {j} +d_{1}\,\mathbf {k} )+(a_{2}+b_{2}\,\mathbf {i} +c_{2}\,\mathbf {j} +d_{2}\,\mathbf {k} )=(a_{1}+a_{2})+(b_{1}+b_{2})\,\mathbf {i} +(c_{1}+c_{2})\,\mathbf {j} +(d_{1}+d_{2})\,\mathbf {k} \,,}
$$

and the componentwise scalar multiplication

和分量标量乘法

>**[success]**  
分量标量乘：依次让每个分量的系数与一个标量相乘  
标量即0维数字

$$
{\displaystyle \lambda (a+b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} )=\lambda a+(\lambda b)\,\mathbf {i} +(\lambda c)\,\mathbf {j} +(\lambda d)\,\mathbf {k} .}
$$

A multiplicative group structure, called the Hamilton product, denoted by juxtaposition, can be defined on the quaternions in the following way:

可以通过以下方式在四元数上定义乘法群结构，称为 Hamilton 积，用juxtaposition表示：

- The real quaternion 1 is the identity element.  
实四元数 1 是单位元。

- The real quaternions commute with all other quaternions, that is aq = qa for every quaternion q and every real quaternion a. In algebraic terminology this is to say that the field of real quaternions are the center of this quaternion algebra.  
实四元数与所有其他四元数满足交换律，即对于每一个四元数 q 和每一个实四元数 a，aq = qa。 在代数术语中，这就是说实四元数域是这个四元数代数的中心。

>**[success]**  
下文3.2会解释“代数的中心”概念

- The product is first given for the basis elements (see next subsection), and then extended to all quaternions by using the distributive property and the center property of the real quaternions. The Hamilton product is not commutative, but is associative, thus the quaternions form an associative algebra over the real numbers.  
首先给出基元素的乘积（见下一小节），然后利用实四元数的分布性质和中心性质扩展到所有四元数。 Hamilton积不是可交换的，而是结合的，因此四元数在实数上形成结合代数。

- Additionally, every nonzero quaternion has an inverse with respect to the Hamilton product:  
此外，根据Hamilton 积的定义每个非零四元数都有逆：

$$
{\displaystyle (a+b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} )^{-1}={\frac {1}{a^{2}+b^{2}+c^{2}+d^{2}}}\,(a-b\,\mathbf {i} -c\,\mathbf {j} -d\,\mathbf {k} ).}
$$

Thus the quaternions form a division algebra.

因此，四元数形成一个除法代数。

## Multiplication of basis elements  基本元素的乘法

Multiplication table  乘法表

Non commutativity is emphasized by colored squares  非交换性用彩色方块强调

|×|1|i|j|k|
|---|---|---|---|---|
|1|1|i|j|k|
|i|i|−1|k|−j|
|j|j|−k|−1|i|
|k|k|j|−i|−1|

The multiplication with 1 of the basis elements i, j, and k is defined by the fact that 1 is a multiplicative identity, that is,

由于1是乘法单位，基元素 i、j 和 k 与 1 的乘法定义如下，即

$$
{\displaystyle \mathbf {i} \,1=1\,\mathbf {i} =\mathbf {i} ,\qquad \mathbf {j} \,1=1\,\mathbf {j} =\mathbf {j} ,\qquad \mathbf {k} \,1=1\,\mathbf {k} =\mathbf {k} \,.}
$$

The products of basis elements are derived from the product rules for $${\displaystyle \mathbf {i} }$$ and $${\displaystyle \mathbf {j}}$$

基元素的乘积源自 $${\displaystyle \mathbf {i} }$$ 和 $${\displaystyle \mathbf {j} }$$ 的乘积规则：

$$
{\displaystyle \mathbf {i} ^{2}=\mathbf {j} ^{2}=-1}
$$

and 并且

$$
{\displaystyle {\begin{aligned}\mathbf {i\,j} &=\mathbf {k} \,,\quad &\mathbf {j\,i} &=-\mathbf {k} \,.\end{aligned}}}
$$

>**[success]**  
类似3D中的叉积

The remaining product rules are obtained by multiplying both sides of these latter rules by $${\displaystyle \mathbf {j} }$$ or $${\displaystyle \mathbf {i} }$$ from the left or right and applying associativity which gives

剩下的乘积规则是通过将上面这些规则的两边从左边或右边乘以 $${\displaystyle \mathbf {j} }$$ 或 $${\displaystyle \mathbf {i} }$$ 并应用关联性来获得的：

$$
{\displaystyle {\begin{aligned}\mathbf {j\,k} &=\mathbf {i} \,,\quad &\mathbf {k\,j} &=-\mathbf {i} \,,\\\mathbf {k\,i} &=\mathbf {j} \,,\quad &\mathbf {i\,k} &=-\mathbf {j} \,,\\\mathbf {i\,j\,k} &=-1\,,\quad &\mathbf {k} ^{2}&=-1\,\\\end{aligned}}}
$$

## Center  中心

The center of a noncommutative ring is the subring of elements c such that cx = xc for every x. The center of the quaternion algebra is the subfield of real quaternions. In fact, it is a part of the definition that the real quaternions belong to the center. Conversely, if q = a + b i + c j + d k belongs to the center, then

非交换环的中心是元素 c 的子环，使得对于每个 x，cx = xc。 四元数代数的中心是实四元数的子域。 事实上，实四元数属于中心是定义的一部分。 反之，若 q = a + b i + c j + d k 属于中心，则

>**[success]**  
**非交换环的中心是元素 c 的子环，使得对于每个 x，cx = xc**：代数中心的定义

$$
{\displaystyle 0=\mathbf {i} \,q-q\,\mathbf {i} =2c\,\mathbf {ij} +2d\,\mathbf {ik} =2c\,\mathbf {k} -2d\,\mathbf {j} \,,}
$$

and c = d = 0. A similar computation with j instead of i shows that one has also b = 0. Thus q = a is a real quaternion.

得出 c = d = 0。用 j 代替 i 做类似计算也能得出 b = 0。因此 q = a 是一个实四元数。

The quaternions form a division algebra. This means that the non-commutativity of multiplication is the only property that makes quaternions different from a field. This non-commutativity has some unexpected consequences, among them that a polynomial equation over the quaternions can have more distinct solutions than the degree of the polynomial. For example, the equation z2 + 1 = 0, has infinitely many quaternion solutions, which are the quaternions z = b i + c j + d k such that b2 + c2 + d2 = 1. Thus these "roots of –1" form a unit sphere in the three-dimensional space of vector quaternions.

四元数构成一个除法代数。 这意味着乘法的不可交换性是使四元数不同于域的唯一属性。 这种非交换性有一些意想不到的后果，其中包括四元数上的多项式方程可以有比多项式的次数更多不同的解。 例如，方程 z2 + 1 = 0 有无限多个四元数解，即四元数 z = bi + cj + dk 使得 b2 + c2 + d2 = 1。因此这些“–1 的根” 在向量四元数的三维空间中形成一个单位球体。

## Hamilton product  Hamilton积

For two elements a1 + b1i + c1j + d1k and a2 + b2i + c2j + d2k, their product, called the Hamilton product (a1 + b1i + c1j + d1k) (a2 + b2i + c2j + d2k), is determined by the products of the basis elements and the distributive law. The distributive law makes it possible to expand the product so that it is a sum of products of basis elements. This gives the following expression:

对于两个元素 a1 + b1i + c1j + d1k 和 a2 + b2i + c2j + d2k，它们的乘积，称为 Hamilton 乘积 (a1 + b1i + c1j + d1k) (a2 + b2i + c2j + d2k)，由基本要素的乘积和分配律推导出。 分配律使得能够扩展乘法规则，使其成为基本要素的乘积之和。 得出了以下表达式：

$$
{\displaystyle {\begin{alignedat}{4}&a_{1}a_{2}&&+a_{1}b_{2}\mathbf {i} &&+a_{1}c_{2}\mathbf {j} &&+a_{1}d_{2}\mathbf {k} \\{}+{}&b_{1}a_{2}\mathbf {i} &&+b_{1}b_{2}\mathbf {i} ^{2}&&+b_{1}c_{2}\mathbf {ij} &&+b_{1}d_{2}\mathbf {ik} \\{}+{}&c_{1}a_{2}\mathbf {j} &&+c_{1}b_{2}\mathbf {ji} &&+c_{1}c_{2}\mathbf {j} ^{2}&&+c_{1}d_{2}\mathbf {jk} \\{}+{}&d_{1}a_{2}\mathbf {k} &&+d_{1}b_{2}\mathbf {ki} &&+d_{1}c_{2}\mathbf {kj} &&+d_{1}d_{2}\mathbf {k} ^{2}\end{alignedat}}}
$$

Now the basis elements can be multiplied using the rules given above to get:[7]

现在可以使用上面给出的规则将基本元素相乘得到：[7]

$$
{\displaystyle {\begin{alignedat}{4}&a_{1}a_{2}&&-b_{1}b_{2}&&-c_{1}c_{2}&&-d_{1}d_{2}\\{}+{}(&a_{1}b_{2}&&+b_{1}a_{2}&&+c_{1}d_{2}&&-d_{1}c_{2})\mathbf {i} \\{}+{}(&a_{1}c_{2}&&-b_{1}d_{2}&&+c_{1}a_{2}&&+d_{1}b_{2})\mathbf {j} \\{}+{}(&a_{1}d_{2}&&+b_{1}c_{2}&&-c_{1}b_{2}&&+d_{1}a_{2})\mathbf {k} \end{alignedat}}}
$$

The product of two rotation quaternions[25] will be equivalent to the rotation a2 + b2i + c2j + d2k followed by the rotation a1 + b1i + c1j + d1k.

两个旋转四元数[25] 的乘积将等价于旋转 a2 + b2i + c2j + d2k，然后是旋转 a1 + b1i + c1j + d1k。

>**[success]**  
$q_1\times q_2$ 等价于先旋转$q_2$再旋转$q_1$

>**[warning]**  
q的旋转怎么定义？

## Scalar and vector parts  标量和矢量部分

A quaternion of the form a + 0 i + 0 j + 0 k, where a is a real number, is called scalar, and a quaternion of the form 0 + b i + c j + d k, where b, c, and d are real numbers, and at least one of b, c or d is nonzero, is called a vector quaternion. If a + b i + c j + d k is any quaternion, then a is called its scalar part and b i + c j + d k is called its vector part. Even though every quaternion can be viewed as a vector in a four-dimensional vector space, it is common to refer to the vector part as vectors in three-dimensional space. With this convention, a vector is the same as an element of the vector space $${\displaystyle \mathbb {R} ^{3}.}$$[b]

a + 0 i + 0 j + 0 k 形式的四元数，其中 a 是实数，称为标量，0 + bi + cj + dk 形式的四元数，其中 b、c 和 d 是实数 数，且 b、c 或 d 中至少有一个非零，称为向量四元数。 如果 a + b i + c j + d k 是任何四元数，则 a 称为其标量部分，而 b i + c j + d k 称为其矢量部分。 尽管每个四元数都可以被视为四维向量空间中的向量，但通常**将向量部分称为三维空间中的向量**。 按照这种约定，向量与向量空间中的元素相同 $${\displaystyle \mathbb {R} ^{3}.}$$[b]

Hamilton also called vector quaternions right quaternions[27][28] and real numbers (considered as quaternions with zero vector part) scalar quaternions.

Hamilton还将向量四元数称为右四元数[27][28] 将实数（被认为是具有零向量部分的四元数）称为标量四元数。

If a quaternion is divided up into a scalar part and a vector part, that is,

如果将一个四元数分为标量部分和向量部分，即

$$
{\displaystyle \mathbf {q} =(r,\ {\vec {v}}),~~\mathbf {q} \in \mathbb {H} ,~~r\in \mathbb {R} ,~~{\vec {v}}\in \mathbb {R} ^{3},}
$$

then the formulas for addition and multiplication are

那么加法和乘法的公式是

$$
{\displaystyle (r_{1},\ {\vec {v}}_{1})+(r_{2},\ {\vec {v}}_{2})=(r_{1}+r_{2},\ {\vec {v}}_{1}+{\vec {v}}_{2}),}
{\displaystyle (r_{1},\ {\vec {v}}_{1})(r_{2},\ {\vec {v}}_{2})=(r_{1}r_{2}-{\vec {v}}_{1}\cdot {\vec {v}}_{2},\ r_{1}{\vec {v}}_{2}+r_{2}{\vec {v}}_{1}+{\vec {v}}_{1}\times {\vec {v}}_{2}),}
$$

where "$${\displaystyle \cdot }$$ " and "$${\displaystyle \times }$$ " denote respectively the dot product and the cross product.

其中“$${\displaystyle \cdot }$$ ”和“$${\displaystyle \times }$$ ”分别表示点积和叉积。

# Conjugation, the norm, and reciprocal  共轭、范数和倒数

Conjugation of quaternions is analogous to conjugation of complex numbers and to transposition (also known as reversal) of elements of Clifford algebras. To define it, let $${\displaystyle q=a+b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} }$$ be a quaternion. The conjugate of q is the quaternion $${\displaystyle q^{*}=a-b\,\mathbf {i} -c\,\mathbf {j} -d\,\mathbf {k} }.$$ It is denoted by q∗, qt, $${\displaystyle {\tilde {q}}}$$, or q.[7] Conjugation is an involution, meaning that it is its own inverse, so conjugating an element twice returns the original element. The conjugate of a product of two quaternions is the product of the conjugates in the reverse order. That is, if p and q are quaternions, then (pq)∗ = q∗p∗, not p∗q∗.

四元数的共轭类似于复数的共轭和 Clifford 代数元素的转置（也称为反转）。 为了定义它，令 $${\displaystyle q=a+b\,\mathbf {i} +c\,\mathbf {j} +d\,\mathbf {k} }$$ 是一个四元数。 q 的共轭是四元数 $${\displaystyle q^{*}=a-b\,\mathbf {i} -c\,\mathbf {j} -d\,\mathbf {k} }.$$ 它可以用 q∗、qt、$${\displaystyle {\tilde {q}}}$$ 或 q 表示。[7] 共轭是对合，这意味着它是它自己的逆，所以共轭一个元素两次返回原始元素。 两个四元数乘积的共轭是共轭逆序的乘积。 也就是说，如果 p 和 q 是四元数，那么 (pq)∗ = q∗p∗，而不是 p∗q∗。

>**[success]**  
**对合**：involution

The conjugation of a quaternion, in stark contrast to the complex setting, can be expressed with multiplication and addition of quaternions:

与复数不同，四元数的共轭，可以用四元数的乘法和加法来表示：

$$
{\displaystyle q^{*}=-{\frac {1}{2}}(q+\,\mathbf {i} \,q\,\mathbf {i} +\,\mathbf {j} \,q\,\mathbf {j} +\,\mathbf {k} \,q\,\mathbf {k} )~.}
$$

>**[warning]**  
这个公式很奇怪

Conjugation can be used to extract the scalar and vector parts of a quaternion. The scalar part of p is 
1
/
2
(p + p∗) , and the vector part of p is 
1
/
2
(p − p∗) .

共轭可用于提取四元数的标量和向量部分。 p 的标量部分是
1
/
2
(p + p∗) ，而 p 的向量部分是
1
/
2
(p - p*) 。

The square root of the product of a quaternion with its conjugate is called its norm and is denoted ||q|| (Hamilton called this quantity the tensor of q, but this conflicts with the modern meaning of "tensor"). In formulas, this is expressed as follows:

四元数与其共轭的乘积的平方根称为其范数，记为 ||q|| （Hamilton称这个量为 q 的张量，但这与“张量”的现代含义相冲突）。 在公式中，这表示如下：

$$
{\displaystyle \lVert q\rVert ={\sqrt {\,qq^{*}~}}={\sqrt {\,q^{*}q~}}={\sqrt {\,a^{2}+b^{2}+c^{2}+d^{2}~}}}
$$

This is always a non-negative real number, and it is the same as the Euclidean norm on $${\displaystyle \mathbb {H} }$$  considered as the vector space $${\displaystyle \mathbb {R} ^{4}}$$. Multiplying a quaternion by a real number scales its norm by the absolute value of the number. That is, if α is real, then

这始终是一个非负实数，它与被视为向量空间 $${\displaystyle \mathbb {H} }$$  的 $${\displaystyle \mathbb {R} ^{4}}$$ 上的欧几里得范数相同。 将一个四元数乘以一个实数会按该数的绝对值缩放其范数。 也就是说，如果 α 是实数，那么

$${\displaystyle \lVert \alpha q\rVert =\left|\alpha \right|\,\lVert q\rVert ~.}$$

This is a special case of the fact that the norm is multiplicative, meaning that

范数可以相乘是四元数的一个特例，这意味着

$$
{\displaystyle \lVert pq\rVert =\lVert p\rVert \,\lVert q\rVert }
$$

for any two quaternions p and q. Multiplicativity is a consequence of the formula for the conjugate of a product. Alternatively it follows from the identity

对于任何两个四元数 p 和 q。 乘法性是乘积共轭公式的结果。 或者它来自身份

>**[warning]**  
这一段没看懂

$$
{\displaystyle \det {\Bigl (}{\begin{array}{cc}a+ib&id+c\\id-c&a-ib\end{array}}{\Bigr )}=a^{2}+b^{2}+c^{2}+d^{2},}
$$

(where i denotes the usual imaginary unit) and hence from the multiplicative property of determinants of square matrices.

（其中 i 表示通常的虚数单位），因此来自方阵行列式的乘法性质。

This norm makes it possible to define the distance d(p, q) between p and q as the norm of their difference:

通过范数可以将 p 和 q 之间的距离 d(p, q) 定义为它们的差异的范数：

$$
{\displaystyle d(p,q)=\lVert p-q\rVert ~.}
$$

This makes $${\displaystyle \mathbb {H} }$$  a metric space. Addition and multiplication are continuous in regard to the associated metric topology. This follows with exacly the same proof as for the real numbers $${\displaystyle \mathbb {R} }$$  from the fact that $${\displaystyle \mathbb {H} }$$ is a normed algebra.

>**[warning]**  
**associated metric topology**：什么是metric topology？怎么定义associate？

这使得 $${\displaystyle \mathbb {H} }$$ 成为一个度量空间。 关于相关的度量拓扑，加法和乘法是连续的。 这与实数 $${\displaystyle \mathbb {R} }$$ 的证明完全相同，因为 $${\displaystyle \mathbb {H} }$$ 是一个范数代数。

## Unit quaternion  单位四元数

*Main article: Versor*

*主条目：Versor*

A unit quaternion is a quaternion of norm one. Dividing a non-zero quaternion q by its norm produces a unit quaternion Uq called the versor of q:

单位四元数是范数为一的四元数。 将非零四元数 q 除以其范数产生一个单位四元数 Uq，称为 q 的 versor：

$$
{\displaystyle \mathbf {U} q={\frac {q}{\lVert q\rVert }}.}
$$

Every quaternion has a polar decomposition $${\displaystyle q=\lVert q\rVert \cdot \mathbf {U} q}.$$

每个四元数都有一个极分解 $${\displaystyle q=\lVert q\rVert \cdot \mathbf {U} q}.$$

Using conjugation and the norm makes it possible to define the reciprocal of a non-zero quaternion. The product of a quaternion with its reciprocal should equal 1, and the considerations above imply that the product of $${\displaystyle q} $$and $${\displaystyle q^{*}/\left\Vert q\right\|^{2}}$$ is 1 (for either order of multiplication). So the reciprocal of q is defined to be

使用共轭和范数可以定义非零四元数的倒数。 四元数与其倒数的乘积应该等于 1，上述考虑意味着 $${\displaystyle q} $$和 $${\displaystyle q^{*}/\left\Vert q\right\|^{2}}$$的乘积 为 1（对于任一乘法顺序）。 所以q的倒数定义为

>**[success]**  
**对于任一乘法顺序**：$||q||^2$是实数，因此乘法顺序可交换

$$
{\displaystyle q^{-1}={\frac {q^{*}}{\lVert q\rVert ^{2}}}.}.
$$

![](图片/注释1.jpg)

This makes it possible to divide two quaternions p and q in two different ways (when q is non-zero). That is, their quotient can be either p q−1 or q−1p ; in general, those products are different, depending on the order of multiplication, except for the special case that p and q are scalar multiples of each other (which includes the case where p = 0). Hence, the notation 
p
/
q
 is ambiguous because it does not specify whether q divides on the left or the right (whether  q−1 multiplies p on its left or its right).

 这使得可以以两种不同的方式划分两个四元数 p 和 q（当 q 非零时）。 也就是说，它们的商可以是 p q−1 或 q−1p ； 一般来说，这些乘积是不同的，具体取决于乘法的顺序，除了 p 和 q 是彼此的标量倍数的特殊情况（包括 p = 0 的情况）。 因此，符号
p
/
q
  是模棱两可的，因为它没有指定 q 是在左边还是右边除（ q−1 是在它的左边还是右边乘以 p）。

# Algebraic properties  代数性质

![](图片/14.png)

>- Cayley graph of Q8. The red arrows represent multiplication on the right by i, and the green arrows represent multiplication on the right by j.  
Q8的凯莱图。 红色箭头代表右边乘以 i，绿色箭头代表右边乘以 j。

The set $${\displaystyle \mathbb {H} }$$  of all quaternions is a vector space over the real numbers with dimension 4.[c] Multiplication of quaternions is associative and distributes over vector addition, but with the exception of the scalar subset, it is not commutative. Therefore, the quaternions $${\displaystyle \mathbb {H} }$$  are a non-commutative, associative algebra over the real numbers. Even though $${\displaystyle \mathbb {H} }$$  contains copies of the complex numbers, it is not an associative algebra over the complex numbers.

所有四元数的集合 $${\displaystyle \mathbb {H} }$$ 是维数为 4 的实数上的向量空间。[c] 四元数满足乘法结合律和加法分配律，不满足交换律（除了其标量子集可交换—）。 因此，四元数 $${\displaystyle \mathbb {H} }$$ 是实数上的非交换结合代数。 尽管 $${\displaystyle \mathbb {H} }$$ 包含复数的副本，但它不是复数上的结合代数。

Because it is possible to divide quaternions, they form a division algebra. This is a structure similar to a field except for the non-commutativity of multiplication. Finite-dimensional associative division algebras over the real numbers are very rare. The Frobenius theorem states that there are exactly three: $${\displaystyle \mathbb {R} }$$ , $${\displaystyle \mathbb {C} }$$ , and $${\displaystyle \mathbb {H} }$$ . The norm makes the quaternions into a normed algebra, and normed division algebras over the real numbers are also very rare: Hurwitz's theorem says that there are only four: $${\displaystyle \mathbb {R} }$$ , $${\displaystyle \mathbb {C} }$$ , $${\displaystyle \mathbb {H} }$$ , and $${\displaystyle \mathbb {O} }$$  (the octonions). The quaternions are also an example of a composition algebra and of a unital Banach algebra.

因为四元数可以相除，所以它们形成了一个除法代数。 这是一个类似于域的结构，除了乘法的不可交换性。 实数上的有限维关联除法代数非常罕见。 Frobenius 定理指出正好有三个：$${\displaystyle \mathbb {R} }$$ 、$${\displaystyle \mathbb {C} }$$ 和 $${\displaystyle \mathbb {H} } $$ 。 范数使四元数成为范数代数，实数上的范数除法也非常罕见：赫尔维茨定理说只有四个： $${\displaystyle \mathbb {R} }$$ , $${\ displaystyle \mathbb {C} }$$ 、 $${\displaystyle \mathbb {H} }$$ 和 $${\displaystyle \mathbb {O} }$$ （八元数）。 四元数也是合成代数和单位巴拿赫代数的一个例子。

![](图片/15.png)

Three-dimensional graph of Q8. Red, green and blue arrows represent multiplication by i, j, and k, respectively. Multiplication by negative numbers are omitted for clarity.

Q8的三维图。 红色、绿色和蓝色箭头分别表示乘以 i、j 和 k。 为清楚起见，省略了乘以负数。

Because the product of any two basis vectors is plus or minus another basis vector, the set {±1, ±i, ±j, ±k} forms a group under multiplication. This non-abelian group is called the quaternion group and is denoted Q8.[29] The real group ring of Q8 is a ring $${\displaystyle \mathbb {R} [\mathrm {Q} _{8}]}$$ which is also an eight-dimensional vector space over $${\displaystyle \mathbb {R} .}$$. It has one basis vector for each element of $${\displaystyle \mathrm {Q} _{8}.}$$ The quaternions are isomorphic to the quotient ring of $${\displaystyle \mathbb {R} [\mathrm {Q} _{8}]}$$ by the ideal generated by the elements 1 + (−1), i + (−i), j + (−j), and k + (−k). Here the first term in each of the differences is one of the basis elements 1, i, j, and k, and the second term is one of basis elements −1, −i, −j, and −k, not the additive inverses of 1, i, j, and k.

因为任何两个基向量的乘积是正负另一个基向量，所以集合{±1，±i，±j，±k}在乘法下形成一个群。 这个非阿贝尔群称为四元数群，记为 Q8。 [29] Q8 的实群环是一个环 $${\displaystyle \mathbb {R} [\mathrm {Q} _{8}]}$$ 也是 $${\displaystyle \mathbb 上的一个八维向量空间 {R} .}$$。 $${\displaystyle \mathrm {Q} _{8}.}$$ 的每个元素都有一个基向量。四元数同构于 $${\displaystyle \mathbb {R} [\mathrm { Q} _{8}]}$$ 由元素 1 + (−1)、i + (−i)、j + (−j) 和 k + (−k) 生成的理想。 这里每个差的第一项是基元素 1、i、j 和 k 之一，第二项是基元素 -1、-i、-j 和 -k 之一，而不是加法逆元 1、i、j 和 k。

# Quaternions and the space geometry  四元数和空间几何

The vector part of a quaternion can be interpreted as a coordinate vector in $${\displaystyle \mathbb {R} ^{3};}$$ therefore, the algebraic operations of the quaternions reflect the geometry of $${\displaystyle \mathbb {R} ^{3}.}$$ Operations such as the vector dot and cross products can be defined in terms of quaternions, and this makes it possible to apply quaternion techniques wherever spatial vectors arise. A useful application of quaternions has been to interpolate the orientations of key-frames in computer graphics.[14]

四元数的向量部分可以解释为 $${\displaystyle \mathbb {R} ^{3};}$$ 中的坐标向量，因此，四元数的代数运算反映了 $${\displaystyle \mathbb {R} ^{3}.}$$ 可以根据四元数定义向量点和叉积等运算，这使得**在出现空间向量的任何地方都可以应用四元数技术**。 四元数的一个有用应用是在计算机图形学中插入关键帧的方向。 [14]

For the remainder of this section, i, j, and k will denote both the three imaginary[30] basis vectors of $${\displaystyle \mathbb {H} }$$  and a basis for $${\displaystyle \mathbb {R} ^{3}.}$$ Replacing i by −i, j by −j, and k by −k sends a vector to its additive inverse, so the additive inverse of a vector is the same as its conjugate as a quaternion. For this reason, conjugation is sometimes called the spatial inverse.

对于本节的接下来部分，i、j 和 k 既表示 $${\displaystyle \mathbb {H} }$$ 的三个虚数[30] 基向量，同时也表示 $${\displaystyle \mathbb { R} ^{3}.}$$ 将 i 替换为 -i，j 替换为 -j，k 替换为 -k 就是向量的加法逆，因此向量的加法逆与它作为四元数的共轭相同 . 因此，共轭有时被称为空间逆。

For two vector quaternions p = b1i + c1j + d1k and q = b2i + c2j + d2k their dot product, by analogy to vectors in $${\displaystyle \mathbb {R} ^{3},}$$ is

对于两个向量四元数 p = b1i + c1j + d1k 和 q = b2i + c2j + d2k 它们的点积，类似于 $${\displaystyle \mathbb {R} ^{3},}$$ 中的向量点积

$$
{\displaystyle p\cdot q=b_{1}b_{2}+c_{1}c_{2}+d_{1}d_{2}~.}
$$

It can also be expressed in a component-free manner as

它也可以用无分量的方式表示为

$$
{\displaystyle p\cdot q=\textstyle {\frac {1}{2}}(p^{*}q+q^{*}p)=\textstyle {\frac {1}{2}}(pq^{*}+qp^{*}).}
$$

This is equal to the scalar parts of the products pq∗, qp∗, p∗q, and q∗p. Note that their vector parts are different.

这等于乘积 pq∗、qp∗、p∗q 和 q∗p 的标量部分。 请注意，它们的矢量部分是不同的。

The cross product of p and q relative to the orientation determined by the ordered basis i, j, and k is

p 和 q 相对于由有序基 i、j 和 k 确定的方向的叉积是

$$
{\displaystyle p\times q=(c_{1}d_{2}-d_{1}c_{2})\mathbf {i} +(d_{1}b_{2}-b_{1}d_{2})\mathbf {j} +(b_{1}c_{2}-c_{1}b_{2})\mathbf {k} \,.}
$$

(Recall that the orientation is necessary to determine the sign.) This is equal to the vector part of the product pq (as quaternions), as well as the vector part of −q∗p∗. It also has the formula

（回想一下，方向是确定符号所必需的。）这等于乘积 pq（作为四元数）的向量部分，以及 -q∗p∗ 的向量部分。 它也有公式

$$
{\displaystyle p\times q=\textstyle {\tfrac {1}{2}}(pq-qp).}
$$

>**[success]**  
经核实，原文章公式中就为qp，而不是-q* p*

For the commutator, [p, q] = pq − qp, of two vector quaternions one obtains

对于交换子，[p, q] = pq - qp，两个向量四元数之一得到

$$
{\displaystyle [p,q]=2p\times q.}
$$

In general, let p and q be quaternions and write

一般来说，设 p 和 q 是四元数并写

$$
{\displaystyle p=p_{\text{s}}+p_{\text{v}},}
$$

$$
{\displaystyle q=q_{\text{s}}+q_{\text{v}},}
$$

where ps and qs are the scalar parts, and pv and qv are the vector parts of p and q. Then we have the formula

其中 ps 和 qs 是标量部分，pv 和 qv 是 p 和 q 的向量部分。 然后我们有公式

$$
{\displaystyle pq=(pq)_{\text{s}}+(pq)_{\text{v}}=(p_{\text{s}}q_{\text{s}}-p_{\text{v}}\cdot q_{\text{v}})+(p_{\text{s}}q_{\text{v}}+q_{\text{s}}p_{\text{v}}+p_{\text{v}}\times q_{\text{v}}).}
$$

This shows that the noncommutativity of quaternion multiplication comes from the multiplication of vector quaternions. It also shows that two quaternions commute if and only if their vector parts are collinear. Hamilton[31] showed that this product computes the third vertex of a spherical triangle from two given vertices and their associated arc-lengths, which is also an algebra of points in Elliptic geometry.

这说明四元数乘法的不可交换性来自向量四元数的乘法。 它还表明，当且仅当它们的向量部分共线时，两个四元数可以交换。 Hamilton[31] 表明，该乘积从两个给定顶点及其相关的弧长计算球面三角形的第三个顶点，这也是椭圆几何中的点代数。

Unit quaternions can be identified with rotations in $${\displaystyle \mathbb {R} ^{3}}$$ and were called versors by Hamilton.[31] Also see Quaternions and spatial rotation for more information about modeling three-dimensional rotations using quaternions.

单位四元数可以用 $${\displaystyle \mathbb {R} ^{3}}$$ 中的旋转来识别，并被 Hamilton 称为 versors。 [31] 另请参阅四元数和空间旋转，了解有关使用四元数对三维旋转进行建模的更多信息。

See Hanson (2005)[32] for visualization of quaternions.

有关四元数的可视化，请参见 Hanson (2005)[32]。

# Matrix representations  矩阵表示

Just as complex numbers can be represented as matrices, so can quaternions. There are at least two ways of representing quaternions as matrices in such a way that quaternion addition and multiplication correspond to matrix addition and matrix multiplication. One is to use 2 × 2 complex matrices, and the other is to use 4 × 4 real matrices. In each case, the representation given is one of a family of linearly related representations. In the terminology of abstract algebra, these are injective homomorphisms from $${\displaystyle \mathbb {H} }$$  to the matrix rings M(2,ℂ) and M(4,ℝ), respectively.

正如复数可以表示为矩阵一样，四元数也可以。 至少有两种将四元数表示为矩阵的方式，即四元数加法和乘法对应于矩阵加法和矩阵乘法。 一种是使用 2 × 2 复矩阵，另一种是使用 4 × 4 实矩阵。 在每种情况下，给定的表示是一系列线性相关的表示之一。 在抽象代数的术语中，这些是从 $${\displaystyle \mathbb {H} }$$ 到矩阵环 M(2,ℂ) 和 M(4,ℝ) 的单射同态。

Using 2 × 2 complex matrices, the quaternion a + bi + cj + dk can be represented as

使用 2 × 2 复矩阵，四元数 a + bi + cj + dk 可以表示为

$$
{\displaystyle {\begin{bmatrix}a+bi&c+di\\-c+di&a-bi\end{bmatrix}}.}
$$

Note that the "i" of the complex numbers is distinct from the "i" of the quaternions.

请注意，**复数的“i”与四元数的“i”不同**。

This representation has the following properties:

此表示具有以下属性：

- Constraining any two of b, c and d to zero produces a representation of complex numbers. For example, setting c = d = 0 produces a diagonal complex matrix representation of complex numbers, and setting b = d = 0 produces a real matrix representation.  
将 b、c 和 d 中的任意两个约束为零会产生复数的表示。 例如，设置 c = d = 0 生成复数的对角复矩阵表示，设置 b = d = 0 生成实矩阵表示。

- The norm of a quaternion (the square root of the product with its conjugate, as with complex numbers) is the square root of the determinant of the corresponding matrix.[33]  
四元数的范数（乘积与其共轭的平方根，与复数一样）是相应矩阵行列式的平方根。 [33]

- The conjugate of a quaternion corresponds to the conjugate transpose of the matrix.  
四元数的共轭对应于矩阵的共轭转置。

- By restriction this representation yields an isomorphism between the subgroup of unit quaternions and their image SU(2). Topologically, the unit quaternions are the 3-sphere, so the underlying space of SU(2) is also a 3-sphere. The group SU(2) is important for describing spin in quantum mechanics; see Pauli matrices.  
通过限制，这种表示在单位四元数的子群和它们的图像 SU(2) 之间产生了同构。 拓扑上，单位四元数是 3 球体，所以 SU(2) 的底层空间也是 3 球体。 SU(2) 群对于描述量子力学中的自旋很重要； 参见泡利矩阵。

- There is a strong relation between quaternion units and Pauli matrices. Obtain the eight quaternion unit matrices by taking a, b, c and d, set three of them at zero and the fourth at 1 or −1. Multiplying any two Pauli matrices always yields a quaternion unit matrix, all of them except for −1. One obtains −1 via i2 = j2 = k2 = i j k = −1; e.g. the last equality is
$${\displaystyle {\begin{aligned}ijk=\sigma _{1}\sigma _{2}\sigma _{3}\sigma _{1}\sigma _{2}\sigma _{3}=-1\end{aligned}}}$$  

四元数单元和Pauli矩阵之间存在很强的关系。 通过取 a、b、c 和 d 获得八个四元数单位矩阵，将其中三个设置为零，第四个设置为 1 或 -1。 将任何两个泡利矩阵相乘总是会产生一个四元数单位矩阵，除了 -1 之外的所有矩阵。 一个通过 i2 = j2 = k2 = i j k = -1 获得 -1； 例如 最后一个等式是
$${\displaystyle {\begin{aligned}ijk=\sigma _{1}\sigma _{2}\sigma _{3}\sigma _{1}\sigma _{2}\sigma _{3}=-1\end{aligned}}}$$  

Using 4 × 4 real matrices, that same quaternion can be written as

使用 4 × 4 实矩阵，相同的四元数可以写为

$$
{\displaystyle {\begin{bmatrix}a&-b&-c&-d\\b&a&-d&c\\c&d&a&-b\\d&-c&b&a\end{bmatrix}}=a{\begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1\end{bmatrix}}+b{\begin{bmatrix}0&-1&0&0\\1&0&0&0\\0&0&0&-1\\0&0&1&0\end{bmatrix}}+c{\begin{bmatrix}0&0&-1&0\\0&0&0&1\\1&0&0&0\\0&-1&0&0\end{bmatrix}}+d{\begin{bmatrix}0&0&0&-1\\0&0&-1&0\\0&1&0&0\\1&0&0&0\end{bmatrix}}.}
$$

However, the representation of quaternions in M(4,ℝ) is not unique. For example, the same quaternion can also be represented as

然而，M(4,ℝ) 中四元数的表示并不是唯一的。 例如，同样的四元数也可以表示为

$$
{\displaystyle {\begin{bmatrix}a&d&-b&-c\\-d&a&c&-b\\b&-c&a&-d\\c&b&d&a\end{bmatrix}}=a{\begin{bmatrix}1&0&0&0\\0&1&0&0\\0&0&1&0\\0&0&0&1\end{bmatrix}}+b{\begin{bmatrix}0&0&-1&0\\0&0&0&-1\\1&0&0&0\\0&1&0&0\end{bmatrix}}+c{\begin{bmatrix}0&0&0&-1\\0&0&1&0\\0&-1&0&0\\1&0&0&0\end{bmatrix}}+d{\begin{bmatrix}0&1&0&0\\-1&0&0&0\\0&0&0&-1\\0&0&1&0\end{bmatrix}}.}
$$

There exist 48 distinct matrix representations of this form in which one of the matrices represents the scalar part and the other three are all skew-symmetric. More precisely, there are 48 sets of quadruples of matrices with these symmetry constraints such that a function sending 1, i, j, and k to the matrices in the quadruple is a homomorphism, that is, it sends sums and products of quaternions to sums and products of matrices.[34] In this representation, the conjugate of a quaternion corresponds to the transpose of the matrix. The fourth power of the norm of a quaternion is the determinant of the corresponding matrix. As with the 2 × 2 complex representation above, complex numbers can again be produced by constraining the coefficients suitably; for example, as block diagonal matrices with two 2 × 2 blocks by setting c = d = 0.

这种形式存在 48 个不同的矩阵表示，其中一个矩阵表示标量部分，其他三个都是斜对称的。 更准确地说，有 48 组具有这些对称约束的矩阵四元组，使得将 1、i、j 和 k 发送到四元组中的矩阵的函数是同态的，也就是说，它将四元数的和和乘积发送到和 和矩阵的产品。[34] 在这种表示中，四元数的共轭对应于矩阵的转置。 四元数范数的四次方是对应矩阵的行列式。 与上面的 2 × 2 复数表示一样，可以通过适当地约束系数再次生成复数； 例如，通过设置 c = d = 0 作为具有两个 2 × 2 块的块对角矩阵。

Each 4×4 matrix representation of quaternions corresponds to a multiplication table of unit quaternions. For example, the last matrix representation given above corresponds to the multiplication table

四元数的每个 4×4 矩阵表示对应于单位四元数的乘法表。 例如，上面给出的最后一个矩阵表示对应于乘法表

|×|a|d|−b|−c|
|---|---|---|---|----|
|a|a|d|−b|−c|
|−d|−d|a|c|−b|
|b|b|−c|a|−d|
|c|c|b|d|a|

which is isomorphic — through $${\displaystyle \{a\mapsto 1,b\mapsto i,c\mapsto j,d\mapsto k\}}$$ — to

这是同构的 - 通过 $${\displaystyle \{a\mapsto 1,b\mapsto i,c\mapsto j,d\mapsto k\}}$$ - 到

|×|1|k|−i|−j|
|---|---|---|---|---|
|1|1|k|−i|−j|
|−k|−k|1|j|−i|
|i|i|−j|1|−k|
|j|j|i|k|1|

Constraining any such multiplication table to have the identity in the first row and column and for the signs of the row headers to be opposite to those of the column headers, then there are 3 possible choices for the second column (ignoring sign), 2 possible choices for the third column (ignoring sign), and 1 possible choice for the fourth column (ignoring sign); that makes 6 possibilities. Then, the second column can be chosen to be either positive or negative, the third column can be chosen to be positive or negative, and the fourth column can be chosen to be positive or negative, giving 8 possibilities for the sign. Multiplying the possibilities for the letter positions and for their signs yields 48. Then replacing 1 with a, i with b, j with c, and k with d and removing the row and column headers yields a matrix representation of a + b i + c j + d k .

约束任何这样的乘法表在第一行和第一列中具有同一性，并且行标题的符号与列标题的符号相反，那么第二列有 3 种可能的选择（忽略符号），2 种可能 第三列的选择（忽略符号），第四列的一个可能选择（忽略符号）； 这产生了 6 种可能性。 然后，第二列可以选择为正或负，第三列可以选择为正或负，第四列可以选择为正或负，给出8种可能的符号。 将字母位置及其符号的可能性相乘得到 48。然后将 1 替换为 a，将 i 替换为 b，将 j 替换为 c，将 k 替换为 d，并删除行和列标题，得到 a + bi + cj + 的矩阵表示。

# Lagrange’s four-square theorem  拉格朗日四平方定理

*Main article: Lagrange's four-square theorem*

*主条目：拉格朗日四平方定理*

Quaternions are also used in one of the proofs of Lagrange's four-square theorem in number theory, which states that every nonnegative integer is the sum of four integer squares. As well as being an elegant theorem in its own right, Lagrange's four square theorem has useful applications in areas of mathematics outside number theory, such as combinatorial design theory. The quaternion-based proof uses Hurwitz quaternions, a subring of the ring of all quaternions for which there is an analog of the Euclidean algorithm.

四元数也用于数论中拉格朗日四平方定理的证明之一，该定理指出每个非负整数都是四个整数平方的和。 拉格朗日四平方定理本身不仅是一个优雅的定理，而且在数论之外的数学领域也有有用的应用，例如组合设计理论。 基于四元数的证明使用 Hurwitz 四元数，它是所有四元数环的一个子环，其中有一个欧几里得算法的类似物。

# Quaternions as pairs of complex numbers  四元数作为复数对

*Main article: Cayley–Dickson construction*

*主条目：Cayley-Dickson 构造*

Quaternions can be represented as pairs of complex numbers. From this perspective, quaternions are the result of applying the Cayley–Dickson construction to the complex numbers. This is a generalization of the construction of the complex numbers as pairs of real numbers.

四元数可以表示为复数对。 从这个角度来看，四元数是将 Cayley-Dickson 构造应用于复数的结果。 这是将复数构造为实数对的概括。

Let $${\displaystyle \mathbb {C} ^{2}}$$ be a two-dimensional vector space over the complex numbers. Choose a basis consisting of two elements 1 and j. A vector in $${\displaystyle \mathbb {C} ^{2}}$$ can be written in terms of the basis elements 1 and j as

令 $${\displaystyle \mathbb {C} ^{2}}$$ 是复数上的二维向量空间。 选择一个由两个元素 1 和 j 组成的基。 $${\displaystyle \mathbb {C} ^{2}}$$ 中的向量可以写成基元素 1 和 j 为

$$
{\displaystyle (a+bi)1+(c+di)\mathbf {j} \,.}
$$

If we define j2 = −1 and i j = −j i, then we can multiply two vectors using the distributive law. Using k as an abbreviated notation for the product i j leads to the same rules for multiplication as the usual quaternions. Therefore, the above vector of complex numbers corresponds to the quaternion a + b i + c j + d k . If we write the elements of $${\displaystyle \mathbb {C} ^{2}}$$ as ordered pairs and quaternions as quadruples, then the correspondence is

如果我们定义 j2 = -1 和 i j = -j i，那么我们可以使用分配定律将两个向量相乘。 使用 k 作为乘积 i j 的缩写符号会导致与通常的四元数相同的乘法规则。 因此，上述复数向量对应于四元数 a + b i + c j + d k 。 如果我们将 $${\displaystyle \mathbb {C} ^{2}}$$ 的元素写成有序对，四元数写成四元数，那么对应关系是

$$
{\displaystyle (a+bi,\ c+di)\leftrightarrow (a,b,c,d).}
$$

# Square roots  平方根

## Square roots of −1    -1的平方根

In the complex numbers, $${\displaystyle \mathbb {C} ,}$$ there are just two numbers, i and −i, whose square is −1 . In $${\displaystyle \mathbb {H} }$$  there are infinitely many square roots of minus one: the quaternion solution for the square root of −1 is the unit sphere in $${\displaystyle \mathbb {R} ^{3}.}$$ To see this, let q = a + b i + c j + d k be a quaternion, and assume that its square is −1. In terms of a, b, c, and d, this means

在复数 $${\displaystyle \mathbb {C} ,}$$ 中只有两个数 i 和 -i，它们的平方是 -1 。 在 $${\displaystyle \mathbb {H} }$$ 中有无穷多个负一的平方根：-1 平方根的四元数解是 $${\displaystyle \mathbb {R} 中的单位球 ^ {3}.}$$ 要看到这一点，让 q = a + bi + cj + dk 是一个四元数，并假设它的平方为 -1。 就 a、b、c 和 d 而言，这意味着

$$
{\displaystyle a^{2}-b^{2}-c^{2}-d^{2}=-1,}
$$

$$
{\displaystyle 2ab=0,}
$$

$$
{\displaystyle 2ac=0,}
$$

$$
{\displaystyle 2ad=0.}
$$

To satisfy the last three equations, either a = 0 or b, c, and d are all 0. The latter is impossible because a is a real number and the first equation would imply that a2 = −1. Therefore, a = 0 and b2 + c2 + d2 = 1. In other words: A quaternion squares to −1 if and only if it is a vector quaternion with norm 1. By definition, the set of all such vectors forms the unit sphere.

要满足最后三个方程，要么 a = 0，要么 b、c 和 d 都为 0。后者是不可能的，因为 a 是实数，而第一个方程意味着 a2 = -1。 因此，a = 0 和 b2 + c2 + d2 = 1。换句话说：当且仅当它是范数为 1 的向量四元数时，四元数平方为 -1。根据定义，所有此类向量的集合形成单位球体 .

Only negative real quaternions have infinitely many square roots. All others have just two (or one in the case of 0).[citation needed][d]

只有负实数四元数有无穷多个平方根。 所有其他人只有两个（或在 0 的情况下一个）。[需要引用][d]

## As a union of complex planes  作为复平面的联合

Each pair of square roots of −1 creates a distinct copy of the complex numbers inside the quaternions. If q2 = −1, then the copy is determined by the function

每对 -1 的平方根在四元数内创建一个复数的不同副本。 如果 q2 = -1，则副本由函数确定

$$
{\displaystyle a+b{\sqrt {-1\,}}\mapsto a+bq\,.}
$$

This is an injective ring homomorphism from $${\displaystyle \mathbb {C} }$$  to $${\displaystyle \mathbb {H} ,}$$ which defines a field isomorphism from $${\displaystyle \mathbb {C} }$$  onto its image. The images of the embeddings corresponding to q and −q are identical.

这是一个从 $${\displaystyle \mathbb {C} }$$ 到 $${\displaystyle \mathbb {H} ,}$$ 的单射环同态，它定义了从 $${\displaystyle \mathbb {C } }$$ 到它的图像上。 对应于 q 和 -q 的嵌入的图像是相同的。

Every non-real quaternion generates a subalgebra of the quaternions that is isomorphic to $${\displaystyle \mathbb {C} ,}$$ and is thus a planar subspace of $${\displaystyle \mathbb {H} \colon }$$ write q as the sum of its scalar part and its vector part:

每个非实数四元数生成一个四元数的子代数，它与 $${\displaystyle \mathbb {C} ,}$$ 同构，因此是 $${\displaystyle \mathbb {H} \colon }$$ 的平面子空间将 q 写为其标量部分和向量部分之和：

$$
{\displaystyle q=q_{s}+{\vec {q}}_{v}.}
$$

Decompose the vector part further as the product of its norm and its versor:

将向量部分进一步分解为其范数及其倒数的乘积：

$$
{\displaystyle q=q_{s}+\lVert {\vec {q}}_{v}\rVert \cdot \mathbf {U} {\vec {q}}_{v}=q_{s}+{\frac {q_{v}}{\|q_{v}\|}}.}
$$

(Note that this is not the same as $${\displaystyle q_{s}+\lVert q\rVert \cdot \mathbf {U} q}$$ The versor of the vector part of q, $${\displaystyle \mathbf {U} {\vec {q}}_{v}}$$, is a right versor with –1 as its square. A straightforward verification shows that

（注意这和 $${\displaystyle q_{s}+\lVert q\rVert \cdot \mathbf {U} q}$$ q的向量部分的倒数， $${\displaystyle \mathbf {U} {\vec {q}}_{v}}$$, 是一个以 –1 为平方的右 versor。一个简单的验证表明

$$
{\displaystyle a+b{\sqrt {-1\,}}\mapsto a+b\mathbf {U} {\vec {q}}_{v}}
$$

defines an injective homomorphism of normed algebras from $${\displaystyle \mathbb {C} }$$  into the quaternions. Under this homomorphism, q is the image of the complex number $${\displaystyle q_{s}+\lVert {\vec {q}}_{v}\rVert i}$$.

定义了从 $${\displaystyle \mathbb {C} }$$ 到四元数的范数的单射同态。 在这种同态下，q 是复数 $${\displaystyle q_{s}+\lVert {\vec {q}}_{v}\rVert i}$$ 的图像。

As $${\displaystyle \mathbb {H} }$$  is the union of the images of all these homomorphisms, this allows viewing the quaternions as a union of complex planes intersecting on the real line. Each of these complex planes contains exactly one pair of antipodal points of the sphere of square roots of minus one.

由于 $${\displaystyle \mathbb {H} }$$ 是所有这些同态的图像的并集，因此可以将四元数视为在实线上相交的复平面的并集。 这些复平面中的每一个都恰好包含负一平方根球面的一对对映点。

## Commutative subrings  交换子环

The relationship of quaternions to each other within the complex subplanes of $${\displaystyle \mathbb {H} }$$  can also be identified and expressed in terms of commutative subrings. Specifically, since two quaternions p and q commute (i.e., p q = q p) only if they lie in the same complex subplane of $${\displaystyle \mathbb {H} }$$ , the profile of $${\displaystyle \mathbb {H} }$$  as a union of complex planes arises when one seeks to find all commutative subrings of the quaternion ring.

$${\displaystyle \mathbb {H} }$$  的复子平面内四元数之间的关系也可以用交换子环来识别和表达。 具体来说，由于两个四元数 p 和 q 仅当它们位于 $${\displaystyle \mathbb {H} }$$ 的同一个复子平面中时才可对易（即 pq = qp），$${\displaystyle \mathbb {H} }$$  作为复平面的并集出现在寻找四元数环的所有可交换子环时。

## Square roots of arbitrary quaternions  任意四元数的平方根

Any quaternion $${\displaystyle \mathbf {q} =(r,\,{\vec {v}})}$$ (represented here in scalar–vector representation) has at least one square root $${\displaystyle {\sqrt {\mathbf {q} }}=(x,\,{\vec {y}})}$$ which solves the equation $${\displaystyle {\sqrt {\mathbf {q} }}^{2}=(x,\,{\vec {y}})^{2}=\mathbf {q} }$$. Looking at the scalar and vector parts in this equation separately yields two equations, which when solved gives the solutions

任何四元数 $${\displaystyle \mathbf {q} =(r,\,{\vec {v}})}$$（这里以标量-矢量表示）至少有一个平方根 $${\displaystyle { \sqrt {\mathbf {q} }}=(x,\,{\vec {y}})}$$ 求解方程 $${\displaystyle {\sqrt {\mathbf {q} }}^{2 }=(x,\,{\vec {y}})^{2}=\mathbf {q} }$$。 分别查看该方程中的标量和矢量部分会产生两个方程，求解时会给出解

$$
{\displaystyle {\sqrt {\mathbf {q} }}={\sqrt {(r,\,{\vec {v}}\,)}}=\pm \left({\sqrt {\frac {\|\mathbf {q} \|+r}{2}}},\ {\frac {\vec {v}}{\|{\vec {v}}\|}}{\sqrt {\frac {\|\mathbf {q} \|-r}{2}}}\right),}
$$

where $${\displaystyle \|{\vec {v}}\|={\sqrt { {\vec {v} }\cdot {\vec {v}}}}={\sqrt {-{\vec {v}}^{2}}}}$$ is the norm of $${\displaystyle {\vec {v}}}$$ and $${\displaystyle \|\mathbf {q} \|={\sqrt {\mathbf {q} ^{*}\mathbf {q} }}=r^{2}+\|{\vec {v}}\|^{2}}$$ is the norm of $${\displaystyle \mathbf {q} }$$ . For any scalar quaternion $${\displaystyle \mathbf {q} }$$, this equation provides the correct square roots if $${\displaystyle {\frac {\vec {v}}{\|{\vec {v}}\|}}}$$ is interpreted as an arbitrary unit vector.

其中 $${\displaystyle \|{\vec {v}}\|={\sqrt { {\vec {v} }\cdot {\vec {v}}}}={\sqrt {-{\vec { v}}^{2}}}}$$ 是 $${\displaystyle {\vec {v}}}$$ 和 $${\displaystyle \|\mathbf {q} \|={\sqrt 的范数 {\mathbf {q} ^{*}\mathbf {q} }}=r^{2}+\|{\vec {v}}\|^{2}}$$ 是 $${\ 显示风格 \mathbf {q} }$$ 。 对于任何标量四元数 $${\displaystyle \mathbf {q} }$$，如果 $${\displaystyle {\frac {\vec {v}}{\|{\vec {v} }\|}}}$$ 被解释为任意单位向量。

Therefore, non-zero, non-scalar quaternions, or positive scalar quaternions, have exactly two roots, while 0 has exactly one root (0), and negative scalar quaternions have infinitely many roots, which are the vector quaternions located on $${\displaystyle \{0\}\times S^{2}({\sqrt {-r}})}$$, i.e., where the scalar part is zero and the vector part is located on the 2-sphere with radius $${\displaystyle {\sqrt {-r}}}$$.

因此，非零、非标量四元数或正标量四元数正好有两个根，而 0 正好有一个根 (0)，负标量四元数有无穷多个根，即位于 $${ 上的向量四元数 \displaystyle \{0\}\times S^{2}({\sqrt {-r}})}$$，即标量部分为零，向量部分位于半径为$的2-球体上 ${\displaystyle {\sqrt {-r}}}$$。

# Functions of a quaternion variable  四元变量的函数

*Main article: Quaternionic analysis*

*主条目：四元离子分析*

![](图片/16.jpg)

>- The Julia sets and Mandelbrot sets can be extended to the Quaternions, but they must use cross sections to be rendered visually in 3 dimensions. This Julia set is cross sectioned at the x y plane.  
Julia 集和 Mandelbrot 集可以扩展到四元数，但它们必须使用横截面才能在 3 维视觉上呈现。 这个 Julia 集在 x y 平面上进行横截面。

Like functions of a complex variable, functions of a quaternion variable suggest useful physical models. For example, the original electric and magnetic fields described by Maxwell were functions of a quaternion variable. Examples of other functions include the extension of the Mandelbrot set and Julia sets into 4-dimensional space.[36]

与复变量的函数一样，四元数变量的函数提出了有用的物理模型。 例如，麦克斯韦描述的原始电场和磁场是四元数变量的函数。 其他函数的示例包括将 Mandelbrot 集和 Julia 集扩展到 4 维空间。 [36]

## Exponential, logarithm, and power functions  指数、对数和幂函数

Given a quaternion,

给定一个四元数，

$$
{\displaystyle q=a+b\mathbf {i} +c\mathbf {j} +d\mathbf {k} =a+\mathbf {v} }
$$

the exponential is computed as[37]

指数计算为[37]

$$
{\displaystyle \exp(q)=\sum _{n=0}^{\infty }{\frac {q^{n}}{n!}}=e^{a}\left(\cos \|\mathbf {v} \|+{\frac {\mathbf {v} }{\|\mathbf {v} \|}}\sin \|\mathbf {v} \|\right)~~}
$$

and the logarithm is[37]

对数是[37]

$$
{\displaystyle \ln(q)=\ln \|q\|+{\frac {\mathbf {v} }{\|\mathbf {v} \|}}\arccos {\frac {a}{\|q\|}}~~}
$$

It follows that the polar decomposition of a quaternion may be written

由此可见，四元数的极分解可以写成

$$
{\displaystyle q=\|q\|e^{ {\hat {n} }\varphi }=\|q\|\left(\cos(\varphi )+{\hat {n}}\sin(\varphi )\right),}
$$

where the angle $${\displaystyle \varphi } [e]$$

其中角度 $${\displaystyle \varphi } [e]$$

$$
{\displaystyle a=\|q\|\cos(\varphi )}
$$

and the unit vector $${\displaystyle {\hat {n}}}$$ is defined by:

单位向量 $${\displaystyle {\hat {n}}}$$ 定义为：

$$
{\displaystyle \mathbf {v} ={\hat {n}}\|\mathbf {v} \|={\hat {n}}\|q\|\sin(\varphi )\,.}
$$

Any unit quaternion may be expressed in polar form as:

任何单位四元数都可以用极性形式表示为：

$$
{\displaystyle q=\exp {({\hat {n}}\varphi )}}.
$$

The power of a quaternion raised to an arbitrary (real) exponent x is given by:

提高到任意（实）指数 x 的四元数的幂由下式给出：

$$
{\displaystyle q^{x}=\|q\|^{x}e^{ {\hat {n} }x\varphi }=\|q\|^{x}\left(\cos(x\varphi )+{\hat {n}}\,\sin(x\varphi )\right)~.}
$$

## Geodesic norm  测地线范数

The geodesic distance dg(p, q) between unit quaternions p and q is defined as:

单位四元数 p 和 q 之间的测地线距离 dg(p, q) 定义为：

$$
{\displaystyle d_{\text{g}}(p,q)=\lVert \ln(p^{-1}q)\rVert .}[39]
$$

and amounts to the absolute value of half the angle subtended by p and q along a great arc of the S3 sphere. This angle can also be computed from the quaternion dot product without the logarithm as:

并且等于沿 S3 球体的大弧线的 p 和 q 对角的一半的绝对值。 这个角度也可以从没有对数的四元数点积计算为：

$$
{\displaystyle \arccos(2(p\cdot q)^{2}-1).}
$$

# Three-dimensional and four-dimensional rotation groups  三维和四维旋转组

*Main articles: Quaternions and spatial rotation and Rotation operator (vector space)*

*主要文章：四元数和空间旋转和旋转算子（向量空间）*

The word "conjugation", besides the meaning given above, can also mean taking an element a to r a r−1 where r is some non-zero quaternion. All elements that are conjugate to a given element (in this sense of the word conjugate) have the same real part and the same norm of the vector part. (Thus the conjugate in the other sense is one of the conjugates in this sense.)

“共轭”这个词，除了上面给出的含义外，还可以表示将元素 a 变为 rar-1，其中 r 是某个非零四元数。 与给定元素共轭的所有元素（在这个词共轭的意义上）具有相同的实部和向量部分的相同范数。 （因此，另一种意义上的共轭是这种意义上的共轭之一。）

>**[warning]**  
**rar-1**:?

Thus the multiplicative group of non-zero quaternions acts by conjugation on the copy of $${\displaystyle \mathbb {R} ^{3}}$$ consisting of quaternions with real part equal to zero. Conjugation by a unit quaternion (a quaternion of absolute value 1) with real part cos(φ) is a rotation by an angle 2φ, the axis of the rotation being the direction of the vector part. The advantages of quaternions are:

因此，非零四元数的乘法群通过共轭作用于由实部为零的四元数组成的 $${\displaystyle \mathbb {R} ^{3}}$$ 的副本。 单位四元数（绝对值为 1 的四元数）与实部 cos(φ) 的共轭是角度 2φ 的旋转，旋转的轴是矢量部分的方向。 四元数的优点是：

- Avoiding gimbal lock, a problem with systems such as Euler angles.  
避免万向节锁定，这是欧拉角等系统的问题。

>**[warning]**  
**万向节锁定**：？

- Faster and more compact than matrices.  
比矩阵更快、更紧凑。

- Nonsingular representation (compared with Euler angles for example).  
非奇异表示（例如与欧拉角相比）。

>**[warning]**  
**非奇异表示**：？

- Pairs of unit quaternions represent a rotation in 4D space (see Rotations in 4-dimensional Euclidean space: Algebra of 4D rotations).  
成对的单位四元数表示 4D 空间中的旋转（请参阅 4 维欧几里得空间中的旋转：4D 旋转的代数）。

The set of all unit quaternions (versors) forms a 3-sphere S3 and a group (a Lie group) under multiplication, double covering the group SO(3,ℝ) of real orthogonal 3×3 matrices of determinant 1 since two unit quaternions correspond to every rotation under the above correspondence. See the plate trick.

所有单位四元数（versors）的集合在乘法下形成一个 3 球 S3 和一个群（李群），双重覆盖行列式 1 的实正交 3×3 矩阵的群 SO(3,ℝ)，因为两个单位四元数 对应于上述对应关系下的每一次旋转。 看盘子戏法。

*Further information: Point groups in three dimensions*

*更多信息：三个维度的点群*

The image of a subgroup of versors is a point group, and conversely, the preimage of a point group is a subgroup of versors. The preimage of a finite point group is called by the same name, with the prefix binary. For instance, the preimage of the icosahedral group is the binary icosahedral group.

一个对视子群的图像是一个点群，反之，一个点群的原像是一个对视子群。 有限点群的原像被称为同名，前缀为二进制。 例如，二十面体群的原像是二元二十面体群。

The versors' group is isomorphic to SU(2), the group of complex unitary 2×2 matrices of determinant 1.

versors 群与 SU(2) 同构，SU(2) 是行列式 1 的复酉 2×2 矩阵群。

Let A be the set of quaternions of the form a + b i + c j + d k where a, b, c, and d are either all integers or all half-integers. The set A is a ring (in fact a domain) and a lattice and is called the ring of Hurwitz quaternions. There are 24 unit quaternions in this ring, and they are the vertices of a regular 24 cell with Schläfli symbol {3,4,3}. They correspond to the double cover of the rotational symmetry group of the regular tetrahedron. Similarly, the vertices of a regular 600 cell with Schläfli symbol {3,3,5} can be taken as the unit icosians, corresponding to the double cover of the rotational symmetry group of the regular icosahedron. The double cover of the rotational symmetry group of the regular octahedron corresponds to the quaternions that represent the vertices of the disphenoidal 288-cell.

令 A 为 a + b i + c j + d k 形式的四元数集合，其中 a、b、c 和 d 要么全是整数，要么全是半整数。 集合 A 是一个环（实际上是一个域）和一个格，称为 Hurwitz 四元数环。 该环中有 24 个单位四元数，它们是具有 Schläfli 符号 {3,4,3} 的常规 24 单元的顶点。 它们对应于正四面体的旋转对称群的双覆盖。 类似地，具有 Schläfli 符号 {3,3,5} 的规则 600 单元的顶点可以作为单位 icosians，对应于规则二十面体的旋转对称群的双覆盖。 正八面体的旋转对称群的双覆盖对应于代表二蝶形 288 单元顶点的四元数。

# Quaternion algebras  四元数代数

*Main article: Quaternion algebra*

*主条目：四元数代数*

The Quaternions can be generalized into further algebras called quaternion algebras. Take F to be any field with characteristic different from 2, and a and b to be elements of F; a four-dimensional unitary associative algebra can be defined over F with basis 1, i, j, and i j, where i2 = a, j2 = b and i j = −j i (so (i j)2 = −a b).

四元数可以推广成更进一步的代数，称为四元数代数。 取 F 为特征不同于 2 的任意场，a 和 b 为 F 的元素； 可以在 F 上定义一个四维酉关联代数，基为 1、i、j 和 i j，其中 i2 = a，j2 = b 和 i j = -j i (so (i j)2 = -a b)。

Quaternion algebras are isomorphic to the algebra of 2×2 matrices over F or form division algebras over F, depending on the choice of a and b.

四元数代数同构于 F 上的 2×2 矩阵的代数或形成 F 上的除法代数，这取决于 a 和 b 的选择。

# Quaternions as the even part of Cl3,0(ℝ)  四元数作为 Cl3,0(ℝ) 的偶数部分

*Main article: Spinor § Three dimensions*

*主条目：旋量§三维*

The usefulness of quaternions for geometrical computations can be generalised to other dimensions by identifying the quaternions as the even part $${\displaystyle \operatorname {Cl} _{3,0}^{+}(\mathbb {R} )}$$ of the Clifford algebra $${\displaystyle \operatorname {Cl} _{3,0}(\mathbb {R} ).}$$ This is an associative multivector algebra built up from fundamental basis elements σ1, σ2, σ3 using the product rules

通过将四元数识别为偶数部分 $${\displaystyle \operatorname {Cl} _{3,0}^{+}(\mathbb {R} )}$，可以将四元数对几何计算的有用性推广到其他维度 克利福德代数 $${\displaystyle \operatorname {Cl} _{3,0}(\mathbb {R} ).}$$ 这是一个结合多向量代数，由基本基元 σ1、σ2、σ3 组成，使用 产品规则

$$
{\displaystyle \sigma _{1}^{2}=\sigma _{2}^{2}=\sigma _{3}^{2}=1,}
$$

$$
{\displaystyle \sigma _{i}\sigma _{j}=-\sigma _{j}\sigma _{i}\qquad (j\neq i).}
$$

If these fundamental basis elements are taken to represent vectors in 3D space, then it turns out that the reflection of a vector r in a plane perpendicular to a unit vector w can be written:

如果用这些基本基元来表示 3D 空间中的向量，那么向量 r 在垂直于单位向量 w 的平面中的反射可以写成：

$$
{\displaystyle r^{\prime }=-w\,r\,w.}
$$

Two reflections make a rotation by an angle twice the angle between the two reflection planes, so

两个反射以两个反射平面之间角度的两倍旋转，所以

$$
{\displaystyle r^{\prime \prime }=\sigma _{2}\sigma _{1}\,r\,\sigma _{1}\sigma _{2}}
$$

corresponds to a rotation of 180° in the plane containing σ1 and σ2. This is very similar to the corresponding quaternion formula,

对应于在包含 σ1 和 σ2 的平面中旋转 180°。 这与对应的四元数公式非常相似，

$$
{\displaystyle r^{\prime \prime }=-\mathbf {k} \,r\,\mathbf {k} .}
$$

In fact, the two are identical, if we make the identification

其实两者是一样的，如果我们做鉴定

$$
{\displaystyle \mathbf {k} =\sigma _{2}\sigma _{1}\,,\quad \mathbf {i} =\sigma _{3}\sigma _{2}\,,\quad \mathbf {j} =\sigma _{1}\sigma _{3}\,,}
$$

and it is straightforward to confirm that this preserves the Hamilton relations

并且很容易确认这保留了Hamilton关系

$$
{\displaystyle \mathbf {i} ^{2}=\mathbf {j} ^{2}=\mathbf {k} ^{2}=\mathbf {i\,j\,k} =-1~.}
$$

In this picture, so-called "vector quaternions" (that is, pure imaginary quaternions) correspond not to vectors but to bivectors – quantities with magnitude and orientations associated with particular 2D planes rather than 1D directions. The relation to complex numbers becomes clearer, too: in 2D, with two vector directions σ1 and σ2, there is only one bivector basis element σ1σ2, so only one imaginary. But in 3D, with three vector directions, there are three bivector basis elements σ1σ2, σ2σ3, σ3σ1, so three imaginaries.

在这张图片中，所谓的“向量四元数”（即纯虚数四元数）对应的不是向量而是双向量——具有与特定 2D 平面而非 1D 方向相关联的大小和方向的量。 与复数的关系也变得更加清晰：在二维中，有两个向量方向 σ1 和 σ2，只有一个双向量基元 σ1σ2，所以只有一个虚数。 但在 3D 中，具有三个向量方向，存在三个双向量基元 σ1σ2、σ2σ3、σ3σ1，因此三个虚数。

This reasoning extends further. In the Clifford algebra $${\displaystyle \operatorname {Cl} _{4,0}(\mathbb {R} ),}$$ there are six bivector basis elements, since with four different basic vector directions, six different pairs and therefore six different linearly independent planes can be defined. Rotations in such spaces using these generalisations of quaternions, called rotors, can be very useful for applications involving homogeneous coordinates. But it is only in 3D that the number of basis bivectors equals the number of basis vectors, and each bivector can be identified as a pseudovector.

这个推理进一步延伸。 在克利福德代数 $${\displaystyle \operatorname {Cl} _{4,0}(\mathbb {R} ),}$$ 中有六个双向量基元素，因为有四个不同的基本向量方向，六个不同的对和 因此可以定义六个不同的线性独立平面。 使用这些四元数的推广（称为转子）在此类空间中的旋转对于涉及齐次坐标的应用非常有用。 但是只有在 3D 中，基双向量的数量才等于基向量的数量，并且每个双向量都可以被识别为伪向量。

There are several advantages for placing quaternions in this wider setting:[40]

在这种更广泛的设置中放置四元数有几个优点：[40]

- Rotors are a natural part of geometric algebra and easily understood as the encoding of a double reflection.  
转子是几何代数的自然组成部分，很容易理解为双反射的编码。

- In geometric algebra, a rotor and the objects it acts on live in the same space. This eliminates the need to change representations and to encode new data structures and methods, which is traditionally required when augmenting linear algebra with quaternions.  
在几何代数中，转子和它作用的物体存在于同一个空间中。 这消除了更改表示和编码新的数据结构和方法的需要，而这在使用四元数增强线性代数时是传统上需要的。

- Rotors are universally applicable to any element of the algebra, not just vectors and other quaternions, but also lines, planes, circles, spheres, rays, and so on.  
转子普遍适用于代数的任何元素，不仅适用于向量和其他四元数，还适用于线、平面、圆、球体、射线等。

- In the conformal model of Euclidean geometry, rotors allow the encoding of rotation, translation and scaling in a single element of the algebra, universally acting on any element. In particular, this means that rotors can represent rotations around an arbitrary axis, whereas quaternions are limited to an axis through the origin.  
在欧几里得几何的共形模型中，转子允许在代数的单个元素中对旋转、平移和缩放进行编码，普遍作用于任何元素。 特别是，这意味着转子可以表示围绕任意轴的旋转，而四元数仅限于通过原点的轴。

- Rotor-encoded transformations make interpolation particularly straightforward.  
转子编码变换使插值特别简单。

- Rotors carry over naturally to pseudo-Euclidean spaces, for example, the Minkowski space of special relativity. In such spaces rotors can be used to efficiently represent Lorentz boosts, and to interpret formulas involving the gamma matrices.  
转子自然地延续到伪欧几里得空间，例如狭义相对论的 Minkowski 空间。 在这样的空间中，转子可以用来有效地表示洛伦兹增强，并解释涉及伽马矩阵的公式。

For further detail about the geometrical uses of Clifford algebras, see Geometric algebra.  
有关 Clifford 代数的几何用途的更多详细信息，请参阅几何代数。

# Brauer group  布劳尔集团

*Further information: Brauer group*

*更多信息：布劳尔集团*

The quaternions are "essentially" the only (non-trivial) central simple algebra (CSA) over the real numbers, in the sense that every CSA over the real numbers is Brauer equivalent to either the real numbers or the quaternions. Explicitly, the Brauer group of the real numbers consists of two classes, represented by the real numbers and the quaternions, where the Brauer group is the set of all CSAs, up to equivalence relation of one CSA being a matrix ring over another. By the Artin–Wedderburn theorem (specifically, Wedderburn's part), CSAs are all matrix algebras over a division algebra, and thus the quaternions are the only non-trivial division algebra over the real numbers.

四元数“本质上”是实数上唯一的（非平凡的）中心简单代数（CSA），因为实数上的每个 CSA 都是 Brauer 等价于实数或四元数。 明确地，实数的 Brauer 群由两个类组成，由实数和四元数表示，其中 Brauer 群是所有 CSA 的集合，直到一个 CSA 是另一个矩阵环的等价关系。 根据 Artin-Wedderburn 定理（特别是 Wedderburn 的部分），CSA 都是除法代数上的矩阵代数，因此四元数是实数上唯一的非平凡除法代数。

CSAs – rings over a field, which are simple algebras (have no non-trivial 2-sided ideals, just as with fields) whose center is exactly the field – are a noncommutative analog of extension fields, and are more restrictive than general ring extensions. The fact that the quaternions are the only non-trivial CSA over the real numbers (up to equivalence) may be compared with the fact that the complex numbers are the only non-trivial field extension of the real numbers.

CSA – 域上的环，它是简单的代数（没有非平凡的 2 边理想，就像域一样），其中心正好是域 – 是扩展域的非交换模拟，并且比一般环扩展更具限制性 . 四元数是实数上唯一的非平凡 CSA（直到等价）这一事实可以与复数是实数的唯一非平凡域扩展的事实相比较。

# Quotations  报价单

I regard it as an inelegance, or imperfection, in quaternions, or rather in the state to which it has been hitherto unfolded, whenever it becomes or seems to become necessary to have recourse to x, y, z, etc.

我认为它是四元数中的不雅或不完美，或者更确切地说，在它迄今展开的状态中，每当它变得或似乎变得有必要求助于 x、y、z 等时。

— William Rowan Hamilton[41]  
— 威廉·罗文·Hamilton[41]


Time is said to have only one dimension, and space to have three dimensions. ... The mathematical quaternion partakes of both these elements; in technical language it may be said to be "time plus space", or "space plus time": and in this sense it has, or at least involves a reference to, four dimensions. And how the One of Time, of Space the Three, Might in the Chain of Symbols girdled be.

据说时间只有一个维度，而空间则有三个维度。 ... 数学四元数包含这两个元素； 用技术语言来说，它可以说是“时间加空间”或“空间加时间”：从这个意义上说，它具有或至少涉及到四个维度。 以及时间之一，空间之三，在符号链中的力量如何。

— William Rowan Hamilton[42][full citation needed]  
— 威廉·罗文·Hamilton[42][需要完整引用]

Quaternions came from Hamilton after his really good work had been done; and, though beautifully ingenious, have been an unmixed evil to those who have touched them in any way, including Clerk Maxwell.

四元数来自Hamilton，是在他完成了非常出色的工作之后。 并且，虽然非常巧妙，但对于那些以任何方式接触过它们的人来说，这都是一种纯粹的邪恶，包括 Clerk Maxwell。

— W. Thompson, Lord Kelvin (1892)[citation needed]  
— W.汤普森，开尔文勋爵（1892）[需要引证]

I came later to see that, as far as the vector analysis I required was concerned, the quaternion was not only not required, but was a positive evil of no inconsiderable magnitude; and that by its avoidance the establishment of vector analysis was made quite simple and its working also simplified, and that it could be conveniently harmonised with ordinary Cartesian work.

后来我发现，就我需要的向量分析而言，四元数不仅不是必需的，而且是一个不可忽视的积极因素； 并且通过避免矢量分析的建立变得非常简单，并且它的工作也简化了，并且它可以方便地与普通的笛卡尔工作相协调。

— Oliver Heaviside (1893)[43]  
— 奥利弗·赫维赛德 (1893)[43]

Neither matrices nor quaternions and ordinary vectors were banished from these ten [additional] chapters. For, in spite of the uncontested power of the modern Tensor Calculus, those older mathematical languages continue, in my opinion, to offer conspicuous advantages in the restricted field of special relativity. Moreover, in science as well as in everyday life, the mastery of more than one language is also precious, as it broadens our views, is conducive to criticism with regard to, and guards against hypostasy [weak-foundation] of, the matter expressed by words or mathematical symbols.

矩阵、四元数和普通向量都没有从这十个[附加]章节中删除。 因为，尽管现代张量微积分具有无可争议的力量，但在我看来，那些较旧的数学语言继续在狭义相对论的有限领域提供显着优势。 而且，在科学和日常生活中，掌握一种以上的语言也是很宝贵的，因为它可以开阔我们的视野，有利于对所表达的事物进行批评和提防。 通过文字或数学符号。

— Ludwik Silberstein (1924)[44][full citation needed]  
— Ludwik Silberstein (1924)[44][需要完整引用]

... quaternions appear to exude an air of nineteenth century decay, as a rather unsuccessful species in the struggle-for-life of mathematical ideas. Mathematicians, admittedly, still keep a warm place in their hearts for the remarkable algebraic properties of quaternions but, alas, such enthusiasm means little to the harder-headed physical scientist.

... 四元数似乎散发出 19 世纪衰败的气息，作为一个在数学思想的生存斗争中相当不成功的物种。 诚然，数学家们仍然对四元数非凡的代数性质保持着温暖的地位，但是，可惜的是，这种热情对于头脑冷静的物理科学家来说意义不大。

— Simon L. Altmann (1986)[45]  
—— 西蒙·L·奥尔特曼 (1986)[45]

# See also  另请参见

- Conversion between quaternions and Euler angles  
四元数和欧拉角之间的转换

- Dual quaternion  
双四元数

- Dual-complex number  
双复数

- Exterior algebra  
外代数

- Hurwitz quaternion order  
赫尔维茨四元数阶

- Hyperbolic quaternion  
双曲四元数

- Lénárt sphere  
Lénárt 球体

- Pauli matrices  
泡利矩阵

- Quaternionic matrix  
四元离子矩阵

- Quaternionic polytope  
四元离子多面体

- Quaternionic projective space  
四元数射影空间

- Rotations in 4-dimensional Euclidean space  
4 维欧几里得空间中的旋转


- Slerp  
斯勒普

- Split-quaternion  
分裂四元数

- Tesseract  
正方体

