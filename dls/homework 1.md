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



### **Base 4**

$$2^2 = 4 \implies \text{Group Base 2 by 2}$$

$$(\underline{10} \;\; \underline{01} \;\; \underline{11} \;\; . \;\; \underline{01})_2$$

$$(213.1)_4$$



### **Base 8**

$$2^3 = 8 \implies \text{Group Base 2 by 3 (Pad with 0s)}$$

$$(\underline{100} \;\; \underline{111} \;\; . \;\; \underline{010})_2$$

$$(47.2)_8$$



### **Base 16**

$$2^4 = 16 \implies \text{Group Base 2 by 4 (Pad with 0s)}$$

$$(\underline{0010} \;\; \underline{0111} \;\; . \;\; \underline{0100})_2$$

$$(27.4)_{16}$$

---
## h.
![[Pasted image 20260502144315.png]]

$$num = (d_0 a^0 + d_1 a^1 + d_2 a^2 + ... + d_{m-1} a^{m-1})$$

$$= d_0 a^0 + d_1 a^1 + ... + d_{n-1} a^{n-1} + a^n (d_{n} a^0 + d_{n+1} a^1 + ... + d_{2n-1} a^{n-1}) +$$
$$a^{2n} (d_{2n} a^0 + d_{2n+1} a^1 + ... + d_{3n-1} a^{n-1})$$
 Every set of parentheses represents a number according to weighted calculation,
 a digit that is within the range $[0, b-1]$ and therefore can be
 represented as a digit in base $b$, meaning:

**Final Equation:**
$$= b^0 \cdot B_0 + b^1 \cdot B_1 + b^2 \cdot B_2 + ... = (... B_3 B_2 B_1 B_0)_b$$

---
# 2.
![[Pasted image 20260502144331.png]]
**1. Number: $11$**

$$11_{10} = 1011_2$$

Minimum bits with sign bit: **$01011$** (5 bits)

**2. Number: $-11$**

Base positive: **$01011$**

- **Sign-Magnitude:** Change MSB to 1 $\implies$ **$11011$**

- **1's Complement:** Invert all bits ($0 \leftrightarrow 1$) $\implies$ **$10100$**

- **2's Complement:** 1's Complement + 1 $\implies 10100 + 1 =$ **$10101$**


**3. Number: $-14$**

$$14_{10} = 1110_2 \implies \text{Base positive: } \mathbf{01110} \text{ (5 bits)}$$

- **Sign-Magnitude:** Change MSB to 1 $\implies$ **$11110$**

- **1's Complement:** Invert all bits $\implies$ **$10001$**

- **2's Complement:** 1's Complement + 1 $\implies 10001 + 1 =$ **$10010$**


**4. Number: $126$**

$$126_{10} = 1111110_2 \implies \text{Base positive: } \mathbf{01111110} \text{ (8 bits)}$$

| **Decimal** | **Positive Binary** | **Sign-Magnitude** | **1's Complement** | **2's Complement** |
| ----------- | ------------------- | ------------------ | ------------------ | ------------------ |
| **11**      | $01011$             | $01011$            | $01011$            | $01011$            |
| **-11**     | $01011$             | $11011$            | $10100$            | $10101$            |
| **-14**     | $01110$             | $11110$            | $10001$            | $10010$            |
| **126**     | $01111110$          | $01111110$         | $01111110$         | $01111110$         |

---
# 3.
![[Pasted image 20260502182718.png]]

Let a negative number $-x$ be defined by Definition 2 (MSB = 1):

$$-x = -2^{n-1} + a_{n-2} 2^{n-2} + \dots + a_1 2^1 + a_0 2^0$$

Multiply by $-1$ to find the positive value $x$:

$$x = 2^{n-1} - a_{n-2} 2^{n-2} - \dots - a_1 2^1 - a_0 2^0$$

Apply the mathematical identity: $2^{n-1} = 2^{n-2} + \dots + 2^1 + 2^0 + 1$:

$$x = (2^{n-2} + \dots + 2^0 + 1) - a_{n-2} 2^{n-2} - \dots - a_0 2^0$$

Group the coefficients for each power of 2:

$$x = (1 - a_{n-2})2^{n-2} + \dots + (1 - a_1)2^1 + (1 - a_0)2^0 + 1$$

Substitute bit inversion logic $a'_i = (1 - a_i)$:

$$x = a'_{n-2}2^{n-2} + \dots + a'_1 2^1 + a'_0 2^0 + 1$$

