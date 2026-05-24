# 1.
![[Pasted image 20260524143636.png]]
## a.
### 1. Reflexive: Yes

**Proof:** Let $x \in \mathbb{N}$. We can choose the natural number $a = 1$. It is clear that $1 \in \mathbb{N}$ and the equation $x = 1 \cdot x$ holds true. Therefore, by the definition of the relation, $xR_1x$ is satisfied.

### 2. Symmetric: No

**Disproof:** Let's use a counterexample. Choose $x = 2$ and $y = 1$. The relation $2R_11$ holds because $2 = 2 \cdot 1$ (where $a = 2 \in \mathbb{N}$). However, $1R_12$ does not hold, because there is no natural number $a \in \mathbb{N}$ that satisfies the equation $1 = a \cdot 2$.

### 3. Anti-symmetric: Yes

**Proof:** Assume that $xR_1y$ and $yR_1x$. According to the definition of the relation, there exist natural numbers $a, b \in \mathbb{N}$ such that:

$$x = a \cdot y$$

$$y = b \cdot x$$

Substituting the second equation into the first yields:

$$x = a \cdot (b \cdot x) = (a \cdot b) \cdot x$$

- If your course defines the natural numbers as including zero ($0 \in \mathbb{N}$) and $x = 0$, then from the equation $y = b \cdot x$ we get $y = 0$, meaning $x = y$.

- If $x \neq 0$, we can divide both sides of the equation by $x$ to get $1 = a \cdot b$. Since both $a$ and $b$ are natural numbers, the only solution to this equation is $a = 1$ and $b = 1$.


Substituting $a = 1$ back into the original equation gives $x = 1 \cdot y$, which means $x = y$.

### 4. Transitive: Yes

**Proof:** Assume that $xR_1y$ and $yR_1z$. According to the definition, there exist natural numbers $a, b \in \mathbb{N}$ such that:

$$x = a \cdot y$$

$$y = b \cdot z$$

Substitute $y$ into the first equation:

$$x = a \cdot (b \cdot z) = (a \cdot b) \cdot z$$

Since the set of natural numbers is closed under multiplication, the product of $a$ and $b$ is necessarily a natural number. Let's denote $c = a \cdot b$ (where $c \in \mathbb{N}$). We have obtained $x = c \cdot z$, and therefore, by the definition of the relation, $xR_1z$ holds.

---
## b.

### 1. Reflexive: Always holds

**Proof:** Since we are given that $F$ is a non-empty set ($F \neq \emptyset$), there is at least one function $f \in F$. For any $x \in \mathbb{N}$, it is trivially true that $f(x) = f(x)$. Therefore, there exists a function in $F$ that satisfies the condition, meaning $xR_2x$ always holds for every $x \in \mathbb{N}$.

### 2. Symmetric: Always holds

**Proof:** Assume that $xR_2y$. By the definition of the relation, there exists some function $f \in F$ such that $f(x) = f(y)$. Because mathematical equality is symmetric, we can rewrite this as $f(y) = f(x)$. This means the exact same function $f$ satisfies the condition for $y$ and $x$, therefore $yR_2x$ always holds.

### 3. Anti-symmetric: Sometimes holds, sometimes doesn't

**Proof by examples:** To show it sometimes holds and sometimes doesn't, we will provide two different sets of functions ($F_1$ and $F_2$).

**Example where it DOES hold ($F_1$):**

Let $F_1 = \{id\}$, a set containing only the identity function defined by $id(n) = n$ for all $n \in \mathbb{N}$. If $xR_2y$ and $yR_2x$, it means $id(x) = id(y)$, which simplifies exactly to $x = y$. For this choice of $F$, the relation is anti-symmetric.

**Example where it DOES NOT hold ($F_2$):**

Let $F_2 = \{c\}$, a set containing only a constant function defined by $c(n) = 1$ for all $n \in \mathbb{N}$. Here, $1R_22$ holds (because $c(1) = c(2) = 1$) and $2R_21$ holds. However, $1 \neq 2$. Therefore, for this choice of $F$, the relation is not anti-symmetric.

### 4. Transitive: Sometimes holds, sometimes doesn't

**Proof by examples:** Again, we will provide two different sets of functions.

**Example where it DOES hold ($F_1$):**

We can reuse $F_1 = \{id\}$ where $id(n) = n$. Since $xR_2y$ simply means $x = y$, the relation is standard equality, which is perfectly transitive. (If $x=y$ and $y=z$, then $x=z$).

