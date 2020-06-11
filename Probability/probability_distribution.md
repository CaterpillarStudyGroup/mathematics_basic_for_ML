||离散型变量|连续性变量|
---|---|---
概率分布|概率质量函数<br>$$x \sim P(x)$$ | 概率密度函数<br>$$x \sim p(x)$$
性质1|定义域必须是x所有可能的状态的集合 | 同
性质2|$$\forall x, 0 \leq P(x) \leq 1$$ | $$\forall x, 0 \leq p(x)$$<br>Note:不要求$$p(x) \leq 1$$
性质3（归一化）| $$\sum_{a \in x}P(a) = 1$$ | $$\int p(x)dx = 1$$
部分概率 | P(x = a) | $$\int_a^b p(x)dx$$
联合分布|P(X=x, Y=y)||
边缘概率 | $$\forall a \in x, P(x=a)=\sum_{b \in y}P(x=a, y=b)$$ | $$p(x)=\int p(x,y)dy$$
条件概率 | $$P(y=b\mid x=a) = \frac {P(y=b, x=a)}{P(x=a)}$$ | $$P(A\mid B) = \frac{P(A,B)}{P(B)}$$<br>P()为连续型变量落入某一区间的概率



# 条件概率的链式法则

$$
P(A, B, C) = P(A|B,C)P(B|C)P(C)
$$

# 独立

**相互独立**：P(A, B) = P(A)P(B)  
**条件独立**：P(A, B | C) = P(A | C)P(B | C)