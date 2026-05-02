# 1.
![[Pasted image 20260502130728.png]]
## a.
![[Pasted image 20260502130740.png]]
Convert $(101010.11)_2$ to bases 4, 8, 10, 16:

$$ \text{To Base 10:} $$

$$ (101010.11)_{2} = 1 \cdot 2^{5} + 0 \cdot 2^{4} + 1 \cdot 2^{3} + 0 \cdot 2^{2} + 1 \cdot 2^{1} + 0 \cdot 2^{0} + 1 \cdot 2^{-1} + 1 \cdot 2^{-2} $$

$$ = 32 + 0 + 8 + 0 + 2 + 0 + 0.5 + 0.25 $$

$$ = (42.75)_{10} $$

$$ \text{To Base 4:} $$

$$ \text{Group bits in pairs from the binary point (since } 4 = 2^2 \text{):} $$

$$ 10 \ | \ 10 \ | \ 10 \ . \ 11 $$

$$ 2 \ | \ 2 \ | \ 2 \ . \ 3 $$

$$ = (222.3)_{4} $$

$$ \text{To Base 8:} $$

$$ \text{Group bits in triplets from the binary point (since } 8 = 2^3 \text{):} $$

$$ \text{Add a trailing zero to the fractional part to complete the group:} $$

$$ 101 \ | \ 010 \ . \ 110 $$

$$ 5 \ | \ 2 \ . \ 6 $$

$$ = (52.6)_{8} $$

$$ \text{To Base 16:} $$

$$ \text{Group bits in groups of four from the binary point (since } 16 = 2^4 \text{):} $$

$$ \text{Add leading/trailing zeros to complete the groups:} $$

$$ 0010 \ | \ 1010 \ . \ 1100 $$

$$ 2 \ | \ A \ . \ C $$

$$ = (2A.C)_{16} $$

---

### Question 1 - Part b

Convert $(121.223)_9$ to base 3:

$$ \text{Since } 9 = 3^2 \text{, each base 9 digit corresponds to exactly two base 3 digits:} $$

$$ 1_{9} = (01)_{3} $$

$$ 2_{9} = (02)_{3} $$

$$ 3_{9} = (10)_{3} $$

$$ \text{Substitute each digit step-by-step:} $$

$$ 1 \ | \ 2 \ | \ 1 \ . \ 2 \ | \ 2 \ | \ 3 $$

$$ 01 \ | \ 02 \ | \ 01 \ . \ 02 \ | \ 02 \ | \ 10 $$

$$ = (10201.02021)_{3} $$

---

### Question 1 - Part c

Convert $(87.5)_9$ to base 3:

$$ \text{Using the same logic (} 9 = 3^2 \text{), convert each digit to a two-digit base 3 number:} $$

$$ 8_{9} = 2 \cdot 3^1 + 2 \cdot 3^0 = (22)_{3} $$

$$ 7_{9} = 2 \cdot 3^1 + 1 \cdot 3^0 = (21)_{3} $$

$$ 5_{9} = 1 \cdot 3^1 + 2 \cdot 3^0 = (12)_{3} $$

$$ \text{Substitute each digit step-by-step:} $$

$$ 8 \ | \ 7 \ . \ 5 $$

$$ 22 \ | \ 21 \ . \ 12 $$

$$ = (2221.12)_{3} $$

Would you like me to continue with the rest of Question 1 in English?
