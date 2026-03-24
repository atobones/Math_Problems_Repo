# Task 8 — Sequences with Repetition

## Key Concept

A **sequence with repetition** — each position independently chooses from all $n$ values. Repetition is allowed.

$$n^k$$

---

## Solutions

### Problem 1 — 5-digit PIN codes (digits 0–9, repetition allowed)

Each of 5 positions: 10 independent choices.

$$10^5 = 100{,}000$$

---

### Problem 2 — PIN codes with at least one repeated digit

**Complementary counting:** total minus codes with all different digits.

$$10^5 - P(10,5) = 100{,}000 - 30{,}240 = 69{,}760$$

---

### Problem 3 — PIN codes with all digits different

Ordered selection of 5 distinct digits from 10:

$$P(10,5) = 10 \times 9 \times 8 \times 7 \times 6 = 30{,}240$$
