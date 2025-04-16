P31    
### Spherical Harmonics

$$
Y_ {lm}(\theta ,\phi )= N_ {lm}P_ {lm}(\cos \theta )e^ {Im \phi }
$$

![](./assets/69-31-1.png)

$$
\begin{align*}
 x& =  \sin \theta \cos \phi \\\\
  y &  =  \sin \theta \sin \phi\\\\
  z &  = \cos\theta
\end{align*}
$$

Complex sphere integration can be approximated by quadratic polynomial：   

$$
\int\limits_{\theta =0}^{\pi } \int\limits_{\phi  =0}^{2\pi } L(\theta,\phi )Y_{lm}(\theta ,\phi )\sin \theta d\theta d\phi \approx \begin{bmatrix}
x \\\\
y \\\\
 z\\\\
1
\end{bmatrix}^TM\begin{bmatrix}
x \\\\
y \\\\
z \\\\
1
\end{bmatrix}
$$

![](./assets/69-31-3.png)

> 利用球谐函数定义了一组基，通过对球谐基的加权平均，可以组合出任意复杂的球面。       

P32    
#### Spherical Harmonics 基

![](./assets/69-32-1.png)

Spherical Harmonics, a mathematical system analogous to the Fourier transform but defined across    
the surface of a sphere. The SH functions in general are defined on imaginary numbers    

> 绿色表示正值，红色表示负值。   
每一个维度的所有基都是正交的。    
二阶导永远 0（光滑）。    

P33   
#### Spherical Harmonics Encoding

![](./assets/69-33-3.png)

![](./assets/69-33-4.png)

 
