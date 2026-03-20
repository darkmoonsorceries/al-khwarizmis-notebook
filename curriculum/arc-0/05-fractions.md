# Island 0.5: Fractions — The Inheritance Fulfilled

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> يُوصِيكُمُ اللَّهُ فِي أَوْلَادِكُمْ ۖ لِلذَّكَرِ مِثْلُ حَظِّ الْأُنثَيَيْنِ ۚ فَإِن كُنَّ نِسَاءً فَوْقَ اثْنَتَيْنِ فَلَهُنَّ ثُلُثَا مَا تَرَكَ
> "Allah instructs you concerning your children: for the male, what
> is equal to the share of two females. But if there are only
> daughters, two or more, for them is two-thirds of what he left."
> *— Surah An-Nisa (4:11)*

> وَلَهُنَّ الثُّمُنُ مِمَّا تَرَكْتُمْ
> "...then for them [the wives] is an eighth of what you leave."
> *— Surah An-Nisa (4:12)*

**Connection grade: Sahih** — The verse prescribes exact fractions:
1/2, 2/3, 1/4, 1/6, 1/8. These ARE the mathematics. Remove
fraction arithmetic and the verse cannot be obeyed. Zero links
between verse and math. The math IS the verse.

**The problem this ayah creates:** A man has died. His family
sits before me. The Quran gives each heir an exact fractional
share. But what IS a fraction? How do I add one-sixth to
one-eighth? And when the shares demand more than the estate
contains — what then?

---

## ٢. Al-Khwarizmi Discovers

The wife enters first. She walks the way a woman walks who held
the household together before the funeral and will hold it after.
Two daughters behind her, close enough that their sleeves touch.
The father comes last. He is burying his son. Every step costs
him something. The mother is already seated when I look up. She
was here before them. She is waiting.

The same family. The same impossible sum from the prologue. Four
islands of work stand between that day and this one.

The qadi has sent them. The estate is 2700 dinars. The Quran
prescribes their shares.

| Heir | Share | Source |
|------|-------|--------|
| Wife | 1/8 | 4:12 — husband had children |
| Two daughters | 2/3 | 4:11 — two or more daughters |
| Father | 1/6 | 4:11 — deceased had children |
| Mother | 1/6 | 4:11 — deceased had children |

I stare at what I have written.

One-eighth. Two-thirds. One-sixth.

These are not integers. Not a single one. I have the natural
numbers — 1, 2, 3, upward without end. I have zero. I have
negatives. I have addition and multiplication and their laws.
Every tool I own operates on whole numbers.

Not one of them can say "one-eighth."

---

I try anyway. The wife's share: 1/8 of 2700. Divide 2700 into
8 equal parts, take one. But I have no operation for this.
Multiplication gives 8 × 337 = 2696. Close. 8 × 338 = 2704.
Too far. The answer is between 337 and 338. Between two
integers. In a place where no integer lives.

I try the daughters' share. 2/3 of 2700. Split 2700 into 3
parts: 2700 = 3 × 900. Two-thirds is 1800. That works — but
only because 3 divides 2700 evenly. If the estate were 2500?
2500 divided by 3 is not a whole number. My method breaks again.

> *Margin note: The integers handle "how many" and "how far
> below zero." They cannot handle "what part of." The Quran
> demands parts. My tools do not have parts.*

The family is sitting in front of me. The wife has placed her
hands flat on the table, palms down. The daughters are still.
The father has lowered himself onto the bench by the wall. The
mother watches.

I cannot tell them to wait while I invent mathematics. But I
cannot give them an answer with tools that do not reach their
problem.

---

I go back to where everything starts. 1 = 1.

Multiplication says: 8 × something = 1. What is that something?

I know 8 × 0 = 0. Too small. 8 × 1 = 8. Too large. The answer
is between 0 and 1. I name it.

```
1/8 means: the number which, multiplied by 8, gives 1.

8 × (1/8) = 1
```

This is the multiplicative inverse of 8. Just as −5 was the
additive inverse of 5 — the number that, added to 5, gives 0 —
1/8 is the number that, multiplied by 8, gives 1.

> *Margin note: "And of everything We have created pairs"
> (51:49). Addition and subtraction. Multiplication and
> division. Each operation exists with its inverse.*

More generally:

```
a/b = a × (1/b)     [b ≠ 0]
```

The definition requires b ≠ 0. If b = 0, I need 0 × ? = 1.
But 0 × anything = 0, proved in Island 0.4. Division by zero
is not forbidden by convention. It is impossible by logic.

<!-- diagram: estate-rectangle -->

> *The estate: 2700 dinars. A rectangle. The full inheritance
> before any share is taken.*

With fractions defined, I extend the number system once more:

