**Hessian Matrix**：是一个多元函数的二阶偏导数构成的方阵，描述了函数的局部曲率。
![](/assets/images/1.png)  
性质一：H矩阵是对称矩阵。  
性质二：  
当H是正定时，f在x处是极小值点。  
当H是负定时，f在x处是极大值点。  
当H是不定时，f在x处不是极值点。  
当H是半正定或半负定时，f在x处是可疑极值点。  

## H矩阵的病态  

[病态矩阵](https://windmissing.github.io/mathematics_basic_for_ML/LinearAlgebra/IllConditioning.html)  
以2*2的H矩阵为例，  
如果条件数小，相当于f的等高线是一组同心圆。  
如果条件数大，相当于f的等高线是一组同心椭圆。条件数越大，椭圆越扁。  