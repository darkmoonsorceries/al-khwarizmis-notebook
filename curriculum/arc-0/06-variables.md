# Island 0.6: Variables — The Merchant's Unknown

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> وَأَقِيمُوا الصَّلَاةَ وَآتُوا الزَّكَاةَ
> "And establish prayer and give zakat."
> *— Surah Al-Baqarah (2:43)*

**Connection grade: HONEST CHAIN** — The verse commands zakat. Obeying requires computing a fraction of one's wealth. When that wealth is unknown — ships at sea, warehouses uncounted — the computation requires a placeholder for the unknown quantity. The chain: verse commands zakat → zakat requires computation → computation on unknown wealth requires variables. Each link is real.

**The problem this ayah creates:** A merchant owes zakat — one part in forty of his total wealth. He knows the rule. He does not know the number. Every tool I have built requires a known input. His input does not exist yet.

---

## ٢. Al-Khwarizmi Thinks

The door opens. The smell enters before the man does — sandalwood and sea salt, layered with something sharper underneath. Ink.

He is broad across the shoulders. His hands are large, but it is the fingers I notice. Stained black at the tips. A man who keeps his own ledgers. He sits across from me, sets a leather-bound book on the table, and opens it. Columns of figures, tidy, precise. A merchant who trusts his own pen more than any clerk's.

"I must pay zakat," he says. "One part in forty. I know the rule."

"Then compute it."

He shakes his head. "I have three ships at sea. They carry silk, spices, copper. I do not know what survived the crossing. I have two warehouses in the eastern quarter — the inventory has not been taken since Ramadan. I have debts owed to me by four men, two of whom I may never see again."

He taps the open ledger. "This is what I know." He gestures at the air. "This is what I don't."

---

I stare at his ledger. The columns are there. The headings are there. But the numbers beneath them — many are blank. Estimated. Marked with question marks in his own hand.

Let me try what I know.

Zakat is one-fortieth of total wealth. In the inheritance problem, I computed one-eighth of 2700. That was:

```
2700 / 8 = 337.5
```

I knew 2700. I knew 8. I divided. The answer came.

What is one-fortieth of the merchant's wealth? His wealth is — what? I reach for a number and there is nothing to grasp. The calculation cannot begin. Not because the method is wrong. Because the method requires something I do not have.

I can add known numbers. Multiply them. Find their fractions. Reduce them with 'awl. Every operation I have built across five islands begins the same way: take *this* number, do *that* to it. The number comes first. The operation follows.

> *Margin note: Five islands of tools. Every one assumes a known starting number. Not one of them can begin from nothing.*

The merchant watches me. He has seen this pause before — in other scholars, other scribes. Men who can compute anything, as long as you hand them a number. He did not come with a number. He came with a rule and an absence.

---

"Tell me what you do know," I say.

He counts on his ink-stained fingers. "My house and workshop — I have had them appraised. Eight thousand dinars. The goods in the near warehouse, I counted last month: four thousand. The debts owed to me by reliable men: twelve hundred." He pauses. "The rest I do not know. My ships, my far warehouse, the debts from men who have disappeared."

"So your wealth is at least thirteen thousand two hundred. And something more."

"Something more. But what? I cannot pay zakat on a guess. Underpayment is theft from the poor. Overpayment — I am not so rich that I can be careless."

I write:

```
Known:   8000 + 4000 + 1200 = 13200
Unknown: ships + far warehouse + uncertain debts = ???
Total:   13200 + ???
```

I cannot add 13200 to a blank space. I cannot divide the sum by 40. The arithmetic stops at the edge of what he knows, and his obligation stretches past that edge.

---

I put down my pen.

The merchant's problem is not that his arithmetic is hard. It is that his arithmetic cannot *start*. Addition requires two numbers. Multiplication requires two numbers. Division requires two numbers. He has one number and an absence.

But the absence is not nothing. His unknown wealth exists. Those ships carry real cargo. The far warehouse holds real goods. The value is definite — fixed at this moment, real as the 8000 dinars in his house. He simply does not know what it is.

What if I gave the unknown a name?

---

I call it shay'. A thing. I write it as a single letter, the way I would write any number:

```
x
```

Not a number. Not yet. A name for the number I do not have. A place where the number will go when it arrives.

His total wealth:

```
Total = 13200 + x
```

His zakat:

```
zakat = (13200 + x) / 40
```

