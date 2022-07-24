# f-divergence

$$
D_f(P||Q) = \int_x q(x)f\left(\frac{p(x)}{q(x)}\right)dx
$$

且f(x) is convex && f(1) = 0

$D_f(P||Q)$用于评估分布P和分布Q的差异。  
f(1) = 0 ==> 当p(x)=q(x)时，Df = 0  
f is convex ==> Df >= f(1) = 0

令$f(x) = x\log x$，则Df是KL divergence  
$$
D_f = \int_x p(x)\log\left(\frac{p(x)}{q(x)}\right)
$$

令$f(x) = -\log x$，则Df是reverse KL divergence  
$$
D_f = \int_x q(x)\log\left(\frac{q(x)}{p(x)}\right)
$$

令$f(x) = (x-1)^2$，则Df是Chi Square Divergence  
$$
D_f = \int_x\frac{(p(x)-q(x))^2}{q(x)}dx
$$

# KL散度 KL divergence

有两个独立的分布P(x)和Q(x)，KL散度用于衡量这两个分布的差异。  

$$
D_{KL}(P||Q) = E_{X\sim P}\left[\log \frac{P(x)}{Q(x)}\right] = E_{X\sim P}[\log P(x) - \log Q(x)]
$$

## 交叉熵 cross-entropy

$$
H(P, Q) = -E_{X\sim P} \log Q(x)
$$

最小化交叉熵等价于最小化KL散度。  

# JS散度 Jensen-Shannon

http://blog.sina.com.cn/s/blog_18bdda0da0102xzpw.html
