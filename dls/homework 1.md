# 1.
![[Pasted image 20260502130728.png]]
## a.
![[Pasted image 20260502130740.png]]
### **Base 10**

$$(101010.11)_2 = 2^5 + 2^3 + 2^1 + 2^{-1} + 2^{-2}$$

$$= 32 + 8 + 2 + 0.5 + 0.25 = (42.75)_{10}$$


### **Base 4**

$$42 \div 4 = 10 \rightarrow R=2$$

$$10 \div 4 = 2 \rightarrow R=2$$

$$2 \div 4 = 0 \rightarrow R=2$$

$$0.75 \times 4 = 3.0 \rightarrow I=3$$

$$(222.3)_4$$


### **Base 8**

$$42 \div 8 = 5 \rightarrow R=2$$

$$5 \div 8 = 0 \rightarrow R=5$$

$$0.75 \times 8 = 6.0 \rightarrow I=6$$

$$(52.6)_8$$


### **Base 16**

$$42 \div 16 = 2 \rightarrow R=10 (A)$$

$$2 \div 16 = 0 \rightarrow R=2$$

$$0.75 \times 16 = 12.0 \rightarrow I=12 (C)$$

$$(2A.C)_{16}$$

---
## b.
![[Pasted image 20260502133848.png]]
$$3^2 = 9 \implies \text{2 digits (Base 3)} \rightarrow \text{1 digit (Base 9)}$$

$$(121.22)_3 = (\underline{01} \;\; \underline{21} \;\; . \;\; \underline{22})_3$$

**Integer:**

$$(\underline{01})_3 = 0 \cdot 3^1 + 1 \cdot 3^0 = 1$$

$$(\underline{21})_3 = 2 \cdot 3^1 + 1 \cdot 3^0 = 7$$

**Fraction:**

$$(\underline{22})_3 = 2 \cdot 3^1 + 2 \cdot 3^0 = 8$$

**Result:**

$$(17.8)_9$$

---
## c.
![[Pasted image 20260502134314.png]]


$$9 = 3^2 \implies \text{1 digit (Base 9)} \rightarrow \text{2 digits (Base 3)}$$

**Integer:**

$$8 \rightarrow 2 \cdot 3^1 + 2 \cdot 3^0 \rightarrow (22)_3$$

$$7 \rightarrow 2 \cdot 3^1 + 1 \cdot 3^0 \rightarrow (21)_3$$

**Fraction:**

$$5 \rightarrow 1 \cdot 3^1 + 2 \cdot 3^0 \rightarrow (12)_3$$

**Result:**

$$(2221.12)_3$$

---
## d.
![[Pasted image 20260502134528.png]]

### **Base 2**

**Integer:**

$$47 \div 2 = 23 \rightarrow R=1$$

$$23 \div 2 = 11 \rightarrow R=1$$

$$11 \div 2 = 5 \rightarrow R=1$$

$$5 \div 2 = 2 \rightarrow R=1$$

$$2 \div 2 = 1 \rightarrow R=0$$

$$1 \div 2 = 0 \rightarrow R=1$$

$$\implies (101111)_2$$

**Fraction:**

$$0.9 \times 2 = 1.8 \rightarrow I=1$$

$$0.8 \times 2 = 1.6 \rightarrow I=1$$

$$0.6 \times 2 = 1.2 \rightarrow I=1$$

$$0.2 \times 2 = 0.4 \rightarrow I=0$$

$$0.4 \times 2 = 0.8 \rightarrow I=0$$

$$0.8 \times 2 = 1.6 \rightarrow I=1$$

_(Repeats)_ $\implies (.111001100...)_2$

**Result:**

$$(101111.111001100...)_2$$


### **Base 8**

Group Base 2 by 3 digits.

**Integer:**

$$(\underline{101} \;\; \underline{111})_2 \implies (57)_8$$

**Fraction:**

$$(.\underline{111} \;\; \underline{001} \;\; \underline{100} \;\; \underline{110} \;\; \underline{011} ...)_2 \implies (.71463...)_8$$

**Result:**

$$(57.71463...)_8$$

---

### **Base 16**

Group Base 2 by 4 digits.

