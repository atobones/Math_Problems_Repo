# Task 9 — Digit Restrictions

## Key Concept

The **leading digit** of a number cannot be 0 — otherwise "0123" would be a 3-digit number. This restricts the first position to digits 1–9 (9 choices).

---

## Solutions

### Problem 1 — How many 5-digit numbers exist?

- First digit: 9 choices (1–9)
- Each remaining digit: 10 choices (0–9)

$$9 \times 10^4 = 90{,}000$$

---

### Problem 2 — How many 5-digit numbers are even?

Split into two cases:

**Case 1 — last digit = 0:**
$9 \times 10^3 = 9{,}000$

**Case 2 — last digit ∈ {2, 4, 6, 8}:**
$9 \times 10^3 \times 4 = 36{,}000$

$$9{,}000 + 36{,}000 = 45{,}000$$

---

### Problem 3 — No repeated digits

- Digit 1: 9 choices (1–9)
- Digit 2: 9 choices (0–9 minus digit 1)
- Digit 3: 8, Digit 4: 7, Digit 5: 6

$$9 \times 9 \times 8 \times 7 \times 6 = 27{,}216$$

---

### Problem 4 — At least one repeated digit

**Complementary counting:**

$$90{,}000 - 27{,}216 = 62{,}784$$
