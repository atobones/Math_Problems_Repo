# Task 7 — k-Permutations (Ordered Selections Without Repetition)

## Key Concept

A **k-permutation** is an ordered selection of $k$ elements from $n$, without repetition. Order matters: gold ≠ silver ≠ bronze.

$$P(n,k) = \frac{n!}{(n-k)!} = n \times (n-1) \times \ldots \times (n-k+1)$$

---

## Solutions

### Problem 1 — First 3 places among 12 runners

Ordered selection of 3 from 12:

$$P(12,3) = 12 \times 11 \times 10 = 1{,}320$$

---

### Problem 2 — 4-digit numbers with distinct digits from 1–9

Each arrangement of 4 distinct digits IS a number. Order matters, no repetition:

$$P(9,4) = 9 \times 8 \times 7 \times 6 = 3{,}024$$

---

### Problem 3 — Numbers from above divisible by 5

The last digit must be 5 (only multiple of 5 in {1–9}). Fix last digit = 5, then arrange 3 distinct digits from the remaining 8 in the first three positions:

$$P(8,3) = 8 \times 7 \times 6 = 336$$