**Integer:**

$$(\underline{0010} \;\; \underline{1111})_2 \implies (2F)_{16}$$

**Fraction:**

$$(.\underline{1110} \;\; \underline{0110} \;\; \underline{0110} ...)_2 \implies (.E66...)_{16}$$

**Result:**

$$(2F.E66...)_{16}$$

---
## e.
![[Pasted image 20260502134904.png]]


$$256 \div 2 = 128 \rightarrow R=0$$

$$128 \div 2 = 64 \rightarrow R=0$$

$$64 \div 2 = 32 \rightarrow R=0$$

$$32 \div 2 = 16 \rightarrow R=0$$

$$16 \div 2 = 8 \rightarrow R=0$$

$$8 \div 2 = 4 \rightarrow R=0$$

$$4 \div 2 = 2 \rightarrow R=0$$

$$2 \div 2 = 1 \rightarrow R=0$$

$$1 \div 2 = 0 \rightarrow R=1$$

$$(100000000)_2$$

---

## e.
![[Pasted image 20260502135015.png]]

**Base 10:**

$$6 \cdot 8^3 + 2 \cdot 8^2 + 5 \cdot 8^1 + 3 \cdot 8^0 + 4 \cdot 8^{-1} + 7 \cdot 8^{-2} + 6 \cdot 8^{-3}$$

$$= 3072 + 128 + 40 + 3 + 0.5 + 0.109375 + 0.01171875$$

$$(3243.621)_{10}$$

**Base 2 (Intermediate):**

$$6 \rightarrow 110, \quad 2 \rightarrow 010, \quad 5 \rightarrow 101, \quad 3 \rightarrow 011$$

$$4 \rightarrow 100, \quad 7 \rightarrow 111, \quad 6 \rightarrow 110$$

$$(110010101011.100111110)_2$$

**Base 4:**

$$2^2 = 4 \implies \text{Group Base 2 by 2 digits}$$

$$(\underline{11} \;\; \underline{00} \;\; \underline{10} \;\; \underline{10} \;\; \underline{10} \;\; \underline{11} \;\; . \;\; \underline{10} \;\; \underline{01} \;\; \underline{11} \;\; \underline{11} \;\; \underline{00})_2$$

$$(302223.2133)_4$$

**Base 16:**

$$2^4 = 16 \implies \text{Group Base 2 by 4 digits}$$

$$(\underline{1100} \;\; \underline{1010} \;\; \underline{1011} \;\; . \;\; \underline{1001} \;\; \underline{1111} \;\; \underline{0000})_2$$

$$(CAB.9F)_{16}$$

---
## f.
![[Pasted image 20260502135822.png]]

$$9 = 3^2 \implies \text{1 digit (Base 9)} \rightarrow \text{2 digits (Base 3)}$$

**Integer:**

$$2 \rightarrow 0 \cdot 3^1 + 2 \cdot 3^0 \rightarrow (02)_3$$

$$3 \rightarrow 1 \cdot 3^1 + 0 \cdot 3^0 \rightarrow (10)_3$$

$$8 \rightarrow 2 \cdot 3^1 + 2 \cdot 3^0 \rightarrow (22)_3$$

$$5 \rightarrow 1 \cdot 3^1 + 2 \cdot 3^0 \rightarrow (12)_3$$

**Fraction:**

$$1 \rightarrow 0 \cdot 3^1 + 1 \cdot 3^0 \rightarrow (01)_3$$

$$4 \rightarrow 1 \cdot 3^1 + 1 \cdot 3^0 \rightarrow (11)_3$$

$$5 \rightarrow 1 \cdot 3^1 + 2 \cdot 3^0 \rightarrow (12)_3$$

**Result:**

$$(2102212.011112)_3$$

---
## g.
![[Pasted image 20260502140924.png]]
### **Base 10**

$$1 \cdot 2^5 + 1 \cdot 2^2 + 1 \cdot 2^1 + 1 \cdot 2^0 + 1 \cdot 2^{-2}$$

$$= 32 + 4 + 2 + 1 + 0.25$$

$$(39.25)_{10}$$

---

### **Base 4**