**Example where it DOES NOT hold ($F_2$):**

Let $F_2 = \{f, g\}$, a set containing two specific functions defined as follows:

$f(n) = 1$ for $n \in \{1, 2\}$, and $f(n) = n$ for all other $n$.

$g(n) = 2$ for $n \in \{2, 3\}$, and $g(n) = n$ for all other $n$.

Now let's check the transitivity condition for the elements 1, 2, and 3:

$1R_22$ holds because $f(1) = 1$ and $f(2) = 1$ (thus $f(1) = f(2)$).

$2R_23$ holds because $g(2) = 2$ and $g(3) = 2$ (thus $g(2) = g(3)$).

For the relation to be transitive, $1R_23$ must hold, meaning there must be some function in $F_2$ where the output for 1 equals the output for 3. Let's check both functions in our set:

$f(1) = 1$ and $f(3) = 3$. ($1 \neq 3$)

$g(1) = 1$ and $g(3) = 2$. ($1 \neq 2$)

Since neither function maps 1 and 3 to the same value, $1R_23$ is false. Therefore, for this choice of $F$, the relation is not transitive.

---
# 2.
![[Pasted image 20260524144127.png]]
## a.
### 1. Equivalence Classes for $R_1$

The relation $R_1$ on $\mathbb{N}$ is defined as: $xR_1y$ if and only if $xy$ is odd OR $x=y$.

The product $xy$ is odd if and only if **both** $x$ and $y$ are odd numbers. Based on this, we can divide the natural numbers into two types of equivalence classes:

- **The class of all odd numbers:** Let $x$ be an odd number. For any other odd number $y$, the product $xy$ will be odd, so $xR_1y$ holds. If $y$ is an even number, $xy$ is even, so they can only be related if $x=y$, which is impossible since an odd number cannot equal an even number. Therefore, all odd numbers are related to each other, and to nothing else. This forms one single equivalence class:
    
    $$[1]_{R_1} = \{1, 3, 5, 7, 9, ...\} = \{x \in \mathbb{N} \mid x \text{ is odd}\}$$
    
- **The singleton classes of even numbers:** Let $x$ be an even number. For any natural number $y$, the product $xy$ will be even. Therefore, the condition "$xy$ is odd" is never met. The only way for $xR_1y$ to hold is the second condition: $x=y$. This means an even number is only related to itself. Therefore, every even number forms its own equivalence class of size 1:
    
    $$[2k]_{R_1} = \{2k\} \text{ for every even number } 2k \in \mathbb{N}$$
    

### 2. Equivalence Classes for $R_2$

The relation $R_2$ on $\mathbb{Z}$ is defined as: $xR_2y$ if and only if there exists $a \in \mathbb{Z}$ and $b,c \in \{0,...,6\}$ such that $x=7a+b$ and $y=7a+c$.

According to the Division Algorithm, every integer can be uniquely written in the form $7a + r$, where $a$ is the quotient and $r \in \{0,...,6\}$ is the remainder. The relation $xR_2y$ essentially states that $x$ and $y$ yield the **same quotient** ($a$) when divided by 7 (their remainders, $b$ and $c$, can be different).

Therefore, two integers are related if they belong to the same "block" of 7 consecutive numbers defined by a specific quotient $a$.

- **The equivalence classes:** For each integer $a \in \mathbb{Z}$, there is an equivalence class consisting of the 7 integers that share that quotient. The classes can be defined as:
    
    $$[7a]_{R_2} = \{7a, 7a+1, 7a+2, 7a+3, 7a+4, 7a+5, 7a+6\}$$
    

**Examples of these classes:**

- For $a=0$: $\{0, 1, 2, 3, 4, 5, 6\}$
    
- For $a=1$: $\{7, 8, 9, 10, 11, 12, 13\}$
    
- For $a=-1$: $\{-7, -6, -5, -4, -3, -2, -1\}$
    

There are infinitely many such classes, one for every integer $a \in \mathbb{Z}$.

---
## b.
### **1. Equivalence Classes for $R_1$**

The relation $R_1$ on $\mathbb{N}$ is defined as: $xR_1y$ if and only if $xy$ is odd or $x=y$.

For the product $xy$ to be odd, **both** $x$ and $y$ must be odd numbers. This gives us two distinct types of equivalence classes:

