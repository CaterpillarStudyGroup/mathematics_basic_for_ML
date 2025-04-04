# 3D变换(3D Transformation)

如果用齐次坐标来表示三维的点或向量，和二维的情况相似：

- 3D point = \\((x, y, z, 1)^{T}\\)
- 3D vector = \\((x, y, z, 0)^{T}\\)

则一个齐次坐标 \\((x, y, z, w)^{T}\\) \\((w\ne 0)\\) 表示的点为  \\(\left( \frac{x}{w},  \frac{y}{w},  \frac{z}{w} \right)\\)

## 缩放(Scale)

\\[
S\left( s_x, s_y, s_z \right) =\left( \begin{matrix}
    s_x&        0&        0&        0\\\\
    0&        s_y&        0&        0\\\\
    0&        0&        s_z&        0\\\\
    0&        0&        0&        1\\\\
\end{matrix} \right) 
\\]

## 平移(Translation)

\\[
T\left( t_x, t_y, t_z \right) =\left( \begin{matrix}
    1&        0&        0&        t_x\\\\
    0&        1&        0&        t_y\\\\
    0&        0&        1&        t_z\\\\
    0&        0&        0&        1\\\\
\end{matrix} \right) 
\\]

## 旋转(Rotation)

### 自然旋转

> **&#x1F4CC;自然旋转：** 绕着某一个坐标轴旋转。

> **&#x1F4A1;思考：** 当绕着x轴旋转时，矩阵在x轴上的坐标值是不变的，因此在变换矩阵中，与X相乘的部分，是 \\((1 ,0 , 0)\\)，绕y、z轴同理。

绕x轴旋转：

\\[
R_x\left( \alpha \right) =\left( \begin{matrix}
    1&        0&        0&        0\\\\
    0&        \cos \alpha&        -\sin \alpha&        0\\\\
    0&        \sin \alpha&        \cos \alpha&        0\\\\
    0&        0&        0&        1\\\\
\end{matrix} \right) 
\\]

绕y轴旋转：

\\[
R_y\left( \alpha \right) =\left( \begin{matrix}
    \cos \alpha&        0&        \sin \alpha&        0\\\\
    0&        1&        0&        0\\\\
    -\sin \alpha&        0&        \cos \alpha&        0\\\\
    0&        0&        0&        1\\\\
\end{matrix} \right) 
\\]

> **&#x1F4A1;思考：** 上式的变换矩阵，与x、z不同，是 \\(R_{-\theta}\\) 而不是 \\(R_{\theta}\\)，这是为什么呢？
> 
> 因为绕y旋转，如果使用 \\(R_\theta\\)，那么可以认为在计算过程中x和z坐标在变化，有 \\(\left( \begin{array}{c}
>     X'\\\\
>     Z'\\\\
> \end{array} \right) =R_{\theta}\cdot \left( \begin{array}{c}
>     X\\\\
>     Z\\\\
> \end{array} \right) =\left( \begin{matrix}
>     \cos \theta&        -\sin \theta\\\\
>     \sin \theta&        \cos \theta\\\\
> \end{matrix} \right) \left( \begin{array}{c}
>     X\\\\
>     Z\\\\
> \end{array} \right) \\) , 但是， \\(\vec{x}\times \vec{z}=-\vec{y}\\)，也就是说，使用 \\(R_\theta\\) 会导致绕y旋转是顺时针旋转，而我们约定了，旋转默认是逆时针旋转，所以需要用 \\(R_{-\theta}=\left( \begin{matrix}
>     \cos \theta&        \sin \theta\\\\
>     -\sin \theta&        \cos \theta\\\\
> \end{matrix} \right) \\)

绕z轴旋转：

\\[
R_z\left( \alpha \right) =\left( \begin{matrix}
    \cos \alpha&        -\sin \alpha&        0&        0\\\\
    \sin \alpha&        \cos \alpha&        0&        0\\\\
    0&        0&        1&        0\\\\
    0&        0&        0&        1\\\\
\end{matrix} \right) 
\\]

### 一般旋转

任意一个3D旋转，可以写成：

\\[
R_{xyz}\left( \alpha , \beta , \gamma \right) =R_x\left( \alpha \right) R_y\left( \beta \right) R_z\left( \gamma \right) 
\\]

也就是说，一般旋转可以由绕x、y、z轴的自然旋转组合而成。

在图形学中，任意旋转用矩阵表达为（Rodrigues' Rotation Formula）：

\\[
R\left( \mathbf{n},\alpha \right) =\cos \left( \alpha \right) \mathbf{I}+\left( 1-\cos \left( \alpha \right) \right) \mathbf{nn}^{\mathrm{T}}+\sin \left( \mathrm{\alpha} \right) \underset{\mathrm{N}}{\underbrace{\left( \begin{matrix}
    0&        -n_z&        n_y\\\\
    n_z&        0&        -n_x\\\\
    -n_y&        n_x&        0\\\\
\end{matrix} \right) }}
\\]

> 公式推导：(暂无)

为解决旋转插值问题，参考四元数[link](暂无)。


-----------

> 本文出自CaterpillarStudyGroup，转载请注明出处。  
> https://caterpillarstudygroup.github.io/GAMES101_mdbook/