$$2^2 = 4 \implies \text{Group Base 2 by 2}$$

$$(\underline{10} \;\; \underline{01} \;\; \underline{11} \;\; . \;\; \underline{01})_2$$

$$(213.1)_4$$

---

### **Base 8**

$$2^3 = 8 \implies \text{Group Base 2 by 3 (Pad with 0s)}$$

$$(\underline{100} \;\; \underline{111} \;\; . \;\; \underline{010})_2$$

$$(47.2)_8$$

---

### **Base 16**

$$2^4 = 16 \implies \text{Group Base 2 by 4 (Pad with 0s)}$$

$$(\underline{0010} \;\; \underline{0111} \;\; . \;\; \underline{0100})_2$$

$$(27.4)_{16}$$
---
The question in the image asks you to prove the fast conversion method between a base $a$ and a base $b$ where $b = a^n$. Specifically, you need to prove that a number $num = (d_{m-1}d_{m-2}...d_1d_0)_a$ can be converted to base $b$ by taking groups of $n$ consecutive digits in base $a$ and converting each group into a single digit in base $b$.

This is the underlying mathematical proof for the shortcut shown in your lectures, such as grouping 4 binary digits to get a single hexadecimal digit (since $16 = 2^4$) or grouping 2 base-3 digits to get a base-9 digit (since $9 = 3^2$).

Here is the step-by-step mathematical proof you can use to solve it:

**1. Express the number using positional weights** According to the definition of number bases, the value of a number can be written as the sum of its digits multiplied by the base raised to the power of their position: $num = d_0 \cdot a^0 + d_1 \cdot a^1 + d_2 \cdot a^2 + \dots + d_{m-1} \cdot a^{m-1}$

**2. Group the terms into blocks of $n$** Assuming $m$ is a multiple of $n$ (if it isn't, we pad the most significant side of the number with leading zeros, which doesn't change its value), we can group the sum into blocks of $n$ digits: $num = (d_0 \cdot a^0 + d_1 \cdot a^1 + \dots + d_{n-1} \cdot a^{n-1}) + (d_n \cdot a^n + d_{n+1} \cdot a^{n+1} + \dots + d_{2n-1} \cdot a^{2n-1}) + \dots$

**3. Factor out the base powers from each group** By factoring out the lowest power of $a$ in each grouped block, we can rewrite the expression as: $num = (d_0 \cdot a^0 + \dots + d_{n-1} \cdot a^{n-1}) \cdot a^0 + (d_n \cdot a^0 + \dots + d_{2n-1} \cdot a^{n-1}) \cdot a^n + \dots$

**4. Substitute $b = a^n$** Since we are given that $b = a^n$, we can substitute $b$ into the factored powers. Because $(a^n)^0 = b^0$, $(a^n)^1 = b^1$, $(a^n)^2 = b^2$, the equation becomes: $num = (d_0 \cdot a^0 + \dots + d_{n-1} \cdot a^{n-1}) \cdot \mathbf{b^0} + (d_n \cdot a^0 + \dots + d_{2n-1} \cdot a^{n-1}) \cdot \mathbf{b^1} + \dots$

**5. Define the new digits in base $b$** Let each grouped sum inside the parentheses be evaluated as a new term, $D_k$: $D_0 = d_0 \cdot a^0 + \dots + d_{n-1} \cdot a^{n-1}$ $D_1 = d_n \cdot a^0 + \dots + d_{2n-1} \cdot a^{n-1}$

The maximum possible value for any group $D_k$ occurs when all its individual digits $d$ are at their maximum value for base $a$, which is $a - 1$. The sum of this maximum sequence calculates exactly to $a^n - 1$. Because $b = a^n$, this maximum value is equal to $b - 1$. Therefore, each $D_k$ calculates to a valid single digit in base $b$.

**6. Form the final number** Substituting $D_k$ back into our equation yields: $num = D_0 \cdot b^0 + D_1 \cdot b^1 + D_2 \cdot b^2 + \dots$

This is the exact mathematical definition of a number represented in base $b$. This concludes the proof, demonstrating that you can safely convert $n$ consecutive digits of base $a$ to directly map them to the individual digits of base $b$.