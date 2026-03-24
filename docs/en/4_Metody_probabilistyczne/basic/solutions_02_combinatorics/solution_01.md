# Solution

# Task 1 — Recognizing Counting Models

## Key Questions Before Choosing a Model

Before applying any formula, I answer these four questions:

1. Are we using **all** objects or only **some**?
2. Does **order** matter?
3. Is **repetition** allowed?
4. Are some objects **identical**?

---

## Solutions

### Problem 1 — Arranging 7 students in a line

- All 7 students are used → YES
- Order matters (position 1 ≠ position 2) → YES
- No repetition (one student = one seat) → NO

**Model: Permutation**

$$P_7 = 7! = 5040$$

---

### Problem 2 — Choosing 4 members of a committee from 12 people

- Only 4 of 12 are selected → using SOME
- Order does NOT matter ({A,B,C,D} = {D,C,B,A} as a committee)
- No repetition

**Model: Combination**

$$\binom{12}{4} = \frac{12!}{4! \cdot 8!} = 495$$

---

### Problem 3 — Assigning gold, silver, and bronze medals among 15 athletes

- Only 3 of 15 are selected → using SOME
- Order DOES matter (gold ≠ silver ≠ bronze)
- No repetition

**Model: k-Permutation (ordered selection without repetition)**

$$P(15,3) = \frac{15!}{12!} = 15 \times 14 \times 13 = 2730$$

---

### Problem 4 — Forming a 6-digit PIN code

- Using 6 positions from digits 0–9 → using SOME
- Order matters (1234 ≠ 4321)
- Repetition IS allowed (same digit can appear twice)

**Model: Sequence with repetition**

$$10^6 = 1{,}000{,}000$$

---

### Problem 5 — Arranging the letters of BANANA

- All 6 letters are used → using ALL
- Order matters
- Some letters are **identical**: B×1, A×3, N×2

**Model: Permutation with repeated elements**

$$\frac{6!}{1! \cdot 3! \cdot 2!} = \frac{720}{1 \cdot 6 \cdot 2} = 60$$

---

### Problem 6 — Seating 6 people around a round table

- All 6 people are used → using ALL
- Arranged in a **circle** — only relative positions matter
- Rotations produce the same arrangement

**Model: Circular Permutation**

$$(6-1)! = 5! = 120$$
