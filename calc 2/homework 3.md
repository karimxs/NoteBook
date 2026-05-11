# 1.
<<<<<<< HEAD
![[Pasted image 20260416101922.png|697]]
$$
f_{n}(x)=\frac{\sin (n\cdot x)+\sin(x)}{n\cdot x} \left\{ x \in (0,\infty) \right\} 
$$
$$
\frac{\sin (n\cdot x)+\sin(x)}{n\cdot x}=\frac{\sin(n\cdot x)}{n\cdot x}+\frac{\sin(x)}{n\cdot x}
$$
$$
-1\leq\sin(n\cdot x)\leq 1
$$
$$
-\frac{1}{n\cdot x}\leq\frac{sin(n\cdot x)}{n\cdot x}\leq \frac{1}{n\cdot x}
$$
$$
\lim_{ n \to \infty } -\frac{1}{n\cdot x}\leq\frac{sin(n\cdot x)}{n\cdot x}\leq \frac{1}{n\cdot x}=0\leq\frac{sin(n\cdot x)}{n\cdot x}\leq0
$$
$$
\lim_{ n \to \infty } \frac{\sin(n\cdot x)}{n\cdot x}+\frac{\sin(x)}{n\cdot x}=0+0=0
$$
---
=======
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
![[Pasted image 20260502124601.png]]

$$ f_{n}(x) = (\sin(x))^{2n} $$

$$ x \in (-\infty, \infty) $$

$$ f(x) = \lim_{n \to \infty} f_{n}(x) = \lim_{n \to \infty} (\sin(x))^{2n} $$

$$ = \lim_{n \to \infty} \left((\sin(x))^2\right)^n $$

$$ \text{Since } -1 \leq \sin(x) \leq 1 \text{, we know that } 0 \leq (\sin(x))^2 \leq 1 $$

$$ \text{We must evaluate the limit based on two cases for the value of } (\sin(x))^2: $$

$$ \text{Case 1: } (\sin(x))^2 < 1 \implies x \neq \frac{\pi}{2} + \pi k \quad (k \in \mathbb{Z}) $$

$$ f(x) = \lim_{n \to \infty} \left((\sin(x))^2\right)^n = 0 $$

$$ \text{Case 2: } (\sin(x))^2 = 1 \implies x = \frac{\pi}{2} + \pi k \quad (k \in \mathbb{Z}) $$

$$ f(x) = \lim_{n \to \infty} 1^n = 1 $$

$$ f(x) = \begin{cases} 1, & x = \frac{\pi}{2} + \pi k \\ 0, & x \neq \frac{\pi}{2} + \pi k \end{cases} $$


---
# 1.
![[Pasted image 20260502124743.png]]
$$ f_{n}(x) = \frac{\arctan(x)}{n} $$

$$ x \in \mathbb{R} $$

$$ f(x) = \lim_{n \to \infty} f_{n}(x) = \lim_{n \to \infty} \frac{\arctan(x)}{n} $$

$$ \text{Since } -\frac{\pi}{2} < \arctan(x) < \frac{\pi}{2} \text{ for all } x \in \mathbb{R}: $$

$$ -\frac{\pi}{2n} < \frac{\arctan(x)}{n} < \frac{\pi}{2n} $$

$$ \text{By the Squeeze Theorem, as } n \to \infty: $$

$$ f(x) = 0 $$


$$ \text{We evaluate } \lim_{n \to \infty} \sup_{x \in \mathbb{R}} \left| f_{n}(x) - f(x) \right| $$

$$ = \lim_{n \to \infty} \sup_{x \in \mathbb{R}} \left| \frac{\arctan(x)}{n} - 0 \right| $$

$$ = \lim_{n \to \infty} \sup_{x \in \mathbb{R}} \frac{\left| \arctan(x) \right|}{n} $$

$$ \text{The supremum (least upper bound) of } \left| \arctan(x) \right| \text{ on } \mathbb{R} \text{ is } \frac{\pi}{2} $$

$$ = \lim_{n \to \infty} \frac{\frac{\pi}{2}}{n} $$

$$ = \lim_{n \to \infty} \frac{\pi}{2n} = 0 $$

$$ \text{Conclusion: Since the limit of the supremum is 0, there } \mathbf{is} \text{ uniform convergence on } \mathbb{R}. $$

---
# 2.
![[Pasted image 20260502124924.png]]
$$ f_n(x) = \left(1 + \frac{1}{n}\right)^n x $$

$$ x \in (0, 5) $$

$$ f(x) = \lim_{n \to \infty} f_n(x) = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n x $$

$$ \text{Using the fundamental limit } \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e: $$

$$ f(x) = e \cdot x $$

$$ \text{We evaluate } \lim_{n \to \infty} \sup_{x \in (0, 5)} |f_n(x) - f(x)| $$

$$ = \lim_{n \to \infty} \sup_{x \in (0, 5)} \left| \left(1 + \frac{1}{n}\right)^n x - ex \right| $$

$$ = \lim_{n \to \infty} \sup_{x \in (0, 5)} x \left| \left(1 + \frac{1}{n}\right)^n - e \right| $$

$$ \text{Since } \left(1 + \frac{1}{n}\right)^n \text{ and } e \text{ are constants with respect to } x\text{, and } x \in (0, 5): $$

$$ \text{The supremum (least upper bound) of } x \text{ on this interval is } 5. $$

$$ = \lim_{n \to \infty} 5 \left| \left(1 + \frac{1}{n}\right)^n - e \right| $$

$$ \text{Now, evaluate the limit as } n \to \infty: $$

$$ = 5 \left| e - e \right| $$

$$ = 0 $$

$$ \text{Conclusion: Since the limit of the supremum is 0, there } \mathbf{is} \text{ uniform convergence on } (0, 5). $$

---
# 3.
![[Pasted image 20260502125149.png]]
$$ f_n(x) = \left(1 + \frac{1}{n}\right)^n x $$

$$ x \in (0, 5) $$


$$ f(x) = \lim_{n \to \infty} f_n(x) = \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n x $$

$$ \text{Using the fundamental limit } \lim_{n \to \infty} \left(1 + \frac{1}{n}\right)^n = e: $$

$$ f(x) = e \cdot x $$


$$ \text{We evaluate } \lim_{n \to \infty} \sup_{x \in (0, 5)} |f_n(x) - f(x)| $$

$$ = \lim_{n \to \infty} \sup_{x \in (0, 5)} \left| \left(1 + \frac{1}{n}\right)^n x - ex \right| $$

$$ = \lim_{n \to \infty} \sup_{x \in (0, 5)} x \left| \left(1 + \frac{1}{n}\right)^n - e \right| $$

$$ \text{Since } \left(1 + \frac{1}{n}\right)^n \text{ and } e \text{ are constants with respect to } x\text{, and } x \in (0, 5): $$

$$ \text{The supremum (least upper bound) of } x \text{ on this interval is } 5. $$

$$ = \lim_{n \to \infty} 5 \left| \left(1 + \frac{1}{n}\right)^n - e \right| $$

$$ \text{Now, evaluate the limit as } n \to \infty: $$

$$ = 5 \left| e - e \right| $$

$$ = 0 $$

$$ \text{Conclusion: Since the limit of the supremum is 0, there } \mathbf{is} \text{ uniform convergence on } (0, 5). $$
>>>>>>> origin/main