```
N ⊂ Z ⊂ Q

Natural numbers: {1, 2, 3, ...}
Integers:        {..., −2, −1, 0, 1, 2, ...}
Rationals:       {a/b : a, b ∈ Z, b ≠ 0}
```

Every integer is rational: 5 = 5/1. The rationals do not replace
the integers — they extend them. Subtraction forced Z into
existence. Division forces Q.

---

Now I can name the wife's share. One-eighth. The daughters'.
Two-thirds. The father's and mother's. One-sixth each.

But naming is not distributing. The four shares have different
denominators: 8, 3, 6, 6. Eighths and sixths are different-sized
pieces. I cannot add them any more than the shepherd could mix
sheep and camels in a single count.

I need pieces of the same size. A common denominator.

The multiples of 8: 8, 16, 24, 32...
The multiples of 3: 3, 6, 9, 12, 15, 18, 21, 24...
The multiples of 6: 6, 12, 18, 24...

<!-- diagram: common-denominator -->

> *Twenty-four divides evenly by 8, by 3, and by 6. Every share
> becomes a number of twenty-fourths.*

LCM(8, 3, 6) = 24. I convert every share:

```
Wife:       1/8 = 3/24     (× 3)
Daughters:  2/3 = 16/24    (× 8)
Father:     1/6 = 4/24     (× 4)
Mother:     1/6 = 4/24     (× 4)
```

<!-- diagram: heir-strips -->

> *Four heirs fill their strips. Three, sixteen, four, four.
> The rectangle divides.*

I add the numerators.

```
3 + 16 + 4 + 4 = 27
```

I stop.

27/24.

That is greater than 1.

<!-- diagram: overflow -->

> *Twenty-seven twenty-fourths. The strips extend past the
> boundary of the rectangle. The estate is not enough.*

Twenty-seven parts out of twenty-four. The Quran prescribes four
shares, each just in isolation, and together they demand more
than the estate. There is not enough.

I check the arithmetic. 3 + 16 = 19. 19 + 4 = 23. 23 + 4 = 27.
Correct. I check the conversions. 1/8 = 3/24 because
1 × 24 = 24 = 8 × 3. Correct. I check the verse references.
Every share is correct.

The overflow is not my error. It is the situation.

The wife is watching me. She has seen the number I wrote. She
does not read mathematics, but she reads faces, and she has
read mine.

"Is there a problem?"

"The shares add to more than the estate." I do not soften it.
"Each share is correct. Together they exceed what he left."

She does not look away. "Then what do we do?"

---

The Caliph Umar ibn al-Khattab, may Allah be pleased with him,
was the first to face this. He gathered the Companions. They
reasoned: when a man dies owing debts greater than his estate,
each creditor receives a fair proportion, not the full amount.
The debts are real. The estate is finite. Justice is
proportional.

The same principle here. The Quranic shares are real. The estate
is finite. Each heir's share is reduced by the same proportion.

> *Margin note: Ibn Abbas, may Allah be pleased with him, held
> a different view — certain heirs should bear the reduction
> while others receive their full share. The Shi'a school
> follows this position. What I describe, 'awl, is the majority
> Sunni method. The mathematics of both is sound. The legal
> question belongs to the jurists: 42:10.*

The procedure. The original denominator is 24. The numerators
sum to 27. I raise the denominator to match:

```
Original:  3/24 + 16/24 + 4/24 + 4/24 = 27/24
Adjusted:  3/27 + 16/27 + 4/27 + 4/27 = 27/27 = 1
```

<!-- diagram: awl -->

> *The strips compress. Each one shrinks by the same proportion.
> They fit inside the rectangle now. The estate is whole.*

The total is exactly 1. The ratios are preserved — daughters
have 16 parts to the wife's 3, before and after. The
relationships the Quran established survive the scaling. Only
the absolute amounts change.

Now I compute dinars.

```
Wife:       2700 × 3/27  = 300 dinars
Daughters:  2700 × 16/27 = 1600 dinars  (800 each)
Father:     2700 × 4/27  = 400 dinars
Mother:     2700 × 4/27  = 400 dinars
```

300 + 1600 + 400 + 400 = 2700. Every dinar accounted for.

I write the amounts and turn the paper so the wife can see. She
reads the numbers. She nods once — the way someone nods when a
weight shifts from their chest to the ground. She stands. She
gathers her daughters.

The father pushes himself from the bench. He does not look at
the paper. He looks at his son's wife, steady and upright, and
something in his face eases.

The mother folds the cloth she has been holding. She places it
on the table. She does not need to grip it anymore.

---

## ٣. The Derivation

Every result below derives from the multiplicative inverse
combined with laws established in Islands 0.1–0.4.

### Definition: multiplicative inverse

For any integer a ≠ 0, the multiplicative inverse is 1/a such
that:

```
a × (1/a) = 1
```

### Definition: fraction

