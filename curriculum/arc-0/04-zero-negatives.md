# Island 0.4: Zero and Negatives — The Debtor's Position

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> يَا أَيُّهَا الَّذِينَ آمَنُوا إِذَا تَدَايَنتُم بِدَيْنٍ إِلَىٰ أَجَلٍ مُّسَمًّى فَاكْتُبُوهُ وَلْيَكْتُب بَّيْنَكُمْ كَاتِبٌ بِالْعَدْلِ

> "O you who believe, when you contract a debt for a specified term,
> write it down. And let a scribe write it between you in justice."
> *— Surah Al-Baqarah (2:282)*

**Connection grade: Hasan** — 2:282 is the longest verse in the Quran.
It commands written records of debts: amounts, terms, witnesses, every
detail. Recording "I have 3 and owe 5" requires a number for the
deficit. The verse DEMANDS the mathematics of negative position. Without
integers, the command cannot be obeyed. The math is not in the verse's
words — it is in the verse's requirement.

**The problem this ayah creates:** A man stands before the qadi with
3 dinars in his hand and a contract showing he owes 5. The qadi must
write his position. What number does he write? The natural numbers
have no answer. The verse says *write it down* — but in what?

---

## ٢. Al-Khwarizmi Discovers

A man comes to the qadi's court.

He holds three dinars. I can see them — copper catching lamplight in
his open palm. In his other hand, a contract. The creditor's seal at
the bottom. Five dinars owed.

The qadi reads the contract, counts the coins, and asks: "What is
your true position?"

The man says: "I owe two."

The qadi nods. He reaches for his pen. He dips it. Then he stops.

He needs to write a number. Not a sentence — a number. The ledger has
columns: name, position. What goes in the column? Three? No — the man
does not have three to his name, because three already belongs to the
creditor. Five? No — that is what he owes, not what he is. He is not
three and he is not five and he is not zero. He is below zero.

The pen stays raised.

---

I have built three islands of tools. Equality gave me the scale.
Counting gave me the natural numbers: 1, 2, 3, 4, ... Multiplication
gave me growth. At every step, the numbers go up. The shepherd counts
forward. The farmer's harvest accumulates. There is no number in my
system for the place where this man stands.

3 − 5. I write it and stare at it. Within the natural numbers,
subtraction requires the first number to be at least as large as the
second. 7 − 4 = 3. Good. 5 − 5... I do not even have an answer for
that. Nothing came back. What number means "nothing"?

And 3 − 5 is worse than nothing. It is below whatever nothing is.

> *Margin note: The Greek mathematicians faced the same problem and
> refused. They called quantities less than nothing atopon — absurd.
> Brahmagupta of Ujjain accepted them six hundred years ago. He wrote
> the rules in his Brahmasphutasiddhanta. The mathematics does not
> care who is comfortable with it. The man's debt is real whether
> the Greeks approve or not.*

---

I think about the shepherd at the gate. Forty-seven sheep left in the
morning. Forty-seven came back. What is the difference? 47 − 47. No
sheep lost, no sheep gained. The number of missing sheep is... nothing.
Not one. Not any counting number. Just empty.

I need a name for that emptiness. I call it **sifr**. Zero. I write
it: **0**.

It is not nothing in the sense of nonexistence. It is a position on
the ledger. The point where having and owing balance. The shepherd
with all his sheep has a loss of 0. A man with no assets and no debts
has a position of 0.

What happens when I add 0 to something? If a man has 5 dinars and
gains nothing, he still has 5. If a farmer harvests 200 measures
and loses nothing, he still has 200.

<!-- diagram: formal-zero -->

```
a + 0 = a     for every number a
```

This is what "nothing" means in the language of addition. Zero added
to anything leaves it unchanged. I name this: 0 is the **additive
identity**.

---

Now back to the man. He has 3 and owes 5. Suppose he had 5 and owed 5.
He pays everything. He holds nothing. He owes nothing. His position: 0.
The 5 that he held and the 5 that he owed cancelled perfectly.

So for every number, there must be another number — its opposite —
that cancels it back to 0:

<!-- diagram: formal-inverse -->

```
a + (−a) = 0
```

I call `−a` the **additive inverse** of `a`. If `a` is 5 dinars held,
then `−a` is 5 dinars owed. Together they annihilate. The debt is paid.
The ledger returns to zero.

> *Margin note: The Arabic for debt — dayn (دَيْن) — shares its root
> with din (دِين), meaning religion, way of life, judgement. Obligation
> and existence are linked in the language itself.*

---

Now I can write the man's position.

He holds 3. He owes 5. His position: `3 + (−5)`. Three dinars of
having, five dinars of owing. The 3 and 3 of the 5 cancel:
`3 + (−3) = 0`, and `−2` remains.

```
3 + (−5) = −2
```

Two below zero. Two dinars in debt.

The qadi writes it: **−2**.

The pen comes down. The ledger is honest. The verse is obeyed.

<!-- diagram: debtor-position -->

---

I step back and look at what I have built. The natural numbers started
at 1 and climbed: 1, 2, 3, ... Now I have 0 below them. And below 0,
the negatives: −1, −2, −3, ... The complete set — every positive
number, zero, and every negative number — I call the **integers**. I
write them as **Z**.

<!-- diagram: number-line -->

```
        ←  deficit  |  surplus  →

  ──┬────┬────┬────┬────┬────┬────┬────┬──
   -3   -2   -1    0    1    2    3    4
```

<!-- diagram: positive-side -->
<!-- diagram: negative-mirror -->

The number line. Symmetric around zero. Every positive number has a
mirror on the left. The man stands at −2. The creditor, if he were
here, might stand at +2 — the mirror position. What one owes, the
other is owed. The line records both.

---

But I am not done. I have addition of integers. What about
multiplication?

The farmer from the masjid (0.3) taught me that multiplication is
repeated addition. So `3 × (−2)` means "add −2 three times":

```
(−2) + (−2) + (−2) = −6
```

A man borrows 2 dinars each month for 3 months. Total position: −6.
The sign makes sense. Repeated addition of a debt accumulates debt.

What about `(−3) × 2`? "Add 2 negative-three times." That is nonsense.
I cannot add something a negative number of times.

I try a different approach. In the multiplication island, the farmer
found that `a × b = b × a` — walking around the rectangle of stones.
I assumed commutativity holds. If I extend that to integers — and I
must be honest that this IS an extension, not an automatic inheritance
from the naturals — then `(−3) × 2 = 2 × (−3) = (−3) + (−3) = −6`.

> *Margin note: Extending commutativity to Z is an assumption. Not
> arbitrary — it is consistent, and the algebraic structure demands
> it. But "consistent and demanded" is not the same as "proved from
> first principles." I state the assumption and use it.*

Now the hardest question. What is `(−1) × (−1)`?

I cannot use repeated addition. I cannot draw a rectangle with −1 rows
and −1 columns. The intuition that carried me through multiplication
of positives fails completely.

I need the distributive law. The farmer's grain (0.3) gave it to me:
`a × (b + c) = a × b + a × c`. I proved it for natural numbers. I
extend it now to all integers. And from this extension, the answer
will be forced.

Let me follow the chain. The distributive law will not merely suggest
what `(−1) × (−1)` equals. It will leave no other possibility.

---

## ٣. The Derivation

### Zero Under Multiplication

**Claim:** `a × 0 = 0` for every integer `a`.

**Proof.** I know `0 + 0 = 0` (additive identity applied to 0 itself).

Multiply both sides by `a`:

```
a × (0 + 0) = a × 0
```

Apply the distributive law to the left side:

```
a × 0 + a × 0 = a × 0
```

Let `k = a × 0`. Then `k + k = k`. Add `(−k)` to both sides:

```
k + k + (−k) = k + (−k)
k + 0 = 0
k = 0
```

Therefore `a × 0 = 0`. ∎

Any number times nothing is nothing. I did not choose this — the
additive identity and the distributive law forced it.

### Multiplying by −1

**Claim:** `(−1) × a = −a` for every integer `a`.

**Proof.** Start from the additive inverse of 1:

```
1 + (−1) = 0
```

Multiply both sides by `a`:

```
a × (1 + (−1)) = a × 0 = 0       (just proved)
```

Apply the distributive law:

```
a × 1 + a × (−1) = 0
```

Since `a × 1 = a` (multiplicative identity from 0.3):

```
a + a × (−1) = 0
```

The number which, added to `a`, gives 0 is `−a` by definition.
Therefore:

```
a × (−1) = −a
```

By commutativity (extended to Z): `(−1) × a = −a`. ∎

Multiplying by −1 flips a number across zero. Positive becomes
negative. Negative becomes positive. Not by convention. By the
distributive law.

<!-- diagram: formal-double-negative -->

### The Central Proof: (−1) × (−1) = 1

**Proof.** Start from `1 + (−1) = 0`. Multiply both sides by `(−1)`:

```
(−1) × (1 + (−1)) = (−1) × 0 = 0
```

Distribute:

```
(−1) × 1 + (−1) × (−1) = 0
```

I just proved `(−1) × 1 = −1`:

```
−1 + (−1)(−1) = 0
```

The number that, added to −1, gives 0 is 1. Therefore:

```
(−1) × (−1) = 1    ∎
```

I did not choose this. I did not decide by convention that negative
times negative is positive. The distributive law — inherited from
multiplication as repeated addition — combined with the additive
inverse — needed to record the debtor's position — forced the result.
I had no say in it.

The qadi might say it plainly: cancelling a debt IS a gain. If you owe
5 and I cancel 5 of what you owe, you have gained 5. `(−1) × (−5) = 5`.
The removal of a loss is a gain. The structure and the intuition agree.

### Sign Rules (Derived, Not Decreed)

| Operation | Result | Why |
|-----------|--------|-----|
| `(+)(+)` | `+` | Repeated addition of positives |
| `(+)(−)` | `−` | Repeated addition of negatives |
| `(−)(+)` | `−` | `(−1) × a = −a` |
| `(−)(−)` | `+` | `(−1)(−1) = 1` |

Every sign rule is a theorem. None is a decree.

### Properties of the Integers Z

| Property | Addition | Multiplication |
|----------|----------|----------------|
| Closure | `a + b ∈ Z` | `a × b ∈ Z` |
| Commutativity | `a + b = b + a` | `a × b = b × a` (extended) |
| Associativity | `(a+b)+c = a+(b+c)` | `(ab)c = a(bc)` |
| Identity | `a + 0 = a` | `a × 1 = a` |
| Inverse | `a + (−a) = 0` | Not always in Z |
| Distributive | `a(b + c) = ab + ac` | |

Integers are closed under addition, subtraction, and multiplication.
Not division: `(−6) ÷ 4` is not an integer. Division will demand
fractions — the next island.

### The Extension Pattern

```
Problem                    System breaks       Extension
───────────────────────    ─────────────────    ─────────────
"How many?"                     —               N (naturals)
"What if nothing?"         No number for 0      add 0
"What if less than 0?"     No number < 0        N → Z (integers)
"What if parts?"           5 ÷ 3 ∉ Z           Z → Q (next)
```

### The Chain from 1 = 1

```
1 = 1                                    (axiom)
├── Equality: reflexive, symmetric,
│   transitive, preservation             (Island 0.1)
├── Counting: successor, addition,
│   commutative, associative, induction  (Island 0.2)
├── Multiplication: repeated addition,
│   identity, commutative, associative,
│   distributive                          (Island 0.3)
└── Zero and Negatives:
    a + 0 = a, a + (−a) = 0,
    (−1)(−1) = 1                          (Island 0.4)
```

**Geometry spec for Layer (Mode A):**

Six phases. (1) Number line drawn from center outward, zero mark at
center. (2) Positive ticks appear right of zero in green, one by one.
(3) Negative ticks appear left of zero in red — a mirror. "surplus"
and "deficit" labels. (4) The debtor's marker pulses at −2.
(5) Proof chain: `(−1)(1 + (−1)) = 0` → distribute → `(−1)(−1) = 1`.
(6) Direction reversal arrows: an arrow goes right (+1), reverses
left (−1), reverses again right ((−1)(−1) = 1) — ending where it
started. Final frame: the number line glows. 1 = 1 has not been lost.

---

## ٤. Al-Khwarizmi Solves

### Example 1: The Debtor's Full Ledger

The man before the qadi has a longer story than I first heard. He
received 12 dinars from selling cloth. Paid 8 for supplies. Borrowed 7
from a friend. Then repaid 3 of the loan.

I track everything as integers.

<!-- diagram: example-debt -->

```
Start:         0
Sells cloth:   0 + 12       = 12
Buys supplies: 12 + (−8)    = 4
Borrows 7:     Cash: 4 + 7  = 11,  Debt: 0 + (−7)  = −7
Repays 3:      Cash: 11 + (−3) = 8,  Debt: −7 + 3   = −4
```

| Event | Cash | Debt | Net Position |
|-------|------|------|-------------|
| Start | 0 | 0 | 0 |
| Sells cloth +12 | 12 | 0 | 12 |
| Buys supplies −8 | 4 | 0 | 4 |
| Borrows 7 | 11 | −7 | 4 |
| Repays 3 | 8 | −4 | 4 |

Net position: `8 + (−4) = 4`. The qadi records **+4**. *Write it down.*

Notice: borrowing did not change his net position. He gained 7 in cash
and gained 7 in debt. `+7 + (−7) = 0`. The loan cancels itself. Only
the repayment — converting cash into less debt — moves the net
position. The integers reveal what the raw numbers hide.

### Example 2: Cancelling a Debt (The Double Negative)

The debtor has three creditors. He owes 10 to the first, 15 to the
second, 8 to the third. Total debt: `(−10) + (−15) + (−8) = −33`.
The second creditor forgives the entire debt — a gift.

Forgiving a debt of 15 is removing a negative:

<!-- diagram: example-reversal -->

```
−33 + (−(−15)) = −33 + 15 = −18
```

Cancelling a debt IS a gain. `−(−15) = 15` — the additive inverse of
the additive inverse returns to the original. The man still owes 18,
but he is 15 dinars closer to zero. The qadi updates the ledger.

### Example 3: Signs by the Distributive Law

Compute `(−3) × (−4) + (−2) × 5`.

First term: factor out the signs.

```
(−3) × (−4) = (−1)(3) × (−1)(4)
            = (−1)(−1) × (3 × 4)
            = 1 × 12
            = 12
```

Second term: one negative sign.

```
(−2) × 5 = (−1)(2)(5) = (−1)(10) = −10
```

Sum: `12 + (−10) = 2`.

Every sign was determined by the distributive law. Nothing was
arbitrary.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** Compute:
(a) `4 + (−7)`
(b) `(−3) + (−5)`
(c) `0 + (−6)`
(d) `(−4) + 4`
*Hint for (d): what is the definition of additive inverse?*

**2.** A shepherd leaves with 30 sheep. During the day, 3 are lost.
He finds 1 stray that is not his. He returns and counts: how many of
his own does he have? Write the day as a sum of integers.
*Hint: the stray is not his — gaining it does not change HIS count.*

<!-- diagram: ex-daif-numberline -->

**3.** The debtor before the qadi has 15 dinars in hand. He owes 8 to
one creditor, 6 to another, and 4 to a third. Write his position as a
sum of integers and compute. Is he in surplus or deficit?
*Hint: position = cash + debts = 15 + (−8) + (−6) + (−4).*

### Hasan (Exam-level)

**4.** Compute, showing your reasoning for each sign: [4 marks]
(a) `(−2) × (−3) × (−1)`
(b) `(−5) × (−5)`
(c) `(−1) × (−1) × (−1) × (−1) × (−1) × (−1) × (−1)`
(d) `(−1)¹⁰⁰`

<!-- diagram: ex-hasan-proof -->

**5.** The debtor before the qadi has 20 dinars. He owes 8, 6, and 11
to three creditors, to be paid in that order. [4 marks]
(a) What is his net position?
(b) After paying the first debt of 8, what does he hold? After paying
the second of 6?
(c) He now has 6 dinars and owes 11. He pays what he can. What is his
position after paying?
(d) Write the qadi's ledger as a running total, showing the point
where the man first enters deficit.

**6.** Expand using the distributive law: [3 marks]
(a) `(−3)(x + 4)`
(b) `(−1)(a + b + c)`
(c) `5(2 + (−3))`
Verify (c) by computing inside the brackets first.

**7.** A merchant's ledger shows six monthly positions:
`+12, −5, +8, −15, +3, −7`. [3 marks]
(a) What is his total position after 6 months?
(b) Compute the running total month by month. In which month does it
first become negative?

### Sahih (Proof and extension)

**8.** Prove that the additive inverse is unique: if `a + b = 0` and
`a + c = 0`, then `b = c`. [4 marks]
*Hint: start from `a + b = a + c` and use the preservation principle
from Island 0.1.*

**9.** Prove that `(−a)(−b) = ab` for any integers `a, b`, using only
the distributive law, additive identity, additive inverse, and
multiplicative identity. [5 marks]

**10.** Prove that `(−1)ⁿ = 1` if `n` is even, and `(−1)ⁿ = −1` if
`n` is odd. [4 marks]
*Hint: write n = 2k or n = 2k + 1 and use the result (−1)(−1) = 1
repeatedly. You may use induction from Island 0.2.*

---

## ٦. Exam Technique

> **Sign errors** lose more marks than any other single mistake on the
> Edexcel paper. The cure: never guess a sign. Derive it.
>
> **Technique 1: Factor out (−1).**
> `(−3) × (−4) = (−1)(3)(−1)(4) = (−1)²(12) = 1 × 12 = 12`
> Each negative number is (−1) times its absolute value. Collect the
> (−1)s and count.
>
> **Technique 2: Count the negatives.**
> Even count of negative factors → positive result. Odd count → negative.
> `(−2)(−3)(−4)` → three negatives → odd → `−(2 × 3 × 4) = −24`
>
> **Technique 3: Subtraction IS addition of the inverse.**
> Never think of subtraction as its own operation. Rewrite:
> `5 − (−3) = 5 + (−(−3)) = 5 + 3 = 8`.
>
> **The bracket trap:** `−x²` versus `(−x)²`. When `x = 3`:
> - `−x² = −(3²) = −9` — the negative is NOT part of the base
> - `(−x)² = (−3)² = 9`
>
> When in doubt, write the brackets. Every time. The mark scheme does
> not reward bravery.
>
> **Is −0 = 0?** Yes. By definition, `0 + (−0) = 0`. But also
> `0 + 0 = 0`. Both 0 and −0 satisfy the equation. Since the additive
> inverse is unique (Problem 8 above), `−0 = 0`. Zero is its own mirror.

---

## ٧. Log Pose

```
                    ┌──────────┐
                    │ Prologue │
                    │ 1 = 1    │
                    └────┬─────┘
                         │
                    ┌────▼─────┐
              ┌─────┤ 0.1 ═══ ├─────┐
              │     │ Equality │     │
              │     └────┬─────┘     │
              │          │           │
         ┌────▼───┐      │      ┌───▼────┐
         │  0.2   │      │      │  0.6   │
         │ Count  │      │      │ Vars   │
         └───┬────┘      │      └────────┘
             │           │
         ┌───▼────┐      │
         │  0.3   │      │
         │ Mult   │      │
         └───┬────┘      │
             │           │
         ┌───▼────┐      │
    ┌────┤  0.4   ├──────┘
    │    │ Zero/  │
    │    │ Neg    │
    │    └───┬────┘
    │        │
    │    ┌───▼────┐
    │    │  0.5   │
    │    │ Frac   │
    │    └────────┘
    │
    └──→ Arc 1: Complex numbers
         (what if x² = −1?)
```

**This island unlocks:**
- **Island 0.5** — Fractions: the inheritance finally computed

**Dependencies used:**
- 0.1 Equality (preservation: add the same to both sides)
- 0.2 Counting (the naturals — the system we extended through zero)
- 0.3 Multiplication (the distributive law that forced every sign rule)

**Forward connections to FP1:**
- Negative numbers → complex numbers (Arc 1: what happens when
  `x² = −1`?)
- Sign rules → manipulation of surds and rational expressions
- Additive inverse → solving equations by "undoing" (Island 0.6)

**Inheritance callback:** The estate may carry debts. The Quran
commands: debts are paid BEFORE inheritance shares are distributed —
*min ba'di wasiyyatin yusi biha aw dayn* (4:11, "after any bequest
or debt"). If the dead man owed more than he owned, the estate's
position is negative. The heirs receive nothing until the debt is
cleared. Negative numbers are not a curiosity. They are the
prerequisite for just inheritance.

---

## ٨. Reflection

The qadi's pen came down.

That is what happened. A man stood before a judge with an honest
position that honest mathematics could not write, and now it can.
The number −2 is not a trick. It is not a convention agreed upon for
convenience. It is the only answer consistent with the tools I already
had — the additive identity, the additive inverse, the distributive
law. The structure demanded it. I recorded it.

The debtor left the court with his position in the ledger. The
creditor has the same number with the opposite sign. Both entries are
true. Both are necessary. Together they sum to zero — the debt exists
between them, perfectly balanced, waiting to be resolved.

And the sign rules. A student who memorizes "negative times negative
is positive" holds a fact. A student who sees the distributive law
force the result — who follows the chain from `1 + (−1) = 0` through
multiplication to the only possible answer — holds understanding. The
fact can be forgotten. The chain cannot. Cancelling a debt is a gain.
The mathematics says what the merchant already knows.

I have integers now. The number line stretches in both directions. I
can record surplus and deficit with equal precision. But the family
from the prologue is still waiting. The wife's share is 1/8. The
daughters' share is 2/3. The parents each receive 1/6. These are not
integers. They live between the whole numbers. 1/8 is less than 1
but more than 0 — a position my number line can point to but my
integers cannot name.

A grieving family sits before me. The father has still not spoken. The
mother is still seated. The wife has gathered the daughters close.
They need fractions. They need to cut whole things into exact pieces
and name each piece. The tools must extend again.

*1 = 1 has not been lost.* The additive identity preserves it:
`1 + 0 = 1`. The inverse restores it: `1 + (−1) + 1 = 1`. The sign
rule confirms it: `(−1)(−1) = 1`. At every extension, the ground holds.

---

*End of Island 0.4. Next: Island 0.5 — Fractions.*
