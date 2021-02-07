# 两点之间的距离

## 范数距离

[范数](https://windmissing.github.io/mathematics_basic_for_ML/LinearAlgebra/norm.html)

$$
L_p(x_i, x_j) = (\sum_{l=1}^{n}|x_i^{(l)}-y_i^{(l)}|^p)^{\frac{1}{p}}
$$

p=1时，曼哈顿距离  
p=2时，欧氏距离   
p=$\inf$时，各个坐标距离的最大值  

## 余弦相似度

![](/assets/images/15.png)  

$$
\cos(\beta) = \frac{\hat v \cdot \hat w}{||\hat v||||\hat w||}
$$

# 点到平面之间的距离

点$$x_0$$到超平面$$y = w \cdot x + b$$的距离为：  
$$
dis = \frac {|w \cdot x_0 + b|}{||w||}
$$
其中$$||w||$$是$$w$$的$$L_2$$范数

# 符号距离

符号距离函数（sign distance function），简称SDF，又可以称为定向距离函数（oriented distance function），在空间中的一个有限区域上确定一个点到区域边界的距离并同时对距离的符号进行定义：点在区域边界内部为正，外部为负，位于边界上时为0。