```
a/b = a × (1/b)          [b ≠ 0]
```

### Division by zero

Suppose 1/0 exists. Then 0 × (1/0) = 1. But 0 × n = 0 for
all n (Island 0.4). So 0 = 1. Contradiction. ∎

### Equivalence of fractions

**Theorem.** a/b = c/d if and only if a × d = b × c.

*Proof.* Multiply both sides by b × d. Left: a × d. Right: b × c. ∎

### Addition

<!-- diagram: formal-fraction-arithmetic -->

> *Geometry spec: two bars of different widths (b and d) placed
> side by side. Both rescaled to common width b × d. Numerators
> adjust proportionally. Bars now stack.*

**Theorem.**

```
a/b + c/d = (a × d + b × c) / (b × d)
```

*Proof.* Multiply both sides by b × d. Distribute. ∎

Use LCM(b, d) when b × d is unnecessarily large.

### Multiplication and division

```
(a/b) × (c/d) = (a × c) / (b × d)

(a/b) ÷ (c/d) = (a × d) / (b × c)   [c ≠ 0]
```

Multiply: numerators × numerators, denominators × denominators.
Divide: multiply by the reciprocal.

### The 'awl procedure — formalized

<!-- diagram: formal-awl -->

> *Geometry spec: a fixed-width rectangle. Strips of prescribed
> widths placed inside, exceeding the boundary. The boundary
> expands to T (the sum), then all strips are expressed as
> fractions of T. Total = 1.*

Given prescribed shares s₁, s₂, ..., sₙ:

1. Find common denominator D.
2. Express each as kᵢ / D.
3. Sum: T = k₁ + k₂ + ... + kₙ.
4. If T = D: distribute directly.
5. If T < D: remainder exists (ta'sib rules).
6. If T > D: apply 'awl. Replace D with T. Each heir gets (kᵢ / T) × E.

**Theorem ('Awl preserves ratios).** The ratio kᵢ / kⱼ is
unchanged by 'awl.

*Proof.* Before: (kᵢ/D) ÷ (kⱼ/D) = kᵢ/kⱼ.
After: (kᵢ/T) ÷ (kⱼ/T) = kᵢ/kⱼ. Same. ∎

**The chain from 1 = 1:**

```
1 = 1
  → equality, preservation              [0.1]
  → multiplication, distributive law    [0.2–0.3]
  → multiplicative identity: a × 1 = a [0.3]
  → multiplicative inverse: a × (1/a) = 1
  → fractions: a/b = a × (1/b)
  → equivalence: a/b = c/d iff a×d = b×c
  → addition: common denominator
  → 'awl: proportional scaling preserves ratios
```

No new axioms. Every operation traces to 1 = 1.

---

## ٤. Al-Khwarizmi Solves

### Example 1: The family's inheritance — full computation

<!-- diagram: example-inheritance-solved -->

> *The family receives their shares. Every dinar accounted for.*

**Step 1.** Common denominator.

LCM(8, 3, 6): LCM(8, 3) = 24. LCM(24, 6) = 24.

```
Wife:       1/8 = 3/24
Daughters:  2/3 = 16/24
Father:     1/6 = 4/24
Mother:     1/6 = 4/24
```

**Step 2.** Sum: 3 + 16 + 4 + 4 = 27 > 24. Apply 'awl.

```
Wife:       3/27
Daughters:  16/27
Father:     4/27
Mother:     4/27
Sum:        27/27 = 1  ✓
```

**Step 3.** Dinars.

```
Wife:       2700 × 3/27  = 300
Daughters:  2700 × 16/27 = 1600  (800 each)
Father:     2700 × 4/27  = 400
Mother:     2700 × 4/27  = 400
Total:      2700  ✓
```

**Ratio check:** 1600/300 = 16/3. Before 'awl: (16/24)÷(3/24) = 16/3. Preserved. ✓

### Example 2: Fraction arithmetic

<!-- diagram: example-fraction-addition -->

> *Three fractions with different denominators. Convert to
> twelfths. Add numerators.*

Simplify:

```
  2     5     1
 --- + --- - ---
  3     6     4
```

LCM(3, 6, 4): LCM(3, 6) = 6. LCM(6, 4) = 12.

```
2/3 = 8/12     5/6 = 10/12     1/4 = 3/12

8/12 + 10/12 - 3/12 = 15/12
```

GCD(15, 12) = 3. Simplify: 15/12 = 5/4. ✓

---

## ٥. Your Turn

### Da'if (Guided)

**D1.** Estate: 3600 dinars. Heirs: husband (1/4) and one
daughter (1/2).

(a) Find the common denominator. *Hint: LCM(4, 2).*
(b) Add the shares. Is 'awl needed?
(c) Compute each heir's dinars. Where does the remainder go?

<!-- diagram: ex-daif-fractions -->

**D2.** The wife (300 dinars) gives each daughter 1/5 of her
share. Compute 1/5 of 300, then each daughter's new total.

**D3.** Simplify 3/4 + 1/6. *Hint: LCM(4, 6) = 12.*

### Hasan (Exam-level)

**H1.** Estate: 4800 dinars. Heirs: wife (1/8), one daughter
(1/2), mother (1/6). [9 marks]

(a) Sum the prescribed shares over the LCM. [3 marks]
(b) Is 'awl needed? Justify. [1 mark]
(c) Find the remainder as a fraction. [2 marks]
(d) No ta'sib claimant — redistribute proportionally. Compute
dinars. [3 marks]

<!-- diagram: ex-hasan-awl -->

**H2.** Simplify fully: 5/8 − 7/12 + 2/3. [3 marks]

**H3.** The father (400 dinars) later dies. His only heir: his
wife (the mother, already holding 400). Wife's share with no
children: 1/4. [5 marks]

(a) Mother's inheritance from the father. [2 marks]
(b) Her total wealth. [1 mark]
(c) Express as a fraction of the original 2700. [2 marks]

### Sahih (Proof and extension)

**S1.** Estate: E dinars. Heirs: wife, three daughters, both
parents. [12 marks]

(a) Prescribed shares from 4:11–12, common denominator, show
'awl is required. [4 marks]
(b) Apply 'awl. Each adjusted share as a fraction of E. [4 marks]
(c) Wife receives 225 dinars. Find E. [2 marks]
(d) Verify total = E. [2 marks]

**S2.** Prove: between any two distinct rationals lies another
rational. [4 marks]

*Hint: consider (a/b + c/d) / 2. This returns in Island 0.8.*

---

## ٦. Exam Technique

> **EXAM NOTE: Fraction arithmetic**
>
> **Show the common denominator.** Mark schemes award M marks
> for visible method. `1/3 + 1/6 = 2/6 + 1/6 = 3/6 = 1/2`.
> Jumping straight to 1/2 loses the method mark.
>
> **Always simplify.** 15/12 must become 5/4.
>
> **Common mistake:** subtracting denominators.
> `5/6 − 1/4 ≠ 4/2`. Only numerators change.
>
> **'Awl:** shares summing to >1 is NOT "impossible." Raise
> the denominator. Recompute. Verify total = estate.

---

## ٧. Log Pose

```
                  +--- 0.6 Variables & Equations
                  |    (the merchant's unknown wealth)
                  |
0.5 Fractions ----+
(inheritance)     |
                  |
                  +--- 0.7 Quadratic Equations
                       (al-jabr's garden problem)
```

**This island unlocks:**
- 0.6 (Variables) — the merchant knows what FRACTION to compute,
  but not what NUMBER to apply it to
- 0.7 (Quadratics) — al-jabr problems require fraction
  manipulation throughout

**Forward to FP1:** 27/24 > 1 — prescribed parts exceeding the
whole. In Arc 1, the quadratic formula demands √(−1). Same
pattern: overflow, then extension. Al-jabr — restoration.

---

## ٨. Reflection

The family came in the late afternoon. They left before maghrib.

The wife received 300 dinars. Each daughter 800. The father and
mother 400 each. The sum is 2700. Every dinar accounted for.
Every ratio the Quran prescribed — daughters to wife, parents
to daughters — preserved through the 'awl reduction. The
proportional relationships survived the scaling. That is what
justice looks like when the whole is not enough: not abandoning
any claim, but bearing the shortfall together.

The four islands before this were preparation. Equality, to know
what "the same" means. Counting, to enumerate. Multiplication,
to scale. Zero and negatives, to record what is absent and what
is owed. Every tool pointed here — to the moment a grieving
family needed exact fractions from a system that only knew whole
numbers.

The wife stood first. The father's face eased. The mother set
down the cloth.

> تِلْكَ حُدُودُ اللَّهِ
> "These are the limits of Allah."
> *— Surah An-Nisa (4:13)*

The fractions of 4:11–12 are not suggestions. They are hudud —
limits set by Allah. The computation that executes them is not
separate from the obedience. It is the obedience.

I set down my pen. The room is quiet. Then the door opens.

A broad-shouldered man enters, smelling of sandalwood and sea
salt. His fingers are stained with ink — he keeps his own
ledgers. He sits across from me and speaks without greeting.

"I must pay zakat. One part in forty of my wealth. But my
warehouses are uncounted and my ships have not returned. I know
the rule. I do not know the number."

He knows what fraction to compute. He does not know what to
compute it from. Every tool I have built requires a known
number. His number is unknown. It might be ten thousand dinars.
It might be fifty thousand. His ships might return full or
empty or not at all.

I need a way to write: "one-fortieth of something I do not
yet know."

*1 = 1 has not been lost.*

---
