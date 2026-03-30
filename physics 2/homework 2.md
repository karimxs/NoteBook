# 1.
![[Pasted image 20260330141229.png]]
$$
\int_{0}^{2}\int_{0}^{1}\int_{0}^{4}3xyz^{2}\space dx\space dy\space dz
$$
Let's take every part of this integration 
$$
\int_{0}^{4}3xyz^{2} dx= \frac{3}{2}x^{2}yz^2|^{4}_{0}=24yz^2
$$
$$
\int^1_{0} 24yz^2dy=12y^2z^2|^{1}_{0}=12z^2
$$
$$
\int_{0}^2 12z^2dz=4z^3|^{2}_{0}=32
$$
$$
\int_{0}^{2}\int_{0}^{1}\int_{0}^{4}3xyz^{2}\space dx\space dy\space dz=32
$$
 ---
# 2.
![[Pasted image 20260330142339.png]]
$$
\int ^{3}_{1}\int ^{x^2}_{x} (x+y)dy\space dx
$$
$$
\int ^{x^2}_{x}(x+y)dy=xy+\frac{y^{2}}{2}|^{x^2}_{x}=x^{3}+\frac{x^{4}}{2}-x^{2}-\frac{x^{2}}{2}
$$
$$
=\frac{x^4}{2}+x^3-1.5x^2
$$
$$
\int^3_{1}x^4+x^3-1.5x^2dx =\frac{x^5}{10}+\frac{x^4}{4}-\frac{x^3}{2}|^3_{1}
$$
$$
=31.05--0.15=31.2
$$
$$
\int ^{3}_{1}\int ^{x^2}_{x} (x+y)dy\space dx=31.2
$$
---
# 3.
![[Pasted image 20260330143748.png]]
## a.
$$
Q=\int \int \sigma dA
$$
$$
=\int \int \alpha y^{2} \space dx \space dy
$$
$$
R^2=x^2+y^2
$$
$$
\int^R_{-R} \int_{-\sqrt{ R^{2}-x^2 }}^\sqrt{ R^{2}-x^{2} } \alpha y^2 \space dy \space dx
$$
$$
\int_{-\sqrt{ R^{2}-x^2 }}^\sqrt{ R^{2}-x^{2} } \alpha y^2 \space dy=\frac{\alpha y^{3}}{3}=\frac{\alpha(R^2-x^2)^{1.5}}{3}+\frac{\alpha(R^2-x^2)^{1.5}}{3}
$$
$$
=\frac{2\alpha(R^2-x^2)^{1.5}}{3}
$$
$$
\int^R_{-R} \frac{2\alpha(R^2-x^2)^{1.5}}{3} dx
=$$
