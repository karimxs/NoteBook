# 1.
## a.
![[Pasted image 20260524170547.png]]
$$
f(x,y,z,w)=y\overline{w}+\overline{xzw}+\overline{zx}y+wz\overline{y}
$$
---
# b.
$$
f(w, x, y, z) = \sum(1, 3, 10, 14) + \sum_{\emptyset}(0, 4, 8, 11, 12, 15)
$$
![[WhatsApp Image 2026-05-24 at 17.22.56.jpeg]]
$$
f(x,y,w,z)=\overline{wx}z+wy
$$
---
# c.
$$f(a, b, c) = a'bc + ab'c + abc' + abc$$
![[WhatsApp Image 2026-05-24 at 17.29.38.jpeg]]
$$
f(a,b,c)= ac+ab+bc
$$
---
# 2.
The main characteristic of an Exclusive OR (XOR) gate is that it outputs $0$ when its two inputs are identical ($0,0$ or $1,1$), and outputs $1$ when they are different.

We will use 4 XOR gates to compare each pair of bits individually:

- $X_0 = A_0 \oplus B_0$
    
- $X_1 = A_1 \oplus B_1$
    
- $X_2 = A_2 \oplus B_2$
    
- $X_3 = A_3 \oplus B_3$
![[WhatsApp Image 2026-05-24 at 17.40.42.jpeg]]
---
# 3.
A 3→8 decoder receives a 3-digit number. We will divide the number into $b_2, b_1, b_0$ where the position of the digit is according to the index.
![[WhatsApp Image 2026-05-24 at 17.58.53.jpeg]]

---
# 4.
Analyzing the Original Function
We will analyze the original function from the question:
$$f(x,w,y,z) = \overline{wx\overline{y}z} + \bar{x}y(z+\overline{w}) + xz(w+y)$$Analyzing the Fault

The fault states that the value of F (the output of gate 1) is stuck at value $1$.
Meaning, the gate is $z+\overline{w} = 1$
And therefore, the value of the AND gate is: $\bar{x}y \cdot 1 = \bar{x}y$
And therefore the faulty function will look like:$$f_{faulty}(x,w,y,z) = \overline{wx\overline{y}z} + \bar{x}y + xz(w+y)$$Checking for Equivalence
Let's see now that the two functions are not equivalent:
The only difference between the two functions is in the middle expression.$$f_{orig} \stackrel{?}{\equiv} f_{faulty}$$$$\bar{x}y \not\equiv \bar{x}y(z+\overline{w})$$The two expressions are not identical. Therefore, we will not always get equality.
Proof by Counterexample
If we substitute, for example, $w=1, z=0, x=0, y=1$ we will get:$$(\overline{0}) \cdot 1 \stackrel{?}{\equiv} (\overline{0}) \cdot 1(0+\overline{1})$$$$1 \stackrel{?}{\equiv} 1 \cdot 0$$$$1 \neq 0$$And we will get:$$f_{faulty}(x,w,y,z) = 1$$$$f_{orig}(x,w,y,z) = 0$$And therefore there is a detectable fault.

---
# 5.
## a.
![[Pasted image 20260531121132.png]]
![[Pasted image 20260531121530.png]]

$$f_{eq}(A,B) = \overline{A_0}\overline{A_1}\overline{B_0}\overline{B_1} + \overline{A_0}A_1\overline{B_0}B_1 + A_0A_1B_0B_1 + A_0\overline{A_1}B_0\overline{B_1}$$

$$\overline{A_0}(\overline{A_1}\overline{B_0}\overline{B_1} + A_1\overline{B_0}B_1) + A_0(A_1B_0B_1 + \overline{A_1}B_0\overline{B_1})$$

$$\overline{A_0}\overline{B_0}(\overline{A_1}\overline{B_1} + A_1B_1) + A_0B_0(A_1B_1 + \overline{A_1}\overline{B_1})$$

$$\overline{A_0}\overline{B_0}(A_1 \otimes B_1) + A_0B_0(A_1 \otimes B_1)$$

$$(A_1 \otimes B_1)(\overline{A_0}\overline{B_0} + A_0B_0)$$

$$f_{eq}(A,B) = (A_0 \otimes B_0) \cdot (A_1 \otimes B_1)$$
![[Pasted image 20260531122316.png]]

$$f_{gt}(A,B) = \overline{B_0}A_0 + A_1\overline{B_0}\overline{B_1} + A_0A_1\overline{B_1}$$
![[Pasted image 20260531124302.png]]

---
## b.

We will create a new block (comparator) which outputs one if the numbers are equal, and one if $A>B$.

**When is a 4-digit number equal:**

$$E_{eq_1} \cdot E_{eq_2} = \begin{cases} (B_2B_3 = A_2A_3) & \text{- when the MSB digits are equal} \\ (B_0B_1 = A_0A_1) & \text{- and when the LSB digits are equal} \end{cases}$$

**When is a 4-digit number greater than another:**

$$E_{gt_1} + (G_{gt_2} \cdot E_{eq_1}) \begin{cases} \text{- when the MSB digits of A are greater than B's} \\ \text{- or the MSB are equal, and then we check the LSB digits} \end{cases}$$

![[Pasted image 20260531124752.png]]

---
# 6.
Here are the step-by-step solutions and explanations for both digital logic questions from your image.

### **Question 6 Solution**

**The Goal:** Design a 4-input combinational circuit where the output is `1` if:

- All inputs are `1`
    
- No inputs are `1` (all are `0`)
    
- There is an odd number of `1`s
    

Let's define the four inputs as $A, B, C, D$ and the output as $F$. We can break the requirements down into three distinct Boolean expressions and OR them together:

1. **"All inputs are equal to 1":** This is only true when $A=1, B=1, C=1, D=1$.
    
- Expression: $A \cdot B \cdot C \cdot D$
    
2. **"No input is equal to 1":** This means all inputs are `0`.
    
- Expression: $\overline{A} \cdot \overline{B} \cdot \overline{C} \cdot \overline{D}$
    
3. **"An odd number of inputs is equal to 1":** In digital logic, an XOR gate acts as an odd-parity generator. If you XOR all inputs together, the result is `1` whenever an odd number of those inputs are `1` (i.e., one or three `1`s).
    
- Expression: $A \oplus B \oplus C \oplus D$
    




$$F = (A \cdot B \cdot C \cdot D) + (\overline{A} \cdot \overline{B} \cdot \overline{C} \cdot \overline{D}) + (A \oplus B \oplus C \oplus D)$$
