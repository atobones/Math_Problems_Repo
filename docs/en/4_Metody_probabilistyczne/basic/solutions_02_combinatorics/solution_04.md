# Task 4 — Circular Permutations

## Key Concept

In a **circular arrangement**, rotating everyone one seat produces the same arrangement. To eliminate this redundancy, fix one person in place and arrange the rest:

$$(n-1)!$$

---

## Solutions

### Problem 1 — 7 people seated around a round table

Fix person A at one seat (removes rotational duplicates). Arrange the remaining 6 people in the other 6 seats.

$$(7-1)! = 6! = 720$$

---

### Problem 2 — Two particular people must sit TOGETHER

**Technique:** Merge A and B into one block → 6 units seated around the circle.

- Circular arrangements of 6 units: $(6-1)! = 5! = 120$
- A and B can swap inside the block: $\times 2$

$$5! \times 2 = 120 \times 2 = 240$$

---

### Problem 3 — Two particular people must sit OPPOSITE each other

Fix person A at a seat. Person B must sit exactly 3 seats away (the only "opposite" position in a 7-seat circle).

- B's seat: **1 way** (forced)
- Remaining 5 people fill the other 5 seats freely: $5!$

$$5! = 120$$