> *Margin note: Shay' — "thing." The word Al-Khwarizmi used. Latin translators rendered it as "xay," then shortened it to x. The unknown has carried this name for twelve hundred years.*

I stare at what I have written. It is not a number. It is a *sentence* about numbers — a relationship that holds regardless of what x turns out to be. If x is 5000, the zakat is 18200/40 = 455. If x is 20000, the zakat is 33200/40 = 830. I do not know which. But the *structure* is settled.

The merchant leans forward. He can read equations. "You have written what I owe without knowing what I have."

"I have written the *relationship* between them. The number waits for your ships."

---

But shay' does more than label the unknown. It lets me reason about it.

The merchant says: "When my ships return, suppose my total wealth after counting everything is W. I pay zakat. The amount remaining is what I actually keep."

```
Remaining = W - W/40
```

I simplify. W is forty-fortieths. W/40 is one-fortieth.

```
Remaining = 40W/40 - W/40 = 39W/40
```

Whatever his wealth, he keeps thirty-nine fortieths of it. I did not need to know W. The relationship between wealth and remainder is fixed before the ships dock, after they dock, whether or not they dock at all.

Now a harder question. The merchant says: "My partner tells me that after paying zakat, I should have at least 19500 dinars, based on what he estimates my total holdings are worth. What does that mean my total wealth is?"

```
39W/40 = 19500
```

I need W. The equation has it. I use the tool from Island 0.1 — what I do to one side, I do to the other.

Multiply both sides by 40:

```
39W = 780000
```

Divide both sides by 39:

```
W = 20000
```

Check: 20000/40 = 500 dinars in zakat. 20000 - 500 = 19500. The equation holds.

I did not guess. I did not try numbers until one worked. I wrote what I knew, named what I didn't, and the algebra — the manipulation of the equation — extracted the answer.

---

I go back to the inheritance.

In Island 0.5, I computed the shares for 2700 dinars. The qadi will see another family tomorrow. A different estate — different number, same heirs, same 'awl. Must I repeat the entire calculation?

Let the estate be x. The 'awl adjustments do not change. The denominator rises from 24 to 27 regardless of the amount:

| Heir | Prescribed | After 'awl | Amount |
|------|-----------|------------|--------|
| Wife | 1/8 → 3/24 | 3/27 | 3x/27 = x/9 |
| Two daughters | 2/3 → 16/24 | 16/27 | 16x/27 |
| Father | 1/6 → 4/24 | 4/27 | 4x/27 |
| Mother | 1/6 → 4/24 | 4/27 | 4x/27 |

```
x/9 + 16x/27 + 4x/27 + 4x/27
= 3x/27 + 16x/27 + 4x/27 + 4x/27
= 27x/27
= x  ✓
```

One computation. Every estate. The variable freed me from repeating the same logic with different numbers forever.

> *Margin note: This is what the inheritance problem looked like before I had a name for the unknown. I computed one case. Now I compute ALL cases.*

The merchant watches me work through this. "You are doing for the qadi what you did for me," he says. "Writing the rule, not the instance."

Exactly.

---

His first ship docks three days later.

A boy runs to find me. The merchant is at the harbor, ink and ledger in hand, counting crates as they come off the gangplank. Silk from Khorasan — 200 bolts. Spices — saffron, cardamom, pepper. Copper ingots, twelve.

By the time the sun sets, he has a number. The ship carried goods worth 4800 dinars.

His known wealth updates:

```
Known before:  13200
Ship 1:        4800
New known:     18000
Still unknown:  y   (second ship, far warehouse, uncertain debts)
```

His zakat equation updates:

```
zakat = (18000 + y) / 40
```

The minimum he owes — if the remaining unknowns turn out to be zero — is 18000/40 = 450 dinars. He can begin paying now. If more arrives, he pays more. The variable lets him act on partial knowledge without waiting for certainty.

"I will pay 450 now," he says. "And adjust when the second ship docks."

This is not estimation. It is a lower bound derived from exact reasoning. The variable holds the door open for what he does not yet know.

---

The transition from expression to equation — from writing `x/40` to writing `39x/40 = 19500` and solving for x — is the jump this island makes. An expression describes. An equation *claims*. And a solution *answers*.

What I need next is the formal machinery.

---

## ٣. The Derivation

### Variables and expressions

