# 1.
![[Pasted image 20260602141840.png]]
### Step 0: Classification and Method

This is a second-order linear non-homogeneous ordinary differential equation (ODE) with constant coefficients. The non-homogeneous part has a form that allows us to guess a particular solution. Since the general solution is structured as $y=y_{p}+y_{h}$, the approach will be to first find the solution to the associated homogeneous ODE using a characteristic polynomial, and then guess a solution for the particular part.

### Step 1: Solving the Associated Homogeneous ODE

We begin with the homogeneous equation:

$y^{\prime\prime}-y=0$

Its characteristic polynomial is:

$p(\lambda)=\lambda^{2}-1=(\lambda-1)(\lambda+1)$

Therefore, $e^{x}$ and $e^{-x}$ are solutions to the homogeneous ODE. Because this is a second-order ODE, they form a basis for its solution space. Thus, the general solution for the homogeneous equation is: $y_{h}=C_{1}e^{-x}+C_{2}e^{x}$

### Step 2: Finding a Particular Solution

We will find a particular solution for the non-homogeneous equation using the method of undetermined coefficients (guessing).

The non-homogeneous part of the ODE is $e^{x}$, but we cannot guess a solution of the form $Ae^{x}$ because $e^{x}$ is a root of the characteristic polynomial of the homogeneous equation, which would result in linear dependence. To resolve this, we multiply by $x$, making our guess: $y_{p}=\alpha xe^{x}$

Now, we differentiate this guess:

- $y_{p}^{\prime}=\alpha(x+1)e^{x}$
    
- $y_{p}^{\prime\prime}=\alpha(x+2)e^{x}$
    

Next, substitute these into the original non-homogeneous ODE ($y^{\prime\prime}-y=e^{x}$):

- $\alpha(x+2)e^{x}-\alpha xe^{x}=e^{x}$
    
- $\alpha(x+2-x)e^{x}=e^{x}$
    
- $2\alpha e^{x}=e^{x}$
    

Solving for $\alpha$, we get:

$\alpha=\frac{1}{2}$

This gives us the particular solution:

$y_{p}=\frac{1}{2}xe^{x}$

### Step 3: The General Solution

Combining the homogeneous and particular solutions gives the general solution:

$y=\frac{1}{2}xe^{x}+C_{1}e^{-x}+C_{2}e^{x}$

### Step 4: Applying Initial Conditions

The initial conditions must be applied to the general solution and its derivative. First, we differentiate the general solution: $y^{\prime}=\frac{1}{2}(x+1)e^{x}-C_{1}e^{-x}+C_{2}e^{x}$

Now, substitute the initial conditions $y(0)=0$ and $y^{\prime}(0)=0$:

- $0=y(0)=C_{1}+C_{2}$
    
- $0=y^{\prime}(0)=\frac{1}{2}-C_{1}+C_{2}$
    

We now have a system of two equations with two variables. Solving this system yields:

$C_{2}=-\frac{1}{4}$ and $C_{1}=\frac{1}{4}$

### Final Answer

Substituting the constants back into the general solution, the final solution is:

$y=\frac{1}{2}xe^{x}+\frac{1}{4}e^{-x}-\frac{1}{4}e^{x}$

---
# 2.
![[Pasted image 20260602142640.png]]
## a.
![[Pasted image 20260602142652.png]]
### Step 0: Classification and Method

This is a second-order linear homogeneous ODE with constant coefficients. The solution method will use the characteristic polynomial.

### Step 1: Finding the Characteristic Polynomial and its Roots

The characteristic polynomial is:

$$p(x)=x^{2}-(a^{2}+1)x+a^{3}-a^{2}+a$$

To factor this polynomial, we look for roots $\lambda_1$ and $\lambda_2$ such that their sum and product match the coefficients:

- $\lambda_1 + \lambda_2 = a^2 + 1$
    
- $\lambda_1 \lambda_2 = a^3 - a^2 + a = a(a^2 - a + 1)$
    

It is easy to see that the roots satisfying these conditions are:

- $\lambda_1 = a$
    
- $\lambda_2 = a^2 - a + 1$
    

### Step 2: Analyzing the Roots

First, we determine when the roots are equal. They are equal if and only if:

$$a = a^2 - a + 1$$

$$a^2 - 2a + 1 = 0$$

$$(a - 1)^2 = 0 \implies a = 1$$

**Case 1: $a = 1$ (Equal Roots)** If $a = 1$, the general solution to the ODE is $y = c_1e^x + c_2xe^x$. We must check the limit as $x \rightarrow -\infty$:

$$\lim_{x\rightarrow-\infty}(c_1e^x + c_2xe^x) = \lim_{x\rightarrow-\infty}\frac{c_1 + c_2x}{e^{-x}}$$

Using L'Hôpital's rule for the second term, this evaluates to $0$. Therefore, $a = 1$ does not satisfy the required condition.

**Case 2: $a \neq 1$ (Distinct Roots)**

For all $a \neq 1$, the general solution is:

$$y = c_1e^{ax} + c_2e^{(a^2-a+1)x}$$

Notice that the expression for the second root, $a^2 - a + 1$, is always strictly positive for any real value of $a$. Because $\lambda_2 > 0$, the limit of the second term as $x \rightarrow -\infty$ is always zero:

$$\lim_{x\rightarrow-\infty}c_2e^{\lambda_2x} = 0$$

Thus, the limit of the entire function depends entirely on the first term, $c_1e^{ax}$. Let's test the remaining possibilities for $a$:

- **If $a > 0$:** Then $\lambda_1 = a > 0$, and $\lim_{x\rightarrow-\infty}c_1e^{\lambda_1x} = 0$. This does not work.
    
- **If $a = 0$:** The limit becomes $\lim_{x\rightarrow-\infty}c_1e^{0 \cdot x} = c_1 \neq \infty$. This does not work.
    
- **If $a < 0$:** We can choose constants where $c_1 > 0$ and $c_2 = 0$. This gives us a valid solution where $\lim_{x\rightarrow-\infty}c_1e^{ax} = \infty$, as required.
    

### Final Answer

A solution $y(x)$ satisfying the given limit exists for **$a < 0$**.

---
## b.
![[Pasted image 20260602143003.png]]

- From our work in part (a), we saw that for all $a \neq 1$, the general solution to the ODE is $y=c_{1}e^{\lambda_{1}x}+c_{2}e^{\lambda_{2}x}$. This solution form consists only of exponential terms and is independent of $xe^{\beta x}$ for any constant.
    
- In contrast, for the case where $a = 1$, the characteristic polynomial has a repeated root ($\lambda = 1$), which changes the structure of the general solution to include an $x$ multiplier.
    
- Specifically, if we choose the constants $c_{1}=0$ and $c_{2}=1$, we get the solution:
    
    $y=xe^{x}$
    
- This perfectly matches the required form $y(x)=xe^{\beta x}$ for the choice of $\beta=1$.
    

### Final Answer

A solution of the specified form exists when **$a = 1$** (which corresponds to $\beta = 1$).

---
# 3.
![[Pasted image 20260602143203.png]]
### Step 0: Classification and Method

We identify that this is a second-order linear non-homogeneous ODE with constant coefficients. The non-homogeneous part can be solved using the method of undetermined coefficients (guessing). Therefore, the steps will be:

1. Find the general solution to the associated homogeneous ODE, $y_h$, using a characteristic polynomial.
    
2. Find a particular solution, $y_p$, by guessing.
    
3. The general solution is the sum of these parts: $y=y_{h}+y_{p}$.
    
4. Determine the specific constants using the initial conditions.
    

### Step 1: Solving the Associated Homogeneous ODE

We begin with the general solution for the associated homogeneous ODE:

$y^{\prime\prime}-2y^{\prime}+y=0$

Its characteristic polynomial is:

$p(\lambda)=\lambda^{2}-2\lambda+1=(\lambda-1)^{2}$

We obtained a double root of $\lambda=1$, which means the functions $y_{1}=e^{x}$ and $y_{2}=xe^{x}$ form a basis for the solution space of the homogeneous ODE. Therefore, the general solution to the homogeneous equation is: $y_{h}=C_{1}e^{x}+C_{2}xe^{x}$

### Step 2: Finding a Particular Solution

We will find a particular solution for the non-homogeneous ODE using the guessing method.

The non-homogeneous part is $f(x)=2e^{x}$, which is a polynomial of degree 0 multiplied by $e^{x}$. This corresponds to $\lambda=1$, which is a root of the characteristic polynomial with a multiplicity of 2. Because of this duplication, we must multiply our standard guess by $x^2$. Our guess takes the form: $y_{p}=\alpha x^{2}e^{x}$

Now, we differentiate this guess:

- $y_{p}^{\prime}=\alpha(x^{2}+2x)e^{x}$
    
