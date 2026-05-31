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

---
**4.**

**a.**
![[Pasted image 20260531112903.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2+y^2}{\sqrt{x^2+y^2}}$$

converting to polar coordinates ($x = r\cos\theta$, $y = r\sin\theta$ as $r \to 0$):

$$\lim_{r \to 0} \frac{r^2\cos^2\theta + r^2\sin^2\theta}{\sqrt{r^2\cos^2\theta + r^2\sin^2\theta}}=$$

$$\lim_{r \to 0} \frac{r^2(\cos^2\theta + \sin^2\theta)}{\sqrt{r^2(\cos^2\theta + \sin^2\theta)}}=$$

$$\lim_{r \to 0} \frac{r^2}{r} = \lim_{r \to 0} r = 0$$

the limit is $0$.

---
**b.**
![[Pasted image 20260531113009.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2-y^2}{\sqrt{x^2+y^2}}$$

converting to polar coordinates:

$$\lim_{r \to 0} \frac{r^2\cos^2\theta - r^2\sin^2\theta}{\sqrt{r^2\cos^2\theta + r^2\sin^2\theta}}=$$

$$\lim_{r \to 0} \frac{r^2(\cos^2\theta - \sin^2\theta)}{r}=$$

$$\lim_{r \to 0} r(\cos^2\theta - \sin^2\theta)$$

since $\cos^2\theta - \sin^2\theta$ is a bounded function and $r \to 0$, the limit is $0$.

---
**c.**
![[Pasted image 20260531113015.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^3+y^3}{\sqrt{x^2+y^2}}$$

converting to polar coordinates:

$$\lim_{r \to 0} \frac{r^3\cos^3\theta + r^3\sin^3\theta}{\sqrt{r^2\cos^2\theta + r^2\sin^2\theta}}=$$

$$\lim_{r \to 0} \frac{r^3(\cos^3\theta + \sin^3\theta)}{r}=$$

$$\lim_{r \to 0} r^2(\cos^3\theta + \sin^3\theta)$$

since $\cos^3\theta + \sin^3\theta$ is bounded and $r^2 \to 0$, the limit is $0$.

---
**d.**
![[Pasted image 20260531113023.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2y}{\sqrt{x^2+y^2}}$$

converting to polar coordinates:

$$\lim_{r \to 0} \frac{(r\cos\theta)^2(r\sin\theta)}{\sqrt{r^2\cos^2\theta + r^2\sin^2\theta}}=$$

$$\lim_{r \to 0} \frac{r^3\cos^2\theta\sin\theta}{r}=$$

$$\lim_{r \to 0} r^2\cos^2\theta\sin\theta$$

since $\cos^2\theta\sin\theta$ is bounded and $r^2 \to 0$, the limit is $0$.

---
**5.**

**a.**
![[Pasted image 20260531113036.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x-y}{x+y}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x-0}{x+0} = \lim_{x \to 0} \frac{x}{x} = 1$$

let's check the path $x=0$:

$$\lim_{y \to 0} \frac{0-y}{0+y} = \lim_{y \to 0} \frac{-y}{y} = -1$$

since the limits are different for different paths ($1 \neq -1$), there is no limit.

---
**b.**
![[Pasted image 20260531113043.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2-y^2}{x^2+y^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x^2-0}{x^2+0} = \lim_{x \to 0} \frac{x^2}{x^2} = 1$$

let's check the path $x=0$:

$$\lim_{y \to 0} \frac{0-y^2}{0+y^2} = \lim_{y \to 0} \frac{-y^2}{y^2} = -1$$

since the limits are different for different paths, there is no limit.

---
**c.**
![[Pasted image 20260531113057.png]]
$$\lim_{(x,y) \to (0,0)} \frac{xy}{|x|+|y|}$$

using the squeeze theorem (sandwich):

$$0 \le \left| \frac{xy}{|x|+|y|} \right| = \frac{|x||y|}{|x|+|y|}$$

since $|x| \le |x|+|y|$, we know that $\frac{|x|}{|x|+|y|} \le 1$.

$$\frac{|x||y|}{|x|+|y|} = |y| \left( \frac{|x|}{|x|+|y|} \right) \le |y| \cdot 1 = |y|$$

$$\lim_{(x,y) \to (0,0)} |y| [cite_start]= 0$$

therefore, by the squeeze theorem, the limit is $0$.

---
**d.**
![[Pasted image 20260531113105.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2y}{x^4+y^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x^2 \cdot 0}{x^4+0^2} = 0$$

let's check the path $y=x^2$:

$$\lim_{x \to 0} \frac{x^2 \cdot x^2}{x^4+(x^2)^2}=$$

$$\lim_{x \to 0} \frac{x^4}{x^4+x^4}=$$

$$\lim_{x \to 0} \frac{x^4}{2x^4} = \frac{1}{2}$$

since the limits are different for different paths ($0 \neq \frac{1}{2}$), there is no limit.

---

**6.**

**a.**
![[Pasted image 20260531113308.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2y}{x^4+y^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x^2 \cdot 0}{x^4+0^2} = 0$$

let's check the path $y=x^2$:

$$\lim_{x \to 0} \frac{x^2 \cdot x^2}{x^4+(x^2)^2}=$$

$$\lim_{x \to 0} \frac{x^4}{x^4+x^4}=$$

$$\lim_{x \to 0} \frac{x^4}{2x^4} = \frac{1}{2}$$

since the limits are different for different paths, there is no limit.

---
**b.**
![[Pasted image 20260531113317.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2y^2}{(x^2+y^2)^2}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x^2 \cdot 0^2}{(x^2+0^2)^2} = 0$$

let's check the path $y=x$:

$$\lim_{x \to 0} \frac{x^2 \cdot x^2}{(x^2+x^2)^2}=$$

$$\lim_{x \to 0} \frac{x^4}{(2x^2)^2}=$$

$$\lim_{x \to 0} \frac{x^4}{4x^4} = \frac{1}{4}$$

since the limits are different for different paths, there is no limit.

---
**c.**
![[Pasted image 20260531113324.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^3y}{x^2+y^2}$$

using the squeeze theorem (sandwich):

$$0 \le \left| \frac{x^3y}{x^2+y^2} \right| = |xy| \left| \frac{x^2}{x^2+y^2} \right|$$

since $x^2 \le x^2+y^2$, we know that $\frac{x^2}{x^2+y^2} \le 1$.

$$|xy| \left| \frac{x^2}{x^2+y^2} \right| \le |xy| \cdot 1 = |xy|$$

$$\lim_{(x,y) \to (0,0)} |xy| = 0$$

therefore, by the squeeze theorem, the limit is $0$.

---
**d.**
![[Pasted image 20260531113331.png]]
$$\lim_{(x,y) \to (0,0)} \frac{x^2y^2}{x^4+y^4}$$

let's check the path $y=0$:

$$\lim_{x \to 0} \frac{x^2 \cdot 0^2}{x^4+0^4} = 0$$

let's check the path $y=x$:

$$\lim_{x \to 0} \frac{x^2 \cdot x^2}{x^4+x^4}=$$

$$\lim_{x \to 0} \frac{x^4}{2x^4} = \frac{1}{2}$$

since the limits are different for different paths, there is no limit.

---
**7.**

**a.**
![[Pasted image 20260531113340.png]]
$$\lim_{x \to 0} \left( \lim_{y \to 0} \frac{xy}{x^2+y^2} \right)$$

first, evaluate the inner limit (treating $x$ as a constant where $x \neq 0$):

$$\lim_{y \to 0} \frac{xy}{x^2+y^2} = \frac{x \cdot 0}{x^2+0^2} = \frac{0}{x^2} = 0$$

now, evaluate the outer limit:

$$\lim_{x \to 0} (0) = 0$$

---
**b.**
![[Pasted image 20260531113348.png]]
$$\lim_{y \to 0} \left( \lim_{x \to 0} \frac{xy}{x^2+y^2} \right)$$

first, evaluate the inner limit (treating $y$ as a constant where $y \neq 0$):

$$\lim_{x \to 0} \frac{xy}{x^2+y^2} = \frac{0 \cdot y}{0^2+y^2} = \frac{0}{y^2} = 0$$

now, evaluate the outer limit:

$$\lim_{y \to 0} (0) = 0$$

---
**c.**
![[Pasted image 20260531113411.png]]
$$\lim_{x \to 0} \left( \lim_{y \to 0} \frac{x^2y}{x^2+y^2} \right)$$

evaluate the inner limit (treating $x$ as a constant where $x \neq 0$):

$$\lim_{y \to 0} \frac{x^2y}{x^2+y^2} = \frac{x^2 \cdot 0}{x^2+0^2} = 0$$

evaluate the outer limit:

$$\lim_{x \to 0} (0) = 0$$
---
**d.**
![[Pasted image 20260531113417.png]]
$$\lim_{y \to 0} \left( \lim_{x \to 0} \frac{x^2y}{x^2+y^2} \right)$$

evaluate the inner limit (treating $y$ as a constant where $y \neq 0$):

$$\lim_{x \to 0} \frac{x^2y}{x^2+y^2} = \frac{0^2 \cdot y}{0^2+y^2} = 0$$

evaluate the outer limit:

$$\lim_{y \to 0} (0) = 0$$