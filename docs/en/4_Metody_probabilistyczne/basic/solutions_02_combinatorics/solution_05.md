# Task 5 — Combinations

## Key Concept

A **combination** is an unordered selection — the set {A,B,C} is the same outcome as {C,B,A}.

$$\binom{n}{k} = \frac{n!}{k!(n-k)!}$$

For restricted problems: complementary counting or multiplying independent sub-selections.

---

## Solutions

### Problem 1 — Committee of 4 from 12 students

Order doesn't matter → Combination.

$$\binom{12}{4} = \frac{12!}{4! \cdot 8!} = 495$$

---

### Problem 2 — Committee must contain one particular student (Alice)

Fix Alice on the committee. Choose the remaining 3 from the other 11 students.

$$\binom{11}{3} = 165$$

---

### Problem 3 — Committee contains at least one of two particular students

**Complementary counting:** total committees minus committees with **neither** of the two.

$$\binom{12}{4} - \binom{10}{4} = 495 - 210 = 285$$

---

### Problem 4 — Exactly 2 women (from 7 men and 5 women)

Two independent sub-selections, multiplied together:

- Choose 2 women from 5: $\binom{5}{2} = 10$
- Choose 2 men from 7: $\binom{7}{2} = 21$

$$10 \times 21 = 210$$
