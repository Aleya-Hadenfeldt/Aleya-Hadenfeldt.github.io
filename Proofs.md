# Math & Proofs

## Real Analysis

- This proof shows that if the integrator \( \alpha \) is constant, then every bounded function is Riemann–Stieltjes integrable with respect to \( \alpha \), and the integral is always zero.

Let \( \alpha(x)=C \) be a constant function and let  
\( f:[a,b]\to\mathbb{R} \) be any bounded function.  
Let  
\( P=\{a=x_0<x_1<\cdots<x_n=b\} \)  
be any partition of \([a,b]\).

Since \( \alpha(x)=C \) is constant, we have  
\[
\Delta\alpha_i=\alpha(x_i)-\alpha(x_{i-1})=C-C=0
\quad \text{for all } i.
\]

Therefore the upper Riemann–Stieltjes sum is
\[
U(P,f,\alpha)
=\sum_{i=1}^n M_i\,\Delta\alpha_i
=\sum_{i=1}^n M_i\cdot 0
=\sum_{i=1}^n 0
=0,
\]
and the lower Riemann–Stieltjes sum is
\[
L(P,f,\alpha)
=\sum_{i=1}^n m_i\,\Delta\alpha_i
=\sum_{i=1}^n m_i\cdot 0
=\sum_{i=1}^n 0
=0.
\]

Thus every Riemann–Stieltjes sum equals \(0\).  
Hence the upper and lower integrals satisfy
\[
\overline{\int_a^b} f\,d\alpha
=\inf\{U(P,f,\alpha)\mid P \text{ is a partition}\}
=\inf\{0\}
=0
\]
and
\[
\underline{\int_a^b} f\,d\alpha
=\sup\{L(P,f,\alpha)\mid P \text{ is a partition}\}
=\sup\{0\}
=0.
\]

Since the upper and lower integrals are equal, the Riemann–Stieltjes integral exists and
\[
\int_a^b f\,d\alpha
=\overline{\int_a^b} f\,d\alpha
=\underline{\int_a^b} f\,d\alpha
=0.
\]

Therefore \( f\in \mathcal{R}(\alpha) \).

[Back to Home](index.md)