- $y_{p}^{\prime\prime}=\alpha(x^{2}+4x+2)e^{x}$
    

Next, substitute these derivatives into the original ODE:

$2e^{x}=\alpha(x^{2}+4x+2)e^{x}-2\alpha(x^{2}+2x)e^{x}+\alpha x^{2}e^{x}$

By combining like terms, we get:

$2e^{x}=[(x^{2}+4x+2)-2(x^{2}+2x)+x^{2}]\alpha e^{x}$ $2e^{x}=2\alpha e^{x}$

From this, we find $\alpha=1$. Therefore, the particular solution is: $y_{p}=x^{2}e^{x}$

### Step 3: The General Solution

The general solution to the non-homogeneous ODE is the sum of our two parts:

$y=y_{p}+y_{h}=x^{2}e^{x}+C_{1}e^{x}+C_{2}xe^{x}$

### Step 4: Applying Initial Conditions

We need to apply the initial conditions to both the function and its derivative. First, we differentiate the general solution: $y^{\prime}=(x^{2}+2x)e^{x}+C_{1}e^{x}+C_{2}(x+1)e^{x}$

Now, we substitute the given initial conditions ($y(0)=2$ and $y^{\prime}(0)=5$):

- $2=y(0)=C_{1}$
    
- $5=y^{\prime}(0)=C_{1}+C_{2}$
    

From the first equation, we immediately see $C_{1}=2$. Substituting this into the second equation gives $5=2+C_{2}$, which means $C_{2}=3$.

### Final Answer

Substituting the constants back into the general solution yields the final answer:

$y=x^{2}e^{x}+2e^{x}+3xe^{x}$


---
# 4.
![[Pasted image 20260602143347.png]]
## a.
![[Pasted image 20260602143359.png]]
**Step 1: Identify the characteristic roots** We recognize that this form of solution comes from a 5th-order linear homogeneous ODE with constant coefficients. Based on the structure of the general solution, we can determine the roots of its characteristic polynomial:

- The constant term $C_1$ corresponds to a root $\lambda_1=0$.
    
- The term $e^{2x}(C_2+C_3x)$ indicates a root $\lambda=2$ with a multiplicity of 2 (hence $\lambda_{2,3}=2$).
    
- The term $e^{-2x}(C_4+C_5x)$ indicates a root $\lambda=-2$ with a multiplicity of 2 (hence $\lambda_{4,5}=-2$).
    

**Step 2: Construct the characteristic polynomial**

Using these roots, the characteristic polynomial is:

$$\lambda(\lambda-2)^{2}(\lambda+2)^{2}=0$$

Now, expand the equation:

$$\lambda((\lambda-2)(\lambda+2))^{2}=0$$

$$\lambda(\lambda^{2}-4)^{2}=0$$

$$\lambda(\lambda^{4}-8\lambda^{2}+16)=0$$

$$\lambda^{5}-8\lambda^{3}+16\lambda=0$$

**Step 3: Write the ODE**

Translating the polynomial back into the corresponding differential equation, we get:

$$y^{(5)}-8y^{(3)}+16y^{\prime}=0$$


---
## b.
![[Pasted image 20260602143520.png]]

**Step 1: Guessing the form for $f_1(x)=4x$** Since $4x$ is a polynomial of degree 1, we would typically guess a polynomial of degree 1: $Ax+B$. However, we must check for duplication with the homogeneous solution. $\lambda=0$ is a root of the characteristic polynomial (with multiplicity 1), meaning a constant term is already part of the homogeneous solution. Therefore, we must multiply our guess by $x$:

$$y_{p1}=x(Ax+B)=Ax^{2}+Bx$$

**Step 2: Guessing the form for $f_2(x)=x\cos(2x)$** This form corresponds to complex roots $\lambda = \alpha \pm \beta i$, where $\alpha=0$ and $\beta=2$. We must check if $\pm 2i$ is a root of our characteristic polynomial. The roots we found earlier were $0, 2,$ and $-2$, so there is no conflict (it is not a root of the characteristic polynomial). Because the trigonometric term is multiplied by $x$ (a polynomial of degree 1), our guess must include a general polynomial of degree 1 for both the cosine and sine terms:

$$y_{p2}=(Cx+D)(E\cos(2x)+F\sin(2x))$$

**Step 3: Combine for the final form**

The full form of the particular solution is simply the sum of our two guesses:

$$y_{p}=y_{p1}+y_{p2}=Ax^{2}+Bx+(Cx+D)(E\cos(2x)+F\sin(2x))$$

