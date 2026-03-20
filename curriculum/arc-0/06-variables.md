# Island 0.6: Variables — The Merchant's Unknown

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> وَإِن مِّن شَيْءٍ إِلَّا عِندَنَا خَزَائِنُهُ وَمَا نُنَزِّلُهُ إِلَّا بِقَدَرٍ مَّعْلُومٍ
> "There is not a thing (shay') but that with Us are its depositories,
> and We do not send it down except in a known measure."
> *— Surah Al-Hijr (15:21)*

**Connection grade: Honest Chain** — The verse is about divine provision, not algebra. The link is linguistic: Al-Khwarizmi used *shay'* (thing) for the unknown quantity. Latin translators rendered it *xay*, shortened to *x*. The word that names the unknown in every algebra classroom is Quranic Arabic. Chain: verse uses *shay'* --> Al-Khwarizmi adopts it for algebra --> *shay'* becomes *x*. Each link is real. Word-overlap, not structural correspondence. Honest Chain, not Hasan.

**The problem this ayah creates:** A merchant owes zakat — one part in forty of his total wealth. He knows the rule. He does not know the number. Every tool I have built requires a known input. How do I compute with something that does not yet exist?

---

## ٢. Al-Khwarizmi Discovers

The door opens. The smell enters before the man does — sandalwood and sea salt, layered with something sharper underneath. Ink.

He is broad across the shoulders, but it is the fingers I notice. Stained black at the tips. A man who keeps his own ledgers. He sets a leather-bound book on the table and opens it. Columns of figures, tidy, precise.

"I must pay zakat," he says. "One part in forty. I know the rule."

"Then compute it."

He shakes his head. "Three ships at sea. Two warehouses uncounted since Ramadan. Debts owed by four men, two of whom I may never see again."

He taps the open ledger. "This is what I know." He gestures at the air. "This is what I don't."

---

I stare at his ledger. The columns are there. The headings are there. But the numbers beneath many of them — blank. Marked with question marks in his own hand.

What is one-fortieth of the merchant's wealth? His wealth is — what? I reach for a number and there is nothing to grasp. Every operation I have built across five islands starts the same way: take THIS number, do THAT to it. The number comes first.

His number does not exist.

> *Margin note: Five islands of tools. Every one assumes a known starting number. Not one of them can begin from nothing.*

---

"Tell me what you do know," I say.

He counts on his ink-stained fingers. "House and workshop: eight thousand. Near warehouse: four thousand. Reliable debts: twelve hundred. The rest — I do not know."

"So at least thirteen thousand two hundred. And something more."

"I cannot pay zakat on a guess. Underpayment is theft from the poor."

I write:

```
Known:   8000 + 4000 + 1200 = 13200
Unknown: ships + far warehouse + uncertain debts = ???
Total:   13200 + ???
```

I cannot add 13200 to a blank space. The arithmetic stops at the edge of what he knows.

---

I put down my pen. His arithmetic cannot START. He has one number and an absence.

But the absence is not nothing. Those ships carry real cargo. The value is definite — fixed at this moment, real as the 8000 dinars in his house. He simply does not know what it is.

What if I gave the unknown a name?

---

I call it *shay'*. A thing. I write it as a single letter:

<!-- diagram: unknown-box -->

> *A golden box, empty, labeled with a single character. The unknown quantity. Not a number. Not yet. A place where the number will go when it arrives.*

```
x
```

His total wealth:

```
Total = 13200 + x
```

His zakat:

```
zakat = (13200 + x) / 40
```

I stare at what I have written. It is not a number. It is a SENTENCE about numbers — a relationship that holds regardless of what x turns out to be. If x is 5000, the zakat is 18200/40 = 455. If x is 20000, the zakat is 33200/40 = 830. The structure is settled. The number waits for his ships.

---

But *shay'* does more than label. It lets me reason.

Whatever his wealth W, he keeps W - W/40 = 39W/40. I did not need to know W. The relationship is fixed before the ships dock, after they dock, whether or not they dock at all.

