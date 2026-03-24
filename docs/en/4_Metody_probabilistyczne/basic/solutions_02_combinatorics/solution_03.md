# Task 2 — Permutations

## Key Concept

A **permutation** arranges ALL elements of a set where order matters and repetition is not allowed.

$$P_n = n!$$

For problems with restrictions, I use **complementary counting**: subtract the forbidden cases from the total.

---

## Solutions

### Problem 1 — 8 different books arranged on a shelf

All 8 books, order matters, no repetition → Permutation.

The first slot can hold any of 8 books, the second any of the remaining 7, and so on.

$$P_8 = 8! = 40{,}320$$

---

### Problem 2 — 8 people in a row, two particular people must sit TOGETHER

**Technique:** Treat the inseparable pair (A and B) as one block.

- We now have 7 units to arrange: $7!$ ways
- Inside the block, A and B can swap: $2!= 2$ ways
- Multiply by the product rule

$$7! \times 2! = 5040 \times 2 = 10{,}080$$

---

### Problem 3 — 8 people in a row, those two must NOT sit together

**Technique:** Complementary counting.

$$\text{Total} - \text{Together} = 8! - 7! \times 2!$$

$$= 40{,}320 - 10{,}080 = 30{,}240$$

---

### Problem 4 — 10 questions in a test, first question is fixed

Since question 1 is fixed in position 1, only the remaining 9 questions are arranged freely.

$$9! = 362{,}880$$
