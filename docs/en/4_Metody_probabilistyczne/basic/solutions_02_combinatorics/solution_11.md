# Task 11 — Modeling Outcomes

## Key Concept

The number of outcomes depends on **how the experiment is recorded** — not just the physical setup. The same draw of 3 balls can yield different sample spaces depending on:
- distinguishable vs indistinguishable objects
- whether order is recorded or ignored

---

## Part 1 — Distinguishable vs Indistinguishable

Box: 4 red, 4 blue, 3 green = 11 balls total.

### (1) Balls indistinguishable by color

$$\frac{11!}{4! \cdot 4! \cdot 3!} = \frac{39{,}916{,}800}{3456} = 11{,}550$$

### (2) All balls individually labeled ($R_1, R_2, \ldots$)

$$11! = 39{,}916{,}800$$

### (3) Why different?

When balls are labeled, swapping $R_1$ and $R_2$ produces a new arrangement. When balls are identical by color, that swap is invisible — it produces the same arrangement. The labeled count overcounts by exactly $4! \times 4! \times 3!$.

---

## Part 2 — Recording Order vs Ignoring Order

Three balls drawn without replacement from the same box (indistinguishable by color).

### (1) Only the set of colors recorded (order ignored)

Possible color multisets: {R,R,R}, {R,R,B}, {R,R,G}, {R,B,B}, {R,B,G}, {R,G,G}, {B,B,B}, {B,B,G}, {B,G,G}, {G,G,G}

**10 distinct outcomes**

### (2) Sequence of colors recorded

Each multiset produces multiple sequences. For example {R,B,G} gives 6 ordered sequences. The total number of distinct color sequences is **34**.

### (3) Why recording order changes the model

When order is recorded, (R,B,G) and (B,R,G) are different outcomes. Without order, both map to {R,B,G}. Recording order multiplies the outcome space by the arrangements of each selection.

---

## Part 3 — PIN Code vs 4-Digit Number

### (1) 4-digit PIN codes (0–9, repetition allowed)

$$10^4 = 10{,}000$$

### (2) 4-digit numbers (first digit ≠ 0)

$$9 \times 10^3 = 9{,}000$$

### (3) Why different rules?

A PIN code allows 0000 — every position is independent with 10 choices. A 4-digit number cannot start with 0, so the first position has only 9 choices.

### (4) Why 1234 ≠ 4321?

A PIN code is an **ordered sequence** — each position is distinct. The entry sequence (1,2,3,4) and (4,3,2,1) differ in every position, so they are counted as different outcomes.
