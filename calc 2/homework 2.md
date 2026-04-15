![[Pasted image 20260415193515.png]]
$$
\sum ^{\infty}_{n=1} \frac{n^{2026}}{2026^{n}}
$$

  $$
  \lim_{n \to \infty} \left| \frac{a_{n+1}}{a_n} \right| = \lim_{n \to \infty} \frac{(n+1)^{2026}}{2026^{n+1}} \cdot \frac{2026^n}{n^{2026}} = \lim_{n \to \infty} \left( \frac{n+1}{n} \right)^{2026} \cdot \frac{1}{2026} = 1 \cdot \frac{1}{2026}
  $$
    
- **Result:** Since $L = \frac{1}{2026} < 1$, the series **converges**.
    

---

### **ב. $\sum_{n=1}^{\infty} \frac{8+(-1)^n}{7^n}$**

- **Test:** Comparison Test.
    
- **Logic:** The numerator oscillates between 7 and 9. We can say:
    
    $$0 < \frac{7}{7^n} \leq \frac{8+(-1)^n}{7^n} \leq \frac{9}{7^n}$$
    
- **Result:** The series $\sum \frac{9}{7^n}$ is a geometric series with $r = \frac{1}{7} < 1$, which converges. By the comparison test, this series **converges**.
    

---

### **ג. $\sum_{n=1}^{\infty} \frac{2n}{n^2+1}$**

- **Test:** Limit Comparison Test (LCT) with the harmonic series $\sum \frac{1}{n}$.
    
- **Calculation:**
    
    $$\lim_{n \to \infty} \frac{\frac{2n}{n^2+1}}{\frac{1}{n}} = \lim_{n \to \infty} \frac{2n^2}{n^2+1} = 2$$
    
- **Result:** Since the limit is a positive constant and $\sum \frac{1}{n}$ diverges, this series **diverges**.
    

---

### **ד. $\sum_{n=1}^{\infty} \frac{\arctan n}{n^2+1}$**

- **Test:** Direct Comparison Test.
    
- **Logic:** We know that $\arctan n < \frac{\pi}{2}$ for all $n$.
    
    $$\frac{\arctan n}{n^2+1} < \frac{\pi/2}{n^2}$$
    
- **Result:** The series $\sum \frac{1}{n^2}$ is a $p$-series with $p=2 > 1$, which converges. Therefore, this series **converges**.
    

---

### **ה. $\sum_{n=2}^{\infty} \frac{\arctan(2n \ln^2 n)}{n \ln^2 n}$**

- **Test:** Comparison Test.
    
- **Logic:** Similar to the previous one, $\arctan(\text{anything}) < \frac{\pi}{2}$.
    
    $$0 < \frac{\arctan(2n \ln^2 n)}{n \ln^2 n} < \frac{\pi/2}{n \ln^2 n}$$
    
- **Integration Test / Known Series:** The series $\sum \frac{1}{n \ln^p n}$ converges if $p > 1$. Here $p=2$.
    
- **Result:** The series **converges**.
    

---

### **ו. $\sum_{n=1}^{\infty} \frac{2^n n!}{n^n}$**

- **Test:** Ratio Test.
    
- **Calculation:**
    
    $$\lim_{n \to \infty} \frac{a_{n+1}}{a_n} = \frac{2^{n+1} (n+1)!}{(n+1)^{n+1}} \cdot \frac{n^n}{2^n n!} = \frac{2(n+1) \cdot n^n}{(n+1)^{n+1}} = \frac{2 \cdot n^n}{(n+1)^n} = \frac{2}{(1 + \frac{1}{n})^n}$$
    
- **Limit:** As $n \to \infty$, the denominator approaches $e$. So the limit is $\frac{2}{e}$.
    
- **Result:** Since $e \approx 2.718$, then $L = \frac{2}{e} < 1$. The series **converges**.