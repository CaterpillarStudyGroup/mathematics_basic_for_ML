# 矩阵

## 矩阵乘法

$$
A_{M\times N}B_{N\times P} = C_{M\times P}
$$

- \\(AB\ne BA\\) （不满足交换律）
- \\(\left( AB \right) C=A\left( BC \right) \\) （结合律）
- \\(\left( A+B \right) C=AC+BC\\)  （分配律）

矩阵与向量相乘时，可以把向量看作是\\(M \times 1\\)的矩阵

$$
a \cdot b = a^\top b \\\\
a \times b = A^* b
$$

## 矩阵转置

转置：行列互换，用\\(A^\top\\)表示

- \\(\left( AB \right) ^T=B^TA^T\\)

## 矩阵的逆

逆矩阵：用\\(A^{-1}\\)表示，方阵才有逆矩阵  
I：单位矩阵，对角线上全1、其余元素全0的矩阵

- \\(AA^{-1}=A^{-1}A=I\\)
- \\(\left( AB \right) ^{-1}=B^{-1}A^{-1}\\)


-----------

> 本文出自CaterpillarStudyGroup，转载请注明出处。  
> https://caterpillarstudygroup.github.io/GAMES101_mdbook/