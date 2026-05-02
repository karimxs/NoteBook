# 1.
![[Pasted image 20260501191327.png]]
$$
f_{n}(x) =\frac{\sin(n\cdot x) +\sin (x)}{n\cdot x}
$$
$$
x \in (0,\infty)
$$
$$
f(x)=\lim_{ n \to \infty } f_{n}(x)=\lim_{ n \to \infty } \frac{\sin(n\cdot x) +\sin (x)}{n\cdot x}
$$
$$
-1\leq\sin(nx)\leq 1
$$
$$
-\frac{1}{\left| n\cdot x \right| }\leq\frac{\sin(n\cdot x)}{n\cdot x}\leq \frac{1}{\left| n\cdot x \right| } 
$$
$$
\lim_{ n \to \infty } \frac{\sin(n\cdot x)}{n\cdot x} =\lim_{ n \to \infty } \frac{1}{\left| n\cdot x \right| } =0
$$
$$
\lim_{ n \to \infty } \frac{\sin(n\cdot x) +\sin (x)}{n\cdot x}=0
$$
$$
\lim_{ n \to \infty } f_{n}(x)=0
$$
---
# 2.
![[Pasted image 20260501193848.png]]

$$ f_{n}(x)=n\cdot(\sqrt[n]{ 10\cdot x }-1) $$

$$ x \in (0,\infty) $$

$$ f(x)=\lim_{ n \to \infty } f_{n}(x)=\lim_{ n \to \infty } n\cdot(\sqrt[n]{ 10\cdot x }-1) $$

$$ \lim_{ n \to \infty } n\cdot((10\cdot x)^{1/n}-1) $$

$$ =\lim_{ n \to \infty } \frac{(10\cdot x)^{1/n}-1}{\frac{1}{n}} $$

$$ =\lim_{ h \to 0 } \frac{(10\cdot x)^{h}-1}{h}\left\{ L'Hôpital \right\} $$

$$ =\lim_{ h \to 0 } \frac{(10\cdot x)^{h}\cdot\ln(10\cdot x)}{1} $$

$$ =(10\cdot x)^{0}\cdot\ln(10\cdot x) $$

$$ =1\cdot\ln(10\cdot x) $$

$$ =\ln(10\cdot x) $$
---
# 3.
![[Pasted image 20260502124009.png]]

$$ f_{n}(x)=n\cdot\left(\sqrt{ 9x+\frac{1}{n} }-\sqrt{ 9x }\right) $$

$$ x \in (0,\infty) $$

$$ f(x)=\lim_{ n \to \infty } f_{n}(x)=\lim_{ n \to \infty } n\cdot\left(\sqrt{ 9x+\frac{1}{n} }-\sqrt{ 9x }\right) $$

$$ \lim_{ n \to \infty } \frac{\sqrt{ 9x+\frac{1}{n} }-\sqrt{ 9x }}{\frac{1}{n}} $$

$$ =\lim_{ h \to 0 } \frac{\sqrt{ 9x+h }-\sqrt{ 9x }}{h}\left\{ L'Hôpital \right\} $$

$$ =\lim_{ h \to 0 } \frac{\frac{1}{2\sqrt{ 9x+h }}}{1} $$

$$ =\frac{1}{2\sqrt{ 9x }} $$

$$ =\frac{1}{6\sqrt{ x }} $$
---
# 4.