This matches Definition 1: $x = (\text{1's Complement of bits}) + 1$.

$$\blacksquare$$


---
# 4.
![[Pasted image 20260502182900.png]]
**Overflow Rules:**

- $\text{Pos} + \text{Pos} = \text{Neg} \implies \textbf{OVERFLOW}$

- $\text{Neg} + \text{Neg} = \text{Pos} \implies \textbf{OVERFLOW}$

- $\text{Pos} + \text{Neg} \implies \textbf{NO OVERFLOW}$


---

**1. $1010 + 1001$**

$$1010 + 1001 = \mathbf{1}0011 \xrightarrow{\text{Drop Carry}} 0011$$

$$\text{Neg} + \text{Neg} = \text{Pos} \implies \textbf{OVERFLOW}$$

**2. $1001 - 0110$**

$$1001 + \text{2's Comp}(0110) \implies 1001 + 1010$$

$$1001 + 1010 = \mathbf{1}0011 \xrightarrow{\text{Drop Carry}} 0011$$

$$\text{Neg} + \text{Neg} = \text{Pos} \implies \textbf{OVERFLOW}$$

**3. $0111 + 0001$**

$$0111 + 0001 = 1000$$

$$\text{Pos} + \text{Pos} = \text{Neg} \implies \textbf{OVERFLOW}$$

**4. $0101 - 0110$**

$$0101 + \text{2's Comp}(0110) \implies 0101 + 1010$$

$$0101 + 1010 = 1111$$

$$\text{Pos} + \text{Neg} \implies \textbf{NO OVERFLOW}$$

**5. $110111 + 010110$**

$$110111 + 010110 = \mathbf{1}001101 \xrightarrow{\text{Drop Carry}} 001101$$

$$\text{Neg} + \text{Pos} \implies \textbf{NO OVERFLOW}$$

**6. $11101 + 11010$**

$$11101 + 11010 = \mathbf{1}10111 \xrightarrow{\text{Drop Carry}} 10111$$

$$\text{Neg} + \text{Neg} = \text{Neg} \implies \textbf{NO OVERFLOW}$$

**7. $01011 + 11101$**

$$01011 + 11101 = \mathbf{1}01000 \xrightarrow{\text{Drop Carry}} 01000$$

$$\text{Pos} + \text{Neg} \implies \textbf{NO OVERFLOW}$$

---
# 5.
![[Pasted image 20260502183354.png]]

**1. $10 + 15$** (Requires **6 bits** to prevent overflow since max sum is 25)

$$10_{10} \rightarrow 001010_2$$

$$15_{10} \rightarrow 001111_2$$

$$001010 + 001111 = \mathbf{011001_2} = 25_{10}$$

**2. $9 + (-19)$** (Requires **6 bits** to represent -19)

$$9_{10} \rightarrow 001001_2$$

$$-19_{10} \rightarrow 101101_2$$

$$001001 + 101101 = \mathbf{110110_2} = -10_{10}$$

**3. $24 + (-9)$** (Requires **6 bits** to represent 24)

$$24_{10} \rightarrow 011000_2$$

$$-9_{10} \rightarrow 110111_2$$

$$011000 + 110111 = \mathbf{1}001111 \xrightarrow{\text{Drop Carry}} \mathbf{001111_2} = 15_{10}$$

**4. $(-3) + (-14)$** (Requires **6 bits**)

$$-3_{10} \rightarrow 111101_2$$

$$-14_{10} \rightarrow 110010_2$$

$$111101 + 110010 = \mathbf{1}101111 \xrightarrow{\text{Drop Carry}} \mathbf{101111_2} = -17_{10}$$

**5. $47 + (-47)$** (Requires **7 bits** to represent 47)

$$47_{10} \rightarrow 0101111_2$$

$$-47_{10} \rightarrow 1010001_2$$

$$0101111 + 1010001 = \mathbf{1}0000000 \xrightarrow{\text{Drop Carry}} \mathbf{0000000_2} = 0_{10}$$

---
# 6.
## a.
![[Pasted image 20260502183848.png]]
Let operands be $X > 0$ and $Y < 0$.

$$\text{Binary representation: } 0.xxxxx + 1.xxxxx$$

Check the Most Significant Bit (MSB) addition: $0 + 1 + C_{in}$ (Carry from previous bit).

- **Case 1: $C_{in} = 0$**

$$\text{MSB}_{sum} = 0 + 1 + 0 = \mathbf{1}$$

$$C_{out} = \mathbf{0}$$

Result is Negative. No overflow.

- **Case 2: $C_{in} = 1$**

$$\text{MSB}_{sum} = 0 + 1 + 1 = \mathbf{0}$$

$$C_{out} = \mathbf{1} \xrightarrow{\text{Drop}}$$

Result is Positive. Drop $C_{out}$.


**Conclusion:** Opposite signs never cause an overflow error; $C_{out}$ is safely discarded.

---
## b.
![[Pasted image 20260502183912.png]]

- **Positive + Positive ($0.xxxxx + 0.xxxxx$)**

$$\text{MSB}_{sum} = 0 + 0 + C_{in} = C_{in}$$

$$C_{out} = \mathbf{0} \text{ (Always)}$$

Ignore $C_{out}$. (If $C_{in}=1$, MSB becomes $1 \implies$ standard Overflow Error detected by MSB change, not $C_{out}$).

- **Negative + Negative ($1.xxxxx + 1.xxxxx$)**

$$\text{MSB}_{sum} = 1 + 1 + C_{in} = C_{in}$$

$$C_{out} = \mathbf{1} \text{ (Always)} \xrightarrow{\text{Drop}}$$

Ignore $C_{out}$ since the $1$ represents $-2^n$, and dropping it resolves to the correct bounds.


**Conclusion:** $C_{out}$ is safely ignored for all cases in 2's complement addition.

---
# 7.
![[Pasted image 20260502183931.png]]