- **The Odd Numbers Class:** If $x$ is an odd number, multiplying it by any other odd number $y$ results in an odd product, satisfying $xR_1y$. If $y$ is even, $xy$ is even, meaning $x$ and $y$ can only be related if $x=y$ (which is impossible since one is odd and the other is even). Therefore, all odd numbers are related to each other and form a single, infinitely large equivalence class:
    
    $$[1]_{R_1} = \{x \in \mathbb{N} \mid x \text{ is odd}\} = \{1, 3, 5, 7, 9, \dots\}$$
    
- **The Even Numbers Classes (Singletons):** If $x$ is an even number, the product $xy$ will always be even for any $y \in \mathbb{N}$. Therefore, the first condition ("$xy$ is odd") can never be met. The only way for an even number $x$ to relate to $y$ is through the second condition: $x=y$. This means every even number is related _only_ to itself, forming an infinite number of singleton equivalence classes (classes of size 1):
    
    $$[2k]_{R_1} = \{2k\} \quad \text{for every even number } 2k \in \mathbb{N}$$
    

### **2. Equivalence Classes for $R_2$**

The relation $R_2$ on $\mathbb{Z}$ is defined as: $xR_2y$ if and only if there exists $a \in \mathbb{Z}$ and $b,c \in \{0, \dots, 6\}$ such that $x=7a+b$ and $y=7a+c$.

By the standard Division Algorithm, any integer can be uniquely expressed as $7a + r$, where $a$ is the integer quotient and $r \in \{0, \dots, 6\}$ is the remainder. The relation $xR_2y$ means that $x$ and $y$ share the exact same quotient ($a$) when divided by 7, regardless of their remainders.

- **The Equivalence Classes:**
    
    Two integers are in the same equivalence class if and only if they have the same quotient $a$. Thus, for every integer $a \in \mathbb{Z}$, there is a corresponding equivalence class containing exactly 7 consecutive integers:
    
    $$[7a]_{R_2} = \{7a, 7a+1, 7a+2, 7a+3, 7a+4, 7a+5, 7a+6\}$$
    

**Examples:**

- For $a = 0$: The class is $\{0, 1, 2, 3, 4, 5, 6\}$
    
- For $a = 1$: The class is $\{7, 8, 9, 10, 11, 12, 13\}$
    
- For $a = -1$: The class is $\{-7, -6, -5, -4, -3, -2, -1\}$

---
# 3.
![[Pasted image 20260524144429.png]]
## a.
Let $A$ be a non-empty set and $f: A \rightarrow A$ be a function.

The relation $R_f$ on $A$ is defined as: $x R_f y$ if and only if $y = f(x)$.

**The Claim:** If $R_f$ is transitive, then $f \circ f = I_A$ (where $I_A$ is the identity function, meaning $f(f(x)) = x$ for all $x$).

**Verdict: The claim is FALSE.**

### **Disproof by Counterexample:**

To disprove the claim, we need to find a set $A$ and a function $f$ where the relation $R_f$ is transitive, but the composition $f \circ f$ does not equal the identity function $I_A$.

Let $A = \{1, 2\}$.

Let's define the function $f: A \rightarrow A$ such that it maps everything to 2:

- $f(1) = 2$
    
- $f(2) = 2$
    

Now, let's analyze the relation $R_f$ generated by this function. Based on the definition $y = f(x)$, the relation contains the following pairs:

$$R_f = \{(1, 2), (2, 2)\}$$

**Verify that $R_f$ is transitive.**

A relation is transitive if whenever $(x, y) \in R_f$ and $(y, z) \in R_f$, then $(x, z) \in R_f$. Let's check all possible chains in our relation:

- We have $(1, 2)$ and $(2, 2)$. The result must be $(1, 2)$, which is indeed in $R_f$.
    
- We have $(2, 2)$ and $(2, 2)$. The result must be $(2, 2)$, which is indeed in $R_f$.
    
    Since all chains satisfy the condition, **$R_f$ is transitive.**
    

**Check if $f \circ f = I_A$.**

The identity function $I_A$ on our set would require $I_A(1) = 1$ and $I_A(2) = 2$.

Let's calculate $f \circ f$ for the input $1$:

$$(f \circ f)(1) = f(f(1)) = f(2) = 2$$

Since $(f \circ f)(1) = 2$, but $I_A(1) = 1$, we can clearly see that $f \circ f \neq I_A$.