A **variable** is a symbol representing a quantity whose value is not yet determined. I write it as a letter: x, y, z, W.

An **expression** combines variables, numbers, and operations:

```
3x + 7
x/40
2x² - 5x + 1
13200 + x
```

An expression has no truth value. It is not true or false. It is a recipe — waiting for a number to substitute into.

### Expressions vs equations

An **equation** sets two expressions equal:

```
39x/40 = 19500
```

This is a *claim*. It is true for some values of x and false for others. The value that makes it true is the **solution**.

| | Expression | Equation |
|---|---|---|
| Example | `3x + 7` | `3x + 7 = 22` |
| Truth value | None | True or false |
| Purpose | Describe | Claim |
| What we do with it | Simplify | Solve |

### The arithmetic of expressions

Variables obey every law from Islands 0.1-0.5. No new axioms. The variable inherits the entire structure:

| Law | With numbers | With variables |
|-----|-------------|---------------|
| Commutative (add) | 3 + 5 = 5 + 3 | x + 3 = 3 + x |
| Commutative (mult) | 4 × 7 = 7 × 4 | 2 × x = x × 2 |
| Associative (add) | (2 + 3) + 4 = 2 + (3 + 4) | (x + 3) + 5 = x + (3 + 5) = x + 8 |
| Distributive | 3 × (4 + 5) = 12 + 15 | 3(x + 4) = 3x + 12 |
| Additive inverse | 5 + (-5) = 0 | x + (-x) = 0 |
| Multiplicative inverse | 8 × (1/8) = 1 | x × (1/x) = 1, provided x ≠ 0 |

### Collecting like terms

The distributive law, reversed:

```
5x + 3x = (5 + 3)x = 8x
7x - 2x = (7 - 2)x = 5x
3x + 4y - x + 2y = (3 - 1)x + (4 + 2)y = 2x + 6y
```

Terms with different variable parts do not combine. `3x + 4y` is already simplified — three bolts of silk and four sacks of spice do not become seven of anything.

### Substitution

When the unknown becomes known, replace the variable with its value and compute:

```
If x = 5000:
  13200 + x = 13200 + 5000 = 18200
  (13200 + x)/40 = 18200/40 = 455
```

Substitution is how an expression becomes a number and how an equation becomes verifiable.

### Solving linear equations

A **linear equation** has the unknown to the first power only. General form:

```
ax + b = c     where a ≠ 0
```

Solving means isolating x. The tool is Island 0.1 — what I do to one side, I do to the other.

**Step 1.** Subtract b from both sides:

```
ax = c - b
```

**Step 2.** Divide both sides by a (permitted because a ≠ 0):

```
x = (c - b) / a
```

In the standard form ax + b = 0:

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

After solving, substitute back into the *original* equation. If both sides are equal, the solution is correct. If not, there is an error.

```
Solve: 5x - 3 = 22
  5x = 25
  x = 5

Verify: 5(5) - 3 = 25 - 3 = 22  ✓
```

Verification is not optional. It is the check that closes the loop — the same principle as the scale in Island 0.1.

### Rearranging formulas

Any equation can be rearranged for a different variable. The same equality-preservation principle applies.

From `z = x/40`:
- Multiply both sides by 40: `40z = x`
- The same equation, two perspectives. One tells you the zakat from the wealth. The other tells you the wealth from the zakat.

**The chain from 1 = 1:**

```
1 = 1
  → equality preserved under operations              [Island 0.1]
  → arithmetic: commutative, associative,
    distributive, identity, inverse                   [Islands 0.2-0.5]
  → variable: symbol obeying all these laws           [this island]
  → expression: variables + numbers + operations
  → equation: two expressions set equal
  → linear solution: x = -b/a, from preservation of equality
  → substitution: variable becomes number, equation becomes verifiable
```

No new axioms were introduced. The variable is a placeholder that inherits the entire structure already built.

---

## ٤. Al-Khwarizmi Solves

### Worked Example 1: The merchant's zakat

The merchant's total wealth, after all ships return and all warehouses are counted, is found to be 20,000 dinars. His zakat is one-fortieth.

```
zakat = 20000 / 40 = 500 dinars
```

But suppose instead we are told: the merchant paid 625 dinars in zakat. What was his wealth?

Let x = total wealth.

```
x / 40 = 625
x = 625 × 40
x = 25000
```

Check: 25000/40 = 625. ✓