---
# 5.
![[Pasted image 20260602143743.png]]
## a.
![[Pasted image 20260602143756.png]]
**Step 1: Apply Kirchhoff's Current Law (KCL)**

According to the given KCL equation for the circuit:

$i_{R}+i_{C}+i_{L}=i_{s}$

**Step 2: Substitute the component relations**

We are given the physical relations for the resistor and capacitor: $i_{R}=\frac{v}{R}$ and $i_{C}=Cv^{\prime}$. Substituting these into the KCL equation gives:

$\frac{v}{R}+Cv^{\prime}+i_{L}=i_{s}$

**Step 3: Differentiate the equation**

To get an equation exclusively in terms of $v(t)$, we need to eliminate $i_L$. We do this by differentiating the entire equation with respect to time ($t$). Since $i_{s}$ is a constant current source, its derivative is $0$:

$\frac{1}{R}v^{\prime}+Cv^{\prime\prime}+i_{L}^{\prime}=0$

**Step 4: Express the inductor current derivative in terms of voltage**

In a parallel circuit, the voltage across the inductor is the common voltage $v(t)$. Using the given inductor relation $v_{L}=Li_{L}^{\prime}$, we have:

$v=Li_{L}^{\prime}$

Which implies:

$i_{L}^{\prime}=\frac{v}{L}$

**Step 5: Substitute and rearrange into standard form**

Substitute $i_{L}^{\prime}$ back into our differentiated equation:

$\frac{1}{R}v^{\prime}+Cv^{\prime\prime}+\frac{v}{L}=0$

Finally, rearrange the terms and divide by $C$ to present the ODE in its standard form:

$v^{\prime\prime}+\frac{1}{RC}v^{\prime}+\frac{1}{LC}v=0$

### Final Answer

The second-order ODE for $v(t)$ is **$v^{\prime\prime}+\frac{1}{RC}v^{\prime}+\frac{1}{LC}v=0$**. This is a second-order linear homogeneous ODE.

---
## b.
![[Pasted image 20260602143833.png]]
**Step 1: Identify the given initial voltage**

From the problem description, we are explicitly given the initial condition for the voltage:

$v(0^+) = v_0$

**Step 2: Relate the derivative of voltage to current** To find $v'(0^+)$, we need to use the physical relationship for the capacitor: $i_C = Cv'$

Rearranging this to solve for $v'(0^+)$ gives:

$v'(0^+) = \frac{i_C(0^+)}{C}$

**Step 3: Find the initial capacitor current using KCL** We can find $i_C(0^+)$ by applying Kirchhoff's Current Law (KCL) at the initial moment $t=0^+$: $i_C(0^+) = i_s - i_L(0^+) - i_R(0^+)$

**Step 4: Substitute known initial values into the KCL equation** We are given that the initial current through the inductor is $i_L(0^+) = i_0$. Additionally, we know the initial current through the resistor depends on the initial voltage: $i_R(0^+) = \frac{v(0^+)}{R} = \frac{v_0}{R}$

Substituting both of these into our KCL equation yields: $i_C(0^+) = i_s - i_0 - \frac{v_0}{R}$

**Step 5: Final calculation for $v'(0^+)$**

Now, substitute the expression for $i_C(0^+)$ back into our equation from Step 2:

$v'(0^+) = \frac{i_s - i_0 - \frac{v_0}{R}}{C}$

### Final Answer

The initial conditions for the ODE are:

1. **$v(0^+) = v_0$**
    
2. **$v'(0^+) = \frac{i_s - i_0 - \frac{v_0}{R}}{C}$**

---
## c.
![[Pasted image 20260602143921.png]]
**Step 1: Identify the characteristic polynomial** From the homogeneous ODE found in part 'a', $v^{\prime\prime}+\frac{1}{RC}v^{\prime}+\frac{1}{LC}v=0$, we can write the characteristic polynomial: $r^{2}+\frac{1}{RC}r+\frac{1}{LC}=0$

**Step 2: Determine the condition for no oscillations** For the voltage to decay without oscillations, the system must be either overdamped or critically damped. Mathematically, this means the roots of the characteristic polynomial must be real and negative. For the roots of a quadratic equation to be real, its discriminant ($\Delta$) must be greater than or equal to zero: $\Delta \ge 0$

**Step 3: Set up and solve the inequality**

Applying the discriminant formula ($b^2 - 4ac \ge 0$) to our polynomial:

