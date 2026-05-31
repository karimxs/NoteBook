# 1.
## a.
![[Pasted image 20260531093026.png]]
$$
\lim_{ (x,y) \to (0,0) } \frac{x^2+y^2}{x^2+2y^2}
$$
let's say that
$$
y=kx
$$
$$
\lim_{ (x,y) \to (0,0) } \frac{x^2+(kx)^2}{x^2+2(kx)^2}=
$$
$$
\lim_{ (x,y) \to (0,0) } \frac{x^2+k^2x^2}{x^2+2k^2x^2}=
$$
$$
\lim_{ (x,y) \to (0,0) } \frac{x^2(1+k^2)}{x^2(1+2k^2)}=
$$
$$
\lim_{ (x,y) \to (0,0) } \frac{1+k^2}{1+2k^2}
$$
there is no limit because it depends on k.

---
**b.**
![[Pasted image 20260531112102.png]]

$$\lim_{(x,y) \to (0,0)} \frac{x^2-y^2}{x^2+y^2}$$

let's say that $y=mx$

$$\lim_{(x,y) \to (0,0)} \frac{x^2-(mx)^2}{x^2+(mx)^2}=$$

$$\lim_{x \to 0} \frac{x^2-m^2x^2}{x^2+m^2x^2}=$$

$$\lim_{x \to 0} \frac{x^2(1-m^2)}{x^2(1+m^2)}=$$

$$\frac{1-m^2}{1+m^2}$$

there is no limit because it depends on the path $m$.

---
**c.**
![[Pasted image 20260531112110.png]]

$$\lim_{(x,y) \to (0,0)} \frac{xy}{x^2+y^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x \cdot 0}{x^2+0^2} = 0$$

let's check the path $y=x$:

$$\lim_{x \to 0} \frac{x \cdot x}{x^2+x^2}=$$

$$\lim_{x \to 0} \frac{x^2}{2x^2} = \frac{1}{2}$$

since the limits are different for different paths, there is no limit.

---
**d.**
![[Pasted image 20260531112123.png]]

$$\lim_{(x,y) \to (0,0)} \frac{x^2y^2}{x^2+y^2}$$

using the squeeze theorem (sandwich):

$$0 \le \left| \frac{x^2y^2}{x^2+y^2} \right| = y^2 \left| [cite_start]\frac{x^2}{x^2+y^2} \right|$$

since $x^2 \le x^2+y^2$, we know that $\frac{x^2}{x^2+y^2} \le 1$.

$$y^2 \left| \frac{x^2}{x^2+y^2} \right| [cite_start]\le y^2 \cdot 1 = y^2$$

$$\lim_{(x,y) \to (0,0)} y^2 = 0$$

therefore, by the squeeze theorem, the limit is $0$.

---
**2.**
**a.**
![[Pasted image 20260531112137.png]]

$$\lim_{(x,y) \to (0,0)} \frac{|xy|}{x^2+y^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{|x \cdot 0|}{x^2+0^2} = 0$$

let's check the path $y=x$:

$$\lim_{x \to 0} \frac{|x \cdot x|}{x^2+x^2}=$$

$$\lim_{x \to 0} \frac{x^2}{2x^2} = \frac{1}{2}$$

since the limits are different for different paths, there is no limit.

---
**b.**
![[Pasted image 20260531112342.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2y}{x^2+y^2}$$

using the squeeze theorem (sandwich):

$$0 \le \left| \frac{x^2y}{x^2+y^2} \right| = |y| \left| [cite_start]\frac{x^2}{x^2+y^2} \right|$$

since $\frac{x^2}{x^2+y^2} \le 1$:

$$|y| \left| \frac{x^2}{x^2+y^2} \right| \le |y| [cite_start]\cdot 1 = |y|$$

$$\lim_{(x,y) \to (0,0)} |y| [cite_start]= 0$$

therefore, by the squeeze theorem, the limit is $0$.

---
**c.**
![[Pasted image 20260531112356.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^4+y^4}{x^2+y^2}$$

using the squeeze theorem (sandwich):

$$0 \le \frac{x^4+y^4}{x^2+y^2} \le \frac{x^4}{x^2} + \frac{y^4}{y^2} = x^2 + y^2$$

$$\lim_{(x,y) \to (0,0)} (x^2 + y^2) = 0$$

therefore, by the squeeze theorem, the limit is $0$.

**d.**
![[Pasted image 20260531112404.png]]
$$\lim_{(x,y) \to (0,0)} \frac{|x|^3+|y|^3}{x^2+y^2}$$

using the squeeze theorem (sandwich):

$$0 \le \frac{|x|^3+|y|^3}{x^2+y^2} \le \frac{|x|^3}{x^2} + \frac{|y|^3}{y^2} = |x| + [cite_start]|y|$$

$$\lim_{(x,y) \to (0,0)} (|x| + |y|) = 0$$

therefore, by the squeeze theorem, the limit is $0$.

---
**3.**

**a.**
![[Pasted image 20260531112507.png]]

$$\lim_{(x,y) \to (0,0)} \frac{\sin(xy)}{x^2+y^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{\sin(x \cdot 0)}{x^2+0^2} = 0$$

let's check the path $y=x$:

$$\lim_{x \to 0} \frac{\sin(x \cdot x)}{x^2+x^2} =$$

$$\lim_{x \to 0} \frac{\sin(x^2)}{2x^2} = \frac{1}{2} \cdot 1 = \frac{1}{2}$$

since the limits are different for different paths, there is no limit.

---
**b.**
![[Pasted image 20260531112521.png]]
$$\lim_{(x,y) \to (0,0)} \frac{\sin(x^2+y^2)}{x^2+y^2}$$

let $t = x^2+y^2$.

as $(x,y) \to (0,0)$, $t \to 0$.

$$\lim_{t \to 0} \frac{\sin(t)}{t} = 1$$

so the limit is $1$.

---
**c.**
![[Pasted image 20260531112533.png]]
$$\lim_{(x,y) \to (0,0)} (x^2+y^2)\sin\left(\frac{1}{x^2+y^2}\right)$$

using the squeeze theorem (sandwich):

$$0 \le \left| (x^2+y^2)\sin\left(\frac{1}{x^2+y^2}\right) \right| \le x^2+y^2$$

since $\left|\sin\left(\frac{1}{x^2+y^2}\right)\right| \le 1$.

$$\lim_{(x,y) \to (0,0)} (x^2+y^2) = 0$$

therefore, by the squeeze theorem, the limit is $0$.

---
**d.**
![[Pasted image 20260531112545.png]]
$$\lim_{(x,y) \to (0,0)} \frac{xy}{x^2+y^2}\sin\left(\frac{1}{x^2+y^2}\right)$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x \cdot 0}{x^2+0^2}\sin\left(\frac{1}{x^2+0^2}\right) = 0$$

let's check the path $y=x$:

$$\lim_{x \to 0} \frac{x \cdot x}{x^2+x^2}\sin\left(\frac{1}{x^2+x^2}\right) =$$

$$\lim_{x \to 0} \frac{x^2}{2x^2}\sin\left(\frac{1}{2x^2}\right) =$$

$$\lim_{x \to 0} \frac{1}{2}\sin\left(\frac{1}{2x^2}\right)$$

this limit does not exist because the sine function oscillates.

since there is no limit on the path $y=x$, the overall limit does not exist.