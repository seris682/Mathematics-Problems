# 数论
1. 回想数列周期性的证明。 $a_n$ 模 $m$ 的余数有 $m$ 种，由抽屉原理知，其中必有两项的余数相等，不妨设为 $a_r$ 和 $a_t$，则由递推公式知 $a_{r+1}$ 和 $a_{t+1}$ 模 $m$ 的余数相等，以此类推， $a_n\mod m$ 是周期数列（不一定是纯周期），且周期 $T\leq m$。于是
考虑最大情况 $T=m$，此时最晚应于第 $m$ 项进入周期，因为若在第 $m+1$ 项才进入周期，前面还剩 $m$ 项，则由递推公式，周期从第1项开始，矛盾！所以不存在 $\{a_n\}$，使其从第 $i$ 项（ $i>m$ ）才开始进入周期。

# 其它
## 三角
1. _证明：_ $\prod_{k=1}^n{\cos{\frac{k\pi}{2n+1}}}=\frac12$。  

    配对法。由二倍角公式知

$$
\begin{aligned}
\prod_{k=1}^n{\cos{\frac{k\pi}{2n+1}}}&=\frac{
\cos{\frac{\pi}{2n+1}}\cdots \cos{\frac{n\pi}{2n+1}}
\cdot
\sin{\frac{\pi}{2n+1}}\cdots \sin{\frac{n\pi}{2n+1}}}
{\sin{\frac{\pi}{2n+1}}\cdots \sin{\frac{n\pi}{2n+1}}}\\
&=\frac{1}{2^n}
\cdot
\frac{
\sin{\frac{2\pi}{2n+1}}\sin{\frac{4\pi}{2n+1}}\cdots \sin{\frac{2n\pi}{2n+1}}}
{\sin{\frac{\pi}{2n+1}}\cdots \sin{\frac{n\pi}{2n+1}}}\\
&=\frac{1}{2^n}。
\end{aligned}
$$