$\left(\frac{1}{RC}\right)^{2}-4\left(\frac{1}{LC}\right)\ge0$

This simplifies to:

$\frac{1}{R^{2}C^{2}}\ge\frac{4}{LC}$

To isolate $L$, we can multiply both sides by $R^{2}C^{2}LC$ (which is strictly positive): $L\ge4R^{2}C$

### Final Answer

The voltage will decay without oscillations when the condition **$L \ge 4R^{2}C$** is met.

---
# d.
![[Pasted image 20260602143951.png]]
**Step 1: Construct the New ODE**

According to Kirchhoff's Current Law (KCL), the equation is:

$\frac{v}{R}+Cv^{\prime}+i_{L}=i_{s}(t)$

Substitute the given component values and the new current source into the equation:

$5v+v^{\prime}+i_{L}=1-e^{-t}$

To eliminate $i_L$, differentiate the entire equation with respect to time:

$5v^{\prime}+v^{\prime\prime}+i_{L}^{\prime}=e^{-t}$

From the inductor's relation ($v=Li_{L}^{\prime}$), we can isolate $i_{L}^{\prime}$:

$i_{L}^{\prime}=\frac{v}{L}=6v$

Substitute this back into our differentiated equation to get the new ODE:

$v^{\prime\prime}+5v^{\prime}+6v=e^{-t}$

**Step 2: Find the Initial Conditions** We are explicitly given $v(0)=0$ and $i_{L}(0)=0$. To find the initial condition for the derivative, $v^{\prime}(0)$, substitute $t=0$ and the known initial values into the un-differentiated KCL equation from Step 1 ($5v+v^{\prime}+i_{L}=1-e^{-t}$): $5(0)+v^{\prime}(0)+0=1-e^{-0}$ $v^{\prime}(0)=0$

So, our initial conditions are $v(0)=0$ and $v^{\prime}(0)=0$.

**Step 3: Solve the Homogeneous ODE**

The homogeneous part of our new ODE is:

$v^{\prime\prime}+5v^{\prime}+6v=0$

Its characteristic polynomial is:

$r^{2}+5r+6=0$

This factors easily:

$(r+2)(r+3)=0$

The roots are $r_{1}=-2$ and $r_{2}=-3$. Therefore, the homogeneous solution is: $v_{h}=C_{1}e^{-2t}+C_{2}e^{-3t}$

**Step 4: Find the Particular Solution**

Since the right-hand side of the non-homogeneous equation is $e^{-t}$, we guess a particular solution of the form:

$v_{p}=Ae^{-t}$

Differentiate this guess:

- $v_{p}^{\prime}=-Ae^{-t}$
    
- $v_{p}^{\prime\prime}=Ae^{-t}$
    

Substitute these into the non-homogeneous ODE ($v^{\prime\prime}+5v^{\prime}+6v=e^{-t}$):

$Ae^{-t}+5(-Ae^{-t})+6Ae^{-t}=e^{-t}$ $(1-5+6)Ae^{-t}=e^{-t}$ $2A=1 \implies A=\frac{1}{2}$

So the particular solution is:

$v_{p}=\frac{1}{2}e^{-t}$

**Step 5: Form the General Solution and Find Constants**

The general solution is the sum of the homogeneous and particular parts:

$v(t)=C_{1}e^{-2t}+C_{2}e^{-3t}+\frac{1}{2}e^{-t}$

Now apply the initial conditions to find the constants. First, apply $v(0)=0$:

$C_{1}+C_{2}+\frac{1}{2}=0 \implies C_{1}+C_{2}=-\frac{1}{2}$

Next, find the derivative of the general solution:

$v^{\prime}(t)=-2C_{1}e^{-2t}-3C_{2}e^{-3t}-\frac{1}{2}e^{-t}$

Apply the second initial condition, $v^{\prime}(0)=0$:

$-2C_{1}-3C_{2}-\frac{1}{2}=0 \implies 2C_{1}+3C_{2}=-\frac{1}{2}$

We now have a system of two equations:

1. $C_{1}+C_{2}=-\frac{1}{2}$
    
2. $2C_{1}+3C_{2}=-\frac{1}{2}$
    

Solving this system yields $C_{1}=-1$ and $C_{2}=\frac{1}{2}$.

### Final Answer

Substituting the constants back into the general solution gives the final, specific solution for the voltage:

**$v(t)=\frac{1}{2}e^{-t}-e^{-2t}+\frac{1}{2}e^{-3t}$**