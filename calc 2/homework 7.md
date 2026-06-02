# 1.
## a.
![[Pasted image 20260602135125.png]]

$$f(x,y)=y \ln (x^2+y^2)$$

$$P=(2,-1)$$

$$\nabla f(x,y)=f_{x}'(x,y)\cdot \vec{i} +f_{y}'(x,y)\cdot \vec{j}$$

$$f_x = y \cdot \frac{2x}{x^2+y^2} = \frac{2xy}{x^2+y^2}$$

$$f_y = 1 \cdot \ln(x^2+y^2) + y \cdot \frac{2y}{x^2+y^2} = \ln(x^2+y^2) + \frac{2y^2}{x^2+y^2}$$

$$f_x(2,-1) = \frac{2(2)(-1)}{2^2+(-1)^2} = -\frac{4}{5}$$

$$f_y(2,-1) = \ln(2^2+(-1)^2) + \frac{2(-1)^2}{2^2+(-1)^2} = \ln(5) + \frac{2}{5}$$

$$\nabla f(2,-1) = \left(-\frac{4}{5}, \ln(5) + \frac{2}{5}\right)$$

---
## b.
![[Pasted image 20260602140446.png]]

$$f(x,y)=x^3y^2 - 2xy$$

$$P=(1,-1)$$

$$\nabla f(x,y)=f_{x}'(x,y)\cdot \vec{i} +f_{y}'(x,y)\cdot \vec{j}$$

$$f_x = 3x^2y^2 - 2y$$

$$f_y = 2x^3y - 2x$$

$$f_x(1,-1) = 3(1)^2(-1)^2 - 2(-1) = 3 + 2 = 5$$

$$f_y(1,-1) = 2(1)^3(-1) - 2(1) = -2 - 2 = -4$$

$$\nabla f(1,-1) = (5, -4)$$

---
## c.
![[Pasted image 20260602140518.png]]

$$f(x,y)=e^{x^2+y^2}$$

$$P=(0,0)$$

$$\nabla f(x,y)=f_{x}'(x,y)\cdot \vec{i} +f_{y}'(x,y)\cdot \vec{j}$$

$$f_x = 2xe^{x^2+y^2}$$

$$f_y = 2ye^{x^2+y^2}$$

$$f_x(0,0) = 2(0)e^{0^2+0^2} = 0$$

$$f_y(0,0) = 2(0)e^{0^2+0^2} = 0$$

$$\nabla f(0,0) = (0, 0)$$

---
## d.
![[Pasted image 20260602140547.png]]
$$f(x,y)=x^y$$

$$P=(2,3)$$

$$\nabla f(x,y)=f_{x}'(x,y)\cdot \vec{i} +f_{y}'(x,y)\cdot \vec{j}$$

$$f_x = yx^{y-1}$$

$$f_y = x^y \ln(x)$$

$$f_x(2,3) = 3(2)^{3-1} = 3(4) = 12$$

$$f_y(2,3) = 2^3 \ln(2) = 8 \ln(2)$$

$$\nabla f(2,3) = (12, 8 \ln(2))$$

---
## e.
![[Pasted image 20260602140612.png]]

$$f(x,y,z)=x^2+y^2+z^2$$

$$P=(1,-1,2)$$

$$\nabla f(x,y,z)=f_{x}'(x,y,z)\cdot \vec{i} +f_{y}'(x,y,z)\cdot \vec{j} + f_{z}'(x,y,z)\cdot \vec{k}$$

$$f_x = 2x$$

$$f_y = 2y$$

$$f_z = 2z$$

$$f_x(1,-1,2) = 2(1) = 2$$

$$f_y(1,-1,2) = 2(-1) = -2$$

$$f_z(1,-1,2) = 2(2) = 4$$

$$\nabla f(1,-1,2) = (2, -2, 4)$$

---
## f.
![[Pasted image 20260602140637.png]]

$$f(x,y,z)=\sqrt{2x^2+y^3}$$

$$P=(0,1,-2)$$

$$\nabla f(x,y,z)=f_{x}'(x,y,z)\cdot \vec{i} +f_{y}'(x,y,z)\cdot \vec{j} + f_{z}'(x,y,z)\cdot \vec{k}$$

$$f_x = \frac{1}{2\sqrt{2x^2+y^3}} \cdot 4x = \frac{2x}{\sqrt{2x^2+y^3}}$$

$$f_y = \frac{1}{2\sqrt{2x^2+y^3}} \cdot 3y^2 = \frac{3y^2}{2\sqrt{2x^2+y^3}}$$

$$f_z = 0$$

$$f_x(0,1,-2) = \frac{2(0)}{\sqrt{2(0)^2+(1)^3}} = 0$$

$$f_y(0,1,-2) = \frac{3(1)^2}{2\sqrt{2(0)^2+(1)^3}} = \frac{3}{2}$$

$$f_z(0,1,-2) = 0$$

$$\nabla f(0,1,-2) = \left(0, \frac{3}{2}, 0\right)$$

---
# 2.
## a.
![[Pasted image 20260602140711.png]]

$$f(x,y)=x^2y$$

$$P=(1,3)$$

$$\vec{u}=-\vec{i}+2\vec{j} = (-1, 2)$$

$$||\vec{u}|| = \sqrt{(-1)^2 + 2^2} = \sqrt{5}$$

$$\hat{u} = \frac{\vec{u}}{||\vec{u}||} = \left(-\frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}}\right)$$

$$\nabla f(x,y)=f_{x}'(x,y)\cdot \vec{i} +f_{y}'(x,y)\cdot \vec{j}$$

$$f_x = 2xy$$

$$f_y = x^2$$

$$f_x(1,3) = 2(1)(3) = 6$$

$$f_y(1,3) = 1^2 = 1$$

$$\nabla f(1,3) = (6, 1)$$

$$D_{\hat{u}}f(1,3) = \nabla f(1,3) \cdot \hat{u} = (6, 1) \cdot \left(-\frac{1}{\sqrt{5}}, \frac{2}{\sqrt{5}}\right)$$

$$D_{\hat{u}}f(1,3) = -\frac{6}{\sqrt{5}} + \frac{2}{\sqrt{5}} = -\frac{4}{\sqrt{5}}$$

---
## b.
![[Pasted image 20260602140811.png]]

$$f(x,y)=y^3+xy$$

$$P=(-2,1)$$

$$\vec{u}=3\vec{i}+\vec{j} = (3, 1)$$

$$||\vec{u}|| = \sqrt{3^2 + 1^2} = \sqrt{10}$$

$$\hat{u} = \frac{\vec{u}}{||\vec{u}||} = \left(\frac{3}{\sqrt{10}}, \frac{1}{\sqrt{10}}\right)$$

$$\nabla f(x,y)=f_{x}'(x,y)\cdot \vec{i} +f_{y}'(x,y)\cdot \vec{j}$$

$$f_x = y$$

$$f_y = 3y^2 + x$$

$$f_x(-2,1) = 1$$

$$f_y(-2,1) = 3(1)^2 + (-2) = 1$$

$$\nabla f(-2,1) = (1, 1)$$

$$D_{\hat{u}}f(-2,1) = \nabla f(-2,1) \cdot \hat{u} = (1, 1) \cdot \left(\frac{3}{\sqrt{10}}, \frac{1}{\sqrt{10}}\right)$$

$$D_{\hat{u}}f(-2,1) = \frac{3}{\sqrt{10}} + \frac{1}{\sqrt{10}} = \frac{4}{\sqrt{10}}$$