**Conclusion:** We have found a valid function where $R_f$ is transitive, yet $f \circ f \neq I_A$. Therefore, the general claim is false.

---
## b.
 Let $A$ be a non-empty set and $f: A \rightarrow A$ be a function. The relation $R_f$ on $A$ is defined as: $x R_f y$ if and only if $y = f(x)$.

**The Claim:** If $R_f$ is symmetric, then $f \circ f = I_A$ (where $I_A$ is the identity function on $A$, meaning $f(f(x)[cite_start]) = x$ for all $x \in A$ ).

**Verdict: The claim is TRUE.**

### **Proof:**

1. Let $x$ be an arbitrary element in the set $A$ ($x \in A$).
    
2. Let $y$ be the image of $x$ under the function $f$, meaning we define $y = f(x)$.
    
3. By the definition of the relation, since $y = f(x)$, it holds that $x R_f y$.
    
4. We are given the premise that the relation $R_f$ is symmetric. By the definition of symmetry, if $x R_f y$ holds, then $y R_f x$ must also hold.
    
5. According to the definition of our relation, the statement $y R_f x$ translates exactly to the equation $x = f(y)$.
    
6. Now, we take the equation $x = f(y)$ and substitute $y$ with our original definition $y = f(x)$:
    
    $$x = f(f(x))$$
    
7. This can be rewritten using function composition notation as $(f \circ f)(x) = x$.
    
8. Because we chose $x$ to be an arbitrary element in $A$, this equation holds for every element in the set. Therefore, the composition of $f$ with itself is indeed the identity function: $f \circ f = I_A$.

---
# 4.
![[Pasted image 20260524144711.png]]
## a.

The function $f: \mathbb{Z} \rightarrow \mathbb{N}^2$ is defined as:

$$f(z) = \begin{cases} (z, 0) & z \ge 0 \\ (-z, 1) & z < 0 \end{cases}$$

**Injective (One-to-One):** Yes. Suppose $f(z_1) = f(z_2)$.

If the resulting image has $0$ as the second coordinate, then both inputs must be non-negative ($z_1, z_2 \ge 0$). This gives $(z_1, 0) = (z_2, 0)$, which means $z_1 = z_2$.

If the resulting image has $1$ as the second coordinate, then both inputs must be negative ($z_1, z_2 < 0$). This gives $(-z_1, 1) = (-z_2, 1)$, meaning $-z_1 = -z_2$, so $z_1 = z_2$.

A case where one maps to $0$ and the other to $1$ is impossible since $0 \neq 1$.

**Surjective (Onto):** No. The codomain is $\mathbb{N}^2$ (all ordered pairs of natural numbers). Consider the element $(1, 2) \in \mathbb{N}^2$. There is no integer $z \in \mathbb{Z}$ that satisfies $f(z) = (1, 2)$ because the second coordinate of the output can only ever be $0$ or $1$.

**Invertible:** No, because the function is not surjective (a function must be both injective and surjective to be invertible).

---
## b.

Let $A, U$ be non-empty sets where $A \subseteq U$.

The function $f: \mathcal{P}(U) \rightarrow \mathcal{P}(U)$ is defined by $f(B) = A \cup B$ for all $B \subseteq U$.

**Injective (One-to-One):** No. Because $A$ is explicitly stated to be non-empty, we can pick two distinct sets from the domain: $B_1 = A$ and $B_2 = \emptyset$. Clearly, $B_1 \neq B_2$. However, plugging them into the function yields:

$f(B_1) = A \cup A = A$

$f(B_2) = A \cup \emptyset = A$

Since $f(B_1) = f(B_2)$, the function is not injective.

**Surjective (Onto):** No. The target codomain is the power set $\mathcal{P}(U)$, which contains the empty set $\emptyset$. For any input $B$, the output is $A \cup B$. Since $A$ is non-empty, the union $A \cup B$ will always contain at least the elements of $A$ and can therefore never be the empty set. Thus, $\emptyset$ has no pre-image.

**Invertible:** No, because it is neither injective nor surjective.

---
## c.

Let $A \neq \emptyset$.

The function $f: A \rightarrow \mathcal{P}(\mathcal{P}(A))$ is defined by $f(a) = \{B \in \mathcal{P}(A) \mid a \in B\}$.

