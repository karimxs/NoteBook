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