His partner tells him: "After paying zakat, you should have at least 19500 dinars."

<!-- diagram: equation-balance -->

> *A scale. On the left pan: a golden box marked 39W/40. On the right pan: the number 19500. The beam is level. The equation: the claim that these two are equal.*

```
39W/40 = 19500
```

I use the tool from Island 0.1. Multiply both sides by 40:

```
39W = 780000
```

Divide both sides by 39:

```
W = 20000
```

<!-- diagram: isolate -->

> *Three frames. First: the box buried under layers — multiplication by 39, division by 40. Second: one layer peels away (multiply by 40). Third: the second layer peels away (divide by 39). The box stands alone. The number inside is revealed: 20000.*

Check: 20000/40 = 500 dinars in zakat. 20000 - 500 = 19500. ✓

I did not guess. I named what I didn't know, and the algebra extracted the answer.

---

His first ship docks three days later. The cargo: 4800 dinars of silk, spices, copper.

```
New known: 13200 + 4800 = 18000
Still unknown: y  (second ship, far warehouse, uncertain debts)
zakat ≥ 18000/40 = 450
```

"I will pay 450 now," he says. "And adjust when the second ship docks."

Not estimation. A lower bound from exact reasoning. The variable lets him act on partial knowledge without waiting for certainty.

---

## ٣. The Derivation

### Variables and expressions

A **variable** is a symbol representing a quantity whose value is not yet determined. I write it as a letter: x, y, z, W.

An **expression** combines variables, numbers, and operations:

<!-- diagram: formal-expression -->

> *Four expressions displayed: 3x + 7, x/40, 13200 + x, 39W/40. Each is a recipe — numbers and operations with a golden box where the unknown sits.*

```
3x + 7
x/40
2x² - 5x + 1
13200 + x
```

An expression has no truth value. It is not true or false. It is a recipe — waiting for a number to substitute into.

### Expressions vs equations

An **equation** sets two expressions equal: `39x/40 = 19500`. This is a claim — true for some values of x, false for others. The value that makes it true is the **solution**.

| | Expression | Equation |
|---|---|---|
| Example | `3x + 7` | `3x + 7 = 22` |
| Truth value | None | True or false |
| Purpose | Describe | Claim |
| Action | Simplify | Solve |

### The arithmetic of expressions

Variables obey every law from Islands 0.1-0.5. No new axioms:

```
Commutative:   x + 3 = 3 + x,  2 × x = x × 2
Associative:   (x + 3) + 5 = x + 8
Distributive:  3(x + 4) = 3x + 12
Inverse:       x + (-x) = 0,  x × (1/x) = 1 (x ≠ 0)
```

### Collecting like terms

The distributive law, reversed:

```
5x + 3x = (5 + 3)x = 8x
3x + 4y - x + 2y = 2x + 6y
```

Terms with different variable parts do not combine. `3x + 4y` is already simplified — three bolts of silk and four sacks of spice do not become seven of anything.

### Substitution

Replace the variable with its value: if x = 5000, then (13200 + x)/40 = 18200/40 = 455. Substitution is how expressions become numbers and equations become verifiable.

### Solving linear equations

A **linear equation** has x to the first power only: `ax + b = c` where a ≠ 0.

<!-- diagram: formal-linear-solve -->

> *A balance scale in three states. State 1: ax + b on the left, c on the right, beam level. State 2: subtract b from both sides. State 3: divide both by a — the box is isolated.*

Isolate x using Island 0.1 — what I do to one side, I do to the other:

```
ax + b = c  →  ax = c - b  →  x = (c - b) / a
```

In standard form ax + b = 0:

```
+---------------------------------------+
|                                       |
|  If ax + b = 0 and a ≠ 0, then:      |
|                                       |
|         x = -b / a                    |
|                                       |
+---------------------------------------+
```

**Special cases:**
- a = 0, b ≠ 0: the equation says b = 0, which is false. No solution.
- a = 0, b = 0: the equation says 0 = 0, which is always true. Every number is a solution.

### Verification

After solving, substitute back into the *original* equation:

```
Solve: 5x - 3 = 22  →  5x = 25  →  x = 5
Verify: 5(5) - 3 = 25 - 3 = 22  ✓
```

Verification is the same principle as the scale in Island 0.1.

### Rearranging formulas

From `z = x/40`, multiply both sides by 40: `40z = x`. Same equation, two perspectives. The zakat from the wealth, or the wealth from the zakat.

**The chain from 1 = 1:**

```
1 = 1  →  equality preserved [0.1]  →  arithmetic [0.2-0.5]
  →  variable: symbol obeying all laws [this island]
  →  expression  →  equation  →  x = -b/a  →  substitution
```

No new axioms. The variable inherits the entire structure already built.

**Geometry spec for Layer (Mode A):**
Six frames. Golden box (shay') buried under operations on a balance scale. Operations peel away from both sides. The box isolates. It opens, revealing the number. End card: *Variables — الشيء / Al-Khwarizmi — 780-850 CE — Baghdad / 15:21*.

---

## ٤. Al-Khwarizmi Solves

### Worked Example 1: The merchant's zakat equation

<!-- diagram: example-zakat -->

> *The merchant's problem, solved step by step. A golden box labeled x on a balance scale, numbers on the other side, layers peeling away.*

The merchant paid 625 dinars in zakat. What was his total wealth?

Let x = total wealth.

```
x / 40 = 625
```

Multiply both sides by 40:

```
x = 625 × 40
x = 25000
```

Check: 25000/40 = 625. ✓

The merchant's wealth was **25,000 dinars**.

---

### Worked Example 2: A simple linear equation

<!-- diagram: example-simple-linear -->

> *A scale: 5x - 3 on the left, 22 on the right. Two operations: add 3, divide by 5. The box isolates to reveal 5.*

```
5x - 3 = 22
5x = 25        (add 3 to both sides)
x = 5          (divide both sides by 5)
Verify: 5(5) - 3 = 22  ✓
```

---

### Worked Example 3: Two warehouses

The merchant's two warehouses total 28,000 dinars. The first holds three times the second. Let y = second warehouse.

```
y + 3y = 28000  →  4y = 28000  →  y = 7000
```

Second: **7000**. First: **21,000**. Check: 7000 + 21000 = 28000. ✓

Zakat on warehouse goods: 28000/40 = **700 dinars**.

---

## ٥. Your Turn

### Da'if (Guided)

**D1.** Simplify: (a) 4x + 7x  (b) 9y - 3y + 2y  (c) 5x + 3 - 2x + 8  (d) 7a + 4b - 3a + b

*Hint: Group terms with the same variable.*

**D2.** Substitute x = 4 into each expression:

<!-- diagram: ex-daif-substitute -->

> *A golden box labeled x. An arrow: the box opens, the number 4 drops in. The expression transforms into pure arithmetic.*

(a) 3x + 5  (b) x² - 2x  (c) (x + 6)/2  (d) 40 - 7x

**D3.** Solve for x: (a) x + 5 = 12  (b) 3x = 21  (c) x/4 = 9  (d) 2x - 7 = 13

*Hint: Inverse operation on both sides. Check by substituting back.*

---

### Hasan (Exam-level)

**H1.** Solve for x [3 marks each]:  (a) 5x + 3 = 2x + 18  (b) 4(x - 2) = 3(x + 1)  (c) (x + 5)/3 = 7

<!-- diagram: ex-hasan-solve -->

> *Three scales, each with a golden box and numbers. The student must isolate the box.*

**H2.** The merchant has goods in three locations. The harbor holds twice the market stall. The ship cargo is 5000 more than the harbor. Total: 43,000 dinars. [5 marks]

(a) Let y = market stall value. Express the other two in terms of y. [1]
(b) Write and solve the equation for y. [2]
(c) Find each location's value. [1]
(d) Compute total zakat at 1/40. [1]

**H3.** An estate: wife receives 1/8, son receives twice the daughter's share, three shares exhaust the estate. The daughter receives 2625 dinars. Find the total estate. [4 marks]

*Hint: Let d = daughter's share. Son = 2d. Wife = x/8. Write x/8 + 3d = x.*

---

### Sahih (Proof and extension)

**S1.** Solve for x, expressing answers as fractions in lowest terms: [4 marks each]

(a) (2x + 1)/3 - (x - 4)/5 = 2

(b) 3(x - 1)/4 + 2 = (5x + 3)/6

**S2.** Generalize the inheritance from Island 0.5. An estate x is divided among a wife (1/8), two daughters (2/3), a father (1/6), and a mother (1/6). 'Awl adjusts each share proportionally. [8 marks]

(a) Show the prescribed shares sum to 27/24 and that 'awl is required. [2 marks]
(b) Write each heir's share as a fraction of x after 'awl. Verify they sum to x. [3 marks]
(c) If the wife's share after 'awl equals 3000 dinars, find x. [3 marks]

---

## ٦. Exam Technique

> **EXAM NOTE: Setting up equations from word problems**
>
> Method marks (M) are for the equation. Accuracy marks (A) are for
> the solution. You CANNOT earn A without M. The equation is where
> the marks begin.
>
> 1. **Name the unknown.** Write "Let x = ..." State what x represents.
> 2. **Express quantities in terms of x.** "A quarter of the estate" --> x/4.
> 3. **Find the equation.** Look for "equals," "is," "totals," "gives."
> 4. **Solve. Show every line.** Each line is a potential method mark.
> 5. **Check.** Substitute into the ORIGINAL equation.
>
> **Common errors:**
> - Answering a different question than asked. Re-read after solving.
> - Converting to decimals. If x = 27/7, report 27/7. Fractions are exact.
> - The word "of" means multiply: "1/8 of the estate" --> x/8.

---

## ٧. Log Pose

```
                  +--- 0.7 Quadratic Equations
                  |    (the patron's square garden)
                  |
0.6 Variables ----+
(equations)       |
                  |
                  +--- 0.8 Irrational Numbers
                       (the builder's diagonal)
```

**This island unlocks:** Quadratic Equations (0.7), where x appears squared and linear tools break.

**Connection forward to FP1:** The linear equation ax + b = 0 has exactly one solution. The quadratic ax² + bx + c = 0 can have zero, one, or two. A polynomial of degree n can have up to n roots. The variable born here carries all the way to the Fundamental Theorem of Algebra.

---

## ٨. Reflection

The merchant came with a rule and an absence. His numbers were incomplete. His obligation was not.

I named the unknown. *Shay'*. A thing. The equation held without the number. The variable captures structure — what he owes depends not on the specific amount but on the relationship between wealth and zakat.

When his ship docked, the equation updated. He paid 450 dinars immediately — exact, not a guess. Obedience did not require omniscience. It required honesty about what he knew and a way to reason about what he didn't.

```
1 = 1
+-- 0.1 Equality: a thing is itself
+-- 0.2 Counting: one, then another
+-- 0.3 Multiplication: repeated addition
+-- 0.4 Zero and negatives: absence and debt
+-- 0.5 Fractions: the inheritance, 'awl
+-- 0.6 Variables: the unknown estate -- here
```

Six islands. The merchant showed me that tools built for known numbers break when the number is absent. Not because they are wrong. Because they assumed something that is not always true: that the input exists. The unknown is not the enemy of computation. It is the beginning of it.

Now the next problem. A patron stands in his courtyard. His garden is 10 cubits by 10 cubits. He wants to double the area. I will write x² + 20x = 100, and the unknown will be squared — multiplied by itself. I will try to isolate it the way I isolated the merchant's x. It will not move.

I will need al-jabr itself.

*1 = 1 has not been lost.*

---