The merchant's wealth was **25,000 dinars**.

---

### Worked Example 2: The inheritance, reversed

The wife from the prologue received her share of an estate. After paying the wife 1/9 of the estate (the 'awl-adjusted share from Island 0.5), 4800 dinars remain among the other heirs. What was the estate?

Let x = total estate. Wife receives x/9. The rest receive:

```
x - x/9 = 4800
9x/9 - x/9 = 4800
8x/9 = 4800
```

Multiply both sides by 9:

```
8x = 43200
```

Divide both sides by 8:

```
x = 5400
```

Check: wife receives 5400/9 = 600. Remainder: 5400 - 600 = 4800. ✓

The estate was **5400 dinars**.

---

### Worked Example 3: Two warehouses

The merchant's two warehouses together hold goods worth 28,000 dinars. The first holds three times the value of the second. What does each warehouse hold? What is his zakat on the warehouse goods alone?

Let y = value in the second warehouse. The first warehouse holds 3y.

```
y + 3y = 28000
4y = 28000
y = 7000
```

Second warehouse: **7000 dinars**. First warehouse: 3 × 7000 = **21,000 dinars**.

Check: 7000 + 21000 = 28000. ✓

His zakat on warehouse goods:

```
28000 / 40 = 700 dinars
```

The merchant traces the answer with his ink-stained finger. Seven hundred dinars. He writes it in his ledger.

---

## ٥. Your Turn

### Da'if (Guided)

**D1.** Simplify by collecting like terms:

(a) 4x + 7x
(b) 9y - 3y + 2y
(c) 5x + 3 - 2x + 8
(d) 7a + 4b - 3a + b

*Hint: Group terms with the same variable. Constants are their own group.*

**D2.** Solve for x:

(a) x + 5 = 12
(b) 3x = 21
(c) x/4 = 9
(d) 2x - 7 = 13

*Hint: Perform the inverse operation on both sides. Check by substituting back.*

**D3.** The merchant discovers his total zakat payment is 330 dinars. His zakat rate is 1/40. What is his total wealth?

*Hint: Let x = total wealth. Write x/40 = 330 and solve.*

---

### Hasan (Exam-level)

**H1.** Solve for x: [3 marks each]

(a) 5x + 3 = 2x + 18
(b) 4(x - 2) = 3(x + 1)
(c) (x + 5)/3 = 7

**H2.** The merchant has goods in three locations. The harbor warehouse holds twice the value of the market stall. The ship cargo is worth 5000 dinars more than the harbor warehouse. Together the three total 43,000 dinars. [5 marks]

(a) Let y = value in the market stall. Express the other two quantities in terms of y. [1 mark]
(b) Write an equation for the total and solve for y. [2 marks]
(c) Find the value at each location. [1 mark]
(d) Compute the merchant's total zakat at 1/40. [1 mark]

**H3.** An estate is divided among three heirs. The wife receives 1/8 of the estate. The son receives twice what the daughter receives. Together, the three shares exhaust the estate. The daughter receives 2625 dinars. What was the total estate? [4 marks]

*Hint: Let d = daughter's share. Son = 2d. Wife = x/8. Write x/8 + d + 2d = x.*

---

### Sahih (Proof and extension)

**S1.** Solve for x, expressing answers as fractions in lowest terms: [4 marks each]

(a) (2x + 1)/3 - (x - 4)/5 = 2

(b) 3(x - 1)/4 + 2 = (5x + 3)/6

**S2.** The inheritance problem, generalized. An estate x is divided among a wife (1/8), two daughters (2/3), a father (1/6), and a mother (1/6). 'Awl is applied. [12 marks]

(a) Show the common denominator of the four prescribed shares is 24. [2 marks]
(b) Show the sum of numerators over 24 is 27 and that 'awl is required. [2 marks]
(c) Write each heir's actual share as a fraction of x after 'awl. [3 marks]
(d) Verify the shares sum to x. [2 marks]
(e) If the wife's share after 'awl equals 3000 dinars, find x. [3 marks]

---

## ٦. Exam Technique

> **EXAM NOTE: Setting up equations from word problems**
>
> Mark schemes award method marks (M) for a correct equation and
> accuracy marks (A) for a correct solution. You CANNOT earn A marks
> without M marks. The equation is where the marks begin.
>
> **Step 1: Name the unknown.** Write "Let x = ..." Always state
> what x represents. Examiners need to read your working.
>
> **Step 2: Express other quantities in terms of x.**
> - "three more than his wealth" → x + 3
> - "a quarter of the estate" → x/4
> - "one-fortieth of his wealth" → x/40
> - "twice what the daughter receives" → 2d
>
> **Step 3: Find the equation.** Look for the word that means "=":
> "equals," "is," "remains," "totals," "gives." Write both sides.
>
> **Step 4: Solve. Show every line.** Do not skip steps. Each line
> is a potential method mark.
>
> **Step 5: Check.** Substitute into the ORIGINAL equation, not
> your rearranged version. A correct check can rescue a lost A mark
> if the examiner sees your method was sound.
>
> **Common error:** Solving correctly but answering a different
> question. "What was the estate?" and "What was the wife's share?"
> use the same equation but need different answers. Re-read the
> question after solving.
>
> **The word "of" means multiply:**
> - "1/8 of the estate" → x/8
> - "three-fifths of the remainder" → (3/5)(remainder)
>
> **When the answer is a fraction:** Do not convert to a decimal
> unless asked. If x = 27/7, report 27/7. Fractions are exact.
> Decimals lose marks when they lose precision.

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

**This island unlocks:** Quadratic Equations (0.7), where x appears squared. A patron will stand in his courtyard and say: "My garden is 10 by 10. I want the area to become 200." I will write (10 + x)² = 200, and when I expand it — x² + 20x + 100 = 200 — the x² will resist every tool from this island. Linear methods isolate x by undoing operations. But x², where the unknown multiplies itself, tangles the variable with itself. I will need a new method. Al-Khwarizmi's own method. Al-jabr.

**Connection forward to FP1:** The linear equation ax + b = 0 has exactly one solution (when a ≠ 0). The quadratic ax² + bx + c = 0 can have zero, one, or two. A polynomial of degree n can have up to n roots — this is the Fundamental Theorem of Algebra. The variable born in this island carries all the way there.

---

## ٨. Reflection

The merchant came with a rule and an absence. One-fortieth of his wealth — but his wealth was scattered across ships and warehouses and the promises of unreliable men. His numbers were incomplete. His obligation was not.

I named the unknown. Shay'. A thing. I wrote x where the number would go, and the equation held without it. The relationship between what he has and what he owes does not depend on the specific amount. It depends on the structure. The variable captures structure.

When his first ship docked, the equation updated. Known wealth grew from 13200 to 18000. The unknown shrank. He paid 450 dinars immediately — a lower bound, exact, not a guess. The variable let him act on partial knowledge. Obedience did not require omniscience. It required honesty about what he knew and a way to reason about what he didn't.

I used the same tool to generalize the inheritance. What I solved for 2700 dinars in Island 0.5, I now solve for any x. One computation serves every family the qadi will ever see. The specific case was the proof of concept. The general case is the tool.

The merchant left with his ledger under his arm. He will count his silk and weigh his spices. But he left knowing something he did not know when he arrived: that the unknown is not the enemy of computation. It is the beginning of it.

```
1 = 1
+-- 0.1 Equality: a thing is itself
+-- 0.2 Counting: one, then another
+-- 0.3 Multiplication: repeated addition
+-- 0.4 Zero and negatives: absence and debt
+-- 0.5 Fractions: the inheritance, 'awl
+-- 0.6 Variables: the unknown estate -- here
```

Six islands. I built tools for known numbers, and the merchant showed me the tools break when the number is absent. Not because they are wrong. Because they assumed something that is not always true: that the input exists.

Now the next problem is visible. The merchant's equation was linear — x to the first power, isolated in a single step. But a man is standing in his courtyard. He has a square garden, 10 cubits per side. He wants to add strips of equal width to two sides and double the area. I will write (10 + x)(10 + x) = 200. When I expand — x² + 20x = 100 — the unknown will be squared. Multiplied by itself. I will try to isolate it the way I isolated the merchant's x. It will not move. The tools from this island will fail at the garden wall.

I will need al-jabr itself.

> وَهُوَ الَّذِي أَنشَأَ جَنَّاتٍ مَّعْرُوشَاتٍ وَغَيْرَ مَعْرُوشَاتٍ
> "And He is the One who produced gardens, trellised and untrellised."
> *— Surah Al-An'am (6:141)*

*1 = 1 has not been lost.*

---