**Injective (One-to-One):** Yes. Let $a_1, a_2 \in A$ such that $a_1 \neq a_2$. Consider the singleton set $\{a_1\}$, which is an element of $\mathcal{P}(A)$. Because $a_1 \in \{a_1\}$, the definition of our function dictates that $\{a_1\} \in f(a_1)$. However, because $a_1 \neq a_2$, the element $a_2$ is not in the set $\{a_1\}$, meaning $\{a_1\} \notin f(a_2)$. Since $f(a_1)$ contains an element that $f(a_2)$ does not, $f(a_1) \neq f(a_2)$.

**Surjective (Onto):** No. By Cantor's Theorem, the cardinality of any set is strictly less than the cardinality of its power set. Therefore, $|A| < |\mathcal{P}(A)| < |\mathcal{P}(\mathcal{P}(A))|$. Since the domain is strictly smaller than the codomain, no surjective mapping can exist.

(Alternative proof: The empty set $\emptyset \in \mathcal{P}(\mathcal{P}(A))$ has no pre-image because for any $a$, the output set $f(a)$ will always contain at least the set $\{a\}$, meaning $f(a)$ is never empty).

**Invertible:** No, because it is not surjective.

---
# 5.
![[Pasted image 20260524145059.png]]
Let $A$ and $B$ be sets such that $A \sim B$. By the definition of equipollence (having the same cardinality), there exists a bijective function $f: A \rightarrow B$.

We need to prove that $\mathcal{P}(A) \sim \mathcal{P}(B)$, which means we must construct a bijective function $F: \mathcal{P}(A) \rightarrow \mathcal{P}(B)$.

Let us define the function $F$ such that for any subset $X \subseteq A$ (meaning $X \in \mathcal{P}(A)$), the output is the direct image of $X$ under the function $f$:

$$F(X) = \{f(x) \mid x \in X\}$$

To prove this forms a bijection, we must show that $F$ is both injective and surjective.

**Injective (One-to-One):**

Suppose $F(X_1) = F(X_2)$ for some subsets $X_1, X_2 \in \mathcal{P}(A)$.

Let $x$ be an arbitrary element in $X_1$. This means $f(x) \in F(X_1)$.

Since $F(X_1) = F(X_2)$, it follows that $f(x) \in F(X_2)$.

By the definition of our function $F$, this means there must exist some element $y \in X_2$ such that $f(x) = f(y)$.

Because the original function $f$ is known to be a bijection, it is injective. This means $f(x) = f(y)$ implies $x = y$.

Since $y \in X_2$ and $x = y$, it follows that $x \in X_2$. Thus, we have shown that every element in $X_1$ is also in $X_2$, meaning $X_1 \subseteq X_2$.

By applying the exact same logic in reverse (starting with an element in $X_2$), we can show $X_2 \subseteq X_1$.

Since $X_1 \subseteq X_2$ and $X_2 \subseteq X_1$, we conclude that $X_1 = X_2$. This proves that $F$ is injective.

**Surjective (Onto):**

Let $Y$ be an arbitrary element of the codomain, meaning $Y \subseteq B$ ($Y \in \mathcal{P}(B)$).

We need to find a pre-image set $X \in \mathcal{P}(A)$ such that $F(X) = Y$.

Let $X$ be the pre-image of the set $Y$ under the original function $f$, defined as:

$$X = \{a \in A \mid f(a) \in Y\}$$

Because $X$ consists only of elements from $A$, it is clear that $X \subseteq A$, so $X \in \mathcal{P}(A)$.

Now let's apply our function $F$ to this set $X$:

$$F(X) = \{f(x) \mid x \in X\} = \{f(x) \mid f(x) \in Y\}$$

Because the original function $f$ is surjective, every element $y \in Y$ has at least one corresponding element $x \in A$ such that $f(x) = y$. Thus, the collection of all outputs $\{f(x) \mid f(x) \in Y\}$ exactly reconstructs the entire set $Y$.

This means $F(X) = Y$, proving that every possible subset $Y$ in the codomain has a pre-image. Therefore, $F$ is surjective.

**Conclusion:**

Since we have successfully constructed a function $F: \mathcal{P}(A) \rightarrow \mathcal{P}(B)$ and proven it is both injective and surjective, $F$ is a bijection. Therefore, the power sets share the same cardinality, and $\mathcal{P}(A) \sim \mathcal{P}(B)$ holds true.