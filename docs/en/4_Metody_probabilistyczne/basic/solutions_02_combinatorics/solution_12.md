# Task 12 — Mixed Counting Problem

## Strategy

For each part: (1) identify independent sub-decisions, (2) choose the correct model, (3) multiply (product rule) or add (sum rule).

---

## Part 1 — Student ID Codes

Format: 2 letters from {A,B,C,D,E} + 3 digits from 0–9.

### (1) Letters and digits may repeat

$$5^2 \times 10^3 = 25 \times 1{,}000 = 25{,}000$$

### (2) Letters may not repeat, digits may repeat

$$P(5,2) \times 10^3 = 20 \times 1{,}000 = 20{,}000$$

### (3) Neither letters nor digits may repeat

$$P(5,2) \times P(10,3) = 20 \times 720 = 14{,}400$$

---

## Part 2 — Medal Assignment (12 runners)

### (1) How many ways to assign gold/silver/bronze?

$$P(12,3) = 12 \times 11 \times 10 = 1{,}320$$

### (2) Two specific runners must both receive medals

Assign 2 of the 3 medals to them (ordered): $P(3,2) = 6$ ways.
Remaining medal goes to one of 10 other runners.

$$6 \times 10 = 60$$

---

## Part 3 — Committee Selection (6 men, 4 women)

### (1) All committees of 4

$$\binom{10}{4} = 210$$

### (2) Exactly 2 women

$$\binom{4}{2} \times \binom{6}{2} = 6 \times 15 = 90$$

### (3) At least 1 woman

$$\binom{10}{4} - \binom{6}{4} = 210 - 15 = 195$$

---

## Part 4 — Circular Seating (7 people)

### (1) All seating arrangements

$$(7-1)! = 720$$

### (2) Two particular people sit next to each other

$$(6-1)! \times 2! = 120 \times 2 = 240$$

---

## Part 5 — Passwords (5 chars from 36 symbols: digits + A–Z)

### (1) Repetition allowed

$$36^5 = 60{,}466{,}176$$

### (2) No character may repeat

$$P(36,5) = 36 \times 35 \times 34 \times 33 \times 32 = 45{,}239{,}040$$

### (3) Counting models used

- With repetition → **Sequence with repetition** (independent choices per position)
- Without repetition → **k-Permutation** (ordered selection, no reuse)
