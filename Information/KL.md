# KL散度 KL divergence

有两个独立的分布P(x)和Q(x)，KL散度用于衡量这两个分布的差异。  

$$
D_{KL}(P||Q) = E_{X\sim P}\left[\log \frac{P(x)}{Q(x)}\right] = E_{X\sim P}[\log P(x) - \log Q(x)]
$$

# 交叉熵 cross-entropy

$$
H(P, Q) = -E_{X\sim P} \log Q(x)
$$

最小化交叉熵等价于最小化KL散度。  