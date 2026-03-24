# Task 10 — Urn Models

## Setup

Urn contains: **5 red**, **4 blue**, **3 green** = 12 balls total.

The same physical experiment (drawing 3 balls) produces different counts depending on whether order is recorded.

---

## Solutions

### Problem 1 — 3 balls drawn without replacement, order ignored

Model: Combination — we select a set, not a sequence.

$$\binom{12}{3} = 220$$

---

### Problem 2 — Exactly 2 red balls, order ignored

- Choose 2 red from 5: $\binom{5}{2} = 10$
- Choose 1 non-red from 7: $\binom{7}{1} = 7$

$$10 \times 7 = 70$$

---

### Problem 3 — 3 balls drawn, order of drawing recorded

Model: k-Permutation — drawing sequence matters.

$$P(12,3) = 12 \times 11 \times 10 = 1{,}320$$

---

### Problem 4 — Exactly 2 red balls, order recorded

- Choose which 2 of the 3 positions are red: $\binom{3}{2} = 3$
- Arrange 2 distinct red balls in those positions: $P(5,2) = 20$
- Choose 1 non-red for the remaining position: $7$

$$3 \times 20 \times 7 = 420$$
