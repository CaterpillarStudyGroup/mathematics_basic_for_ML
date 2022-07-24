$$
||x||_p = (\sum_i{|x_i|^p})^{1/p},\quad p \in \Bbb R,\quad p \geq 1
$$

意义：  
一个将向量映射到非负值的函数。  
衡量从原点到点x 的距离。  

性质：

$$
\begin{aligned}
f(x) = 0 \Rightarrow  x = 0 \\
f(x+y) \leq f(x) + f(y) \\
\forall \alpha \in \Bbb R, f(\alpha x) = \alpha f(x)
\end{aligned}
$$

# 常用范数

## $L^2$范数 （欧几里得范数）

$$
||x|| = ||x||_2 = \sqrt {\sum_i{x_i}^2}
$$

意义：原点到x的欧几里得距离

## 平方$L^2$范数

$$
\sum_i{x_i}^2 = x^Tx
$$

意义：  
1. 对x中每个元素求导只取决于对应的元素  
2. 在原点附近增长十分缓慢（缺点）

## $L^1$范数

$$
||x||_1 = \sum_i |x_i|
$$

意义：  
1. 用于“零和非零元素之间的差异非常重要”的问题  
2. 作为“表示非零元素数目”的替代函数

## $L^\infty$范数

$$
||x||_\infty = max_i|x_i|
$$

意义：表示向量中具有最大幅值的元素的绝对值

## Frobenius范数

$$
||A||_F = \sqrt sum_{i,j}A_{i,j}^2
$$

类似于向量的$L^2$范数