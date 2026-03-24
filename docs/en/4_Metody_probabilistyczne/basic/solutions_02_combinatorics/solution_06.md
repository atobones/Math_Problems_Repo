# Task 6 — Combinations in Card Problems

## Key Facts

- Standard deck: 52 cards total
- Hearts: 13 | Non-hearts: 39
- Face cards (J, Q, K): 12 total | Non-face cards: 40

---

## Solutions

### Problem 1 — Exactly 2 hearts in a 5-card hand

Two independent selections:

- 2 hearts from 13: $\binom{13}{2} = 78$
- 3 non-hearts from 39: $\binom{39}{3} = 9{,}139$

$$78 \times 9{,}139 = 712{,}842$$

---

### Problem 2 — At least one heart in a 5-card hand

**Complementary counting:** total hands minus hands with zero hearts.

$$\binom{52}{5} - \binom{39}{5} = 2{,}598{,}960 - 575{,}757 = 2{,}023{,}203$$

---

### Problem 3 — No face cards in a 5-card hand

Remove all 12 face cards. Choose 5 freely from the remaining 40.

$$\binom{40}{5} = 658{,}008$$
