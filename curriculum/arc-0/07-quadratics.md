# Island 0.7: Quadratics — The Patron's Garden

بسم الله الرحمن الرحيم

---

## ١. The Ayah

This island is different from every island before it.

In every previous island, I began with a verse. The Quran posed the problem; I built the tool. Here, the problem comes from my own book — *Kitab al-Jabr wa'l-Muqabala*. No verse prescribes quadratic equations.

But let me trace the chain honestly:

```
Quran (4:11-12)
  → inheritance demands computation
    → computation demands tools (Islands 0.1-0.6)
      → tools become a METHOD (al-jabr)
        → the method generates new problems (this island)
```

The Quran posed the inheritance problem. The inheritance problem demanded every tool I have built. The tools became a discipline. The discipline now poses its own questions. Human scholarship on divine foundation.

**Connection grade: HONEST** — Al-Khwarizmi's *al-jabr* traces back to the inheritance computation needs of Surah An-Nisa (4:11-12). No verse poses quadratic equations. The chain runs through human minds, not through text. Every link is real. Every link is acknowledged.

**The problem this generates:** A patron wants to expand his square garden by adding strips of equal width, doubling the area. The equation that results has the unknown *squared*. The linear tools from Island 0.6 do not work.

---

## ٢. Al-Khwarizmi Thinks

A patron stands in his courtyard.

He is not poor. The robe says that — silk borders, carefully maintained. His hands say something else — ink under the nails, the kind of man who supervises his own builders. The courtyard is paved. In the center: a square garden, green against the pale stone.

"Ten cubits," he says, pointing to the garden's edge. "Ten by ten. Area of one hundred."

He walks to the east wall. "I want to expand. A strip along the east side, and a strip along the south side, both the same width. The corner where they meet fills in naturally. I want the new area to be two hundred — double what I have."

He turns back to me. "What width should the strips be?"

I can see the garden. Ten by ten. He adds a strip of width *x* to the east and to the south. The new garden becomes (10 + *x*) by (10 + *x*) — still a square, but larger.

I write:

```
(10 + x)² = 200
```

I expand. The distributive law from Island 0.3:

```
(10 + x)(10 + x) = 10 × 10 + 10 × x + x × 10 + x × x
                  = 100 + 10x + 10x + x²
                  = x² + 20x + 100
```

So:

```
x² + 20x + 100 = 200
```

Subtract 100 from both sides. What I do to the left, I do to the right (0.1):

```
x² + 20x = 100
```

I stare at this.

---

In Island 0.6, I solved the merchant's problem. His equation was *x*/40 = 20. Multiply both sides by 40. Done. Linear — the unknown appears once, to the first power, and I isolate it in one step.

Here the unknown appears twice. Once as *x*, multiplied by 20. Once as *x*², multiplied by itself. I cannot collect them. *x* and *x*² are not the same kind of thing. Twenty lengths of a side and one area of a square — they have different dimensions. I cannot add them the way I add like terms.

I try anyway. Divide both sides by *x*:

```
x + 20 = 100/x
```

The *x* is still there. On the right side now, in the denominator. I have not isolated it. I have moved it.

I try differently. Subtract 20*x* from both sides:

```
x² = 100 - 20x
```

The *x* is still on the right. I cannot get a number on the right and *x* alone on the left. Every operation I try pushes the unknown from one side to the other, or changes its form, but never pins it down. It is tangled with itself.

> *Margin note: The inheritance problem (0.5) needed only linear operations — multiply shares by estate, add, compare to the whole. The merchant's equation (0.6) was linear. This is the first problem that demands more. The tools I built for the family are necessary but not sufficient.*

The patron is waiting. He does not see my difficulty. He sees a mathematician thinking.

I am not thinking. I am stuck.

---

Then I look at the garden itself.

Not the equation. The garden. The physical square in the courtyard, ten cubits on each side. The patron wants to add strips. Strips are rectangles. The garden is a square. He wants a larger square. This is geometry, not just symbols.

I kneel and draw in the dust of the courtyard floor.

The original garden: a square, side 10, area 100. He wants the total to be 200. The extra area is 100. That extra area — the 100 that must be added — comes from the strips and the corner.

But let me think about this differently. Forget the 10 for a moment. I have:

```
x² + 20x = 100
```

The *x*² is a square. Side *x*, area *x*². I can draw that.

```
       x
  +---------+
  |         |
x |   x²    |
  |         |
  +---------+
```

The 20*x* is a rectangle. Width *x*, length 20. But I do not want one long lopsided rectangle hanging off my square. I split it. Two equal pieces: each is *x* by 10.

I place one along the right edge. One along the bottom edge.

```
       x         10
  +---------+---------+
  |         |         |
x |   x²    |  10x   |
  |         |         |
  +---------+---------+
  |         |
10|  10x    |
  |         |
  +---------+
```

Total area so far: *x*² + 10*x* + 10*x* = *x*² + 20*x* = 100. The equation holds.

But the figure is not a square. There is a gap — a missing corner, bottom-right. A square hole, 10 by 10.

```
       x         10
  +---------+---------+
  |         |         |
x |   x²    |  10x   |
  |         |         |
  +---------+---------+
  |         |         |
10|  10x    |  100    |
  |         | (empty) |
  +---------+---------+
```

If I fill that corner — a 10 × 10 square, area 100 — the entire figure becomes a perfect square with side (*x* + 10).

I add 100 to complete the figure. But I must add 100 to the right side of the equation too. The scales hold (0.1):

```
x² + 20x + 100 = 100 + 100
(x + 10)² = 200
```

> *Margin note: Al-jabr means restoration. In Island 0.5, I restored shares that exceeded the whole. Here I restore an incomplete figure to a perfect square. The same word. The same principle. This is what my book is about.*

Now I have a perfect square on the left. Its area is 200. Its side is (*x* + 10).

```
x + 10 = √200
```

What is √200? I simplify. 200 = 100 × 2. So √200 = √100 × √2 = 10√2.

```
x + 10 = 10√2
x = 10√2 - 10
x = 10(√2 - 1)
```

I approximate. √2 is roughly 1.414 — I know this from measuring diagonals. So:

```
x ≈ 10(1.414 - 1) = 10(0.414) = 4.14
```

The strips should be about 4.14 cubits wide.

Verification: (10 + 4.14)² = (14.14)² ≈ 200. Yes.

---

I stand up and brush the dust from my hands.

"About four cubits and one-seventh," I tell the patron. "More precisely: ten times the square root of two, minus ten."

He frowns. "That is not a whole number."

"No."

"Not even a fraction?"

I pause. √2. I have been using this number without examining it. Is it a fraction? Is it *p*/*q* for some integers *p* and *q*?

I do not know. The answer bothers me in a way I cannot yet articulate. I set it aside. The patron has his measurement. He can mark 4 cubits and a little more. His builders will manage.

But the number will come back. Numbers that are not fractions — I have not met them yet. That is another island.

---

The patron leaves to find his builders. I stay in the courtyard, looking at the figure in the dust.

The method worked. I completed the square — literally. I took an incomplete figure, filled the missing piece, and got a perfect square whose side I could extract. The geometry solved what the algebra could not.

But the patron's garden was one problem. I need the method for *any* problem of this kind. What if the equation were *x*² + 6*x* = 27? Or 2*x*² + 8*x* = 10? Or *ax*² + *bx* + *c* = 0, with letters I have never seen before?

The dust is still there. I kneel again and begin to generalize.

---

## ٣. The Derivation

### Completing the Square — General Method

Every quadratic equation can be written:

```
ax² + bx + c = 0
```

where *a* ≠ 0. If *a* were zero, this would be linear, and Island 0.6 handles it.

I want to do to this equation what I did to the patron's garden: turn the left side into a perfect square.

**Step 1. Make the leading coefficient 1.**

Divide everything by *a*:

```
x² + (b/a)x + c/a = 0
```

**Step 2. Move the constant to the right.**

Subtract *c*/*a* from both sides:

```
x² + (b/a)x = -c/a
```

This is the shape I recognize. A square (*x*²) plus a rectangle ((*b*/*a*)*x*). The same shape as the patron's garden.

**Step 3. Complete the square.**

The coefficient of *x* is *b*/*a*. I split it in half: *b*/(2*a*). This is the width of each strip, just as I split 20 into two strips of 10 for the patron.

The missing corner is a square with side *b*/(2*a*). Its area is *b*²/(4*a*²).

Add this to both sides:

```
x² + (b/a)x + b²/(4a²) = -c/a + b²/(4a²)
```

The left side is now a perfect square:

```
(x + b/(2a))² = -c/a + b²/(4a²)
```

**Step 4. Simplify the right side.**

Common denominator 4*a*²:

```
(x + b/(2a))² = (b² - 4ac) / (4a²)
```

**Step 5. Take the square root.**

```
x + b/(2a) = ± √(b² - 4ac) / (2a)
```

The ± is honest. Both (+8)² and (−8)² give 64. A square root has two possibilities. For the patron's garden I discarded the negative one because a garden's width cannot be negative. In general, both are valid.

**Step 6. Isolate *x*.**

```
x = -b/(2a) ± √(b² - 4ac) / (2a)
```

As a single fraction:

```
        -b ± √(b² - 4ac)
  x  = -------------------
              2a
```

**This is the quadratic formula.**

Every quadratic equation — past, present, future — is solved by this expression. It is completing the square done once in full generality so it never needs to be done again.

> *Margin note: Count the tools. Equality preserved under operations (0.1). Distributive law to expand (x + b/(2a))² (0.3). Zero and negatives for the ± and for moving terms (0.4). Fractions for dividing by a and finding common denominators (0.5). Variables for a, b, c themselves — unknowns standing for any coefficients (0.6). Every island contributed to this formula.*

**The chain from 1 = 1:**

```
1 = 1 (reflexive, 0.1)
  → equality preserved under operations (0.1)
    → distributive law: a(b + c) = ab + ac (0.3)
      → additive inverse: a + (-a) = 0 (0.4)
        → multiplicative inverse: a × (1/a) = 1 for a ≠ 0 (0.5)
          → variable substitution (0.6)
            → completing the square → quadratic formula
```

---

### The Discriminant

The expression under the square root governs everything. I name it:

```
Δ = b² - 4ac
```

The **discriminant**. It discriminates — it tells me the *nature* of the roots before I compute them.

**Case 1: Δ > 0 — Two distinct real roots.**

The square root of a positive number exists. The ± gives two different values:

```
x₁ = (-b + √Δ) / (2a)
x₂ = (-b - √Δ) / (2a)
```

If Δ is a perfect square (like 256 = 16²), the roots are rational. If Δ is not a perfect square (like 200), the roots involve surds.

**Case 2: Δ = 0 — One repeated root.**

The square root of zero is zero. The ± adds nothing:

```
x = -b / (2a)
```

The equation has one root, counted twice. The perfect square touches zero at exactly one point.

**Case 3: Δ < 0 — No real roots.**

The formula demands the square root of a negative number.

I stop.

No number I have built — natural, integer, rational, or even the irrational numbers I sense but have not yet named — squares to a negative. The equation *x*² + 1 = 0 is well-formed. Nothing is wrong with it. But its solution requires √(−1), which exists in no system I have constructed.

The pattern is familiar. In Island 0.4, subtraction demanded numbers below zero — so I extended to the integers. In Island 0.5, division demanded numbers between integers — so I extended to the rationals. Each time: the equation was honest, the number system was incomplete, and al-jabr demanded extension.

Δ < 0 is that demand again. I note its existence. The door opens in Arc 1. Not today.

> *The quadratic formula does not break when Δ < 0. The formula is perfect. The number system is not yet large enough.*

---

## ٤. Al-Khwarizmi Solves

### Example 1: The Patron's Garden (completing the square)

The patron's equation:

```
x² + 20x = 100
```

Half of 20 is 10. The missing corner: 10² = 100. Add to both sides:

```
x² + 20x + 100 = 200
(x + 10)² = 200
x + 10 = ±√200 = ±10√2
```

Two solutions:

```
x = -10 + 10√2 ≈ 4.14
x = -10 - 10√2 ≈ -24.14
```

A garden's width cannot be negative. So *x* = 10(√2 − 1) ≈ 4.14 cubits.

**Verification:** (10 + 4.14)² = (14.14)² ≈ 199.94 ≈ 200. ✓

The patron marks 4 cubits and about one-seventh more. His builders begin.

---

### Example 2: The Patron's Neighbour (quadratic formula, integer roots)

The patron's neighbour has a square garden. Its area plus six of its sides equals 27. What is the side?

The equation: *x*² + 6*x* − 27 = 0. Here *a* = 1, *b* = 6, *c* = −27.

The discriminant:

```
Δ = 6² - 4(1)(-27) = 36 + 108 = 144
```

Since 144 = 12²:

```
x = (-6 ± 12) / 2
```

Two solutions:

```
x₁ = (-6 + 12) / 2 = 6/2 = 3
x₂ = (-6 - 12) / 2 = -18/2 = -9
```

The side cannot be negative. So *x* = 3.

**Verification:** 3² + 6(3) = 9 + 18 = 27. ✓

---

### Example 3: A Storehouse Problem (two valid solutions)

A merchant builds a rectangular storehouse against an existing wall. He has 24 cubits of fencing for the remaining three sides. He needs 70 square cubits of floor space.

Let the width perpendicular to the wall be *x*. Then:

```
Two widths + one length = 24
Length = 24 - 2x

Area = x(24 - 2x) = 70
24x - 2x² = 70
2x² - 24x + 70 = 0
x² - 12x + 35 = 0
```

Here *a* = 1, *b* = −12, *c* = 35.

```
Δ = (-12)² - 4(1)(35) = 144 - 140 = 4
√Δ = 2
```

```
x = (12 ± 2) / 2
```

```
x₁ = 14/2 = 7     →  length = 24 - 14 = 10
x₂ = 10/2 = 5     →  length = 24 - 10 = 14
```

Check: 7 × 10 = 70. ✓ And 5 × 14 = 70. ✓

Both work. The algebra gives the merchant two options. He chooses the shape that fits his lot. The equation does not decide for him — it shows him what is possible.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** The patron asks about a different expansion. He wants to add strips of width *x* to the east and south of a 6 × 6 garden, producing a total area of 100. Set up and solve the equation.

*Hint: (6 + x)² = 100. Expand, simplify to x² + 12x = 64. Half of 12 is 6. Add 6² = 36 to both sides.*

**2.** Solve by completing the square: *x*² + 8*x* = 20.

*Hint: half of 8 is 4. Add 4² = 16 to both sides. What perfect square do you get on the left?*

**3.** Compute the discriminant of *x*² − 4*x* + 4 = 0. How many roots does this equation have? Solve it.

*Identify a = 1, b = −4, c = 4. Compute Δ = b² − 4ac.*

---

### Hasan (Exam-level)

**4.** The patron wants a *rectangular* extension to his garden. The length is 4 cubits more than the width. The total area must be 60 square cubits. Find the dimensions. [5 marks]

**5.** The patron's builder encloses a rectangular courtyard using three walls (the fourth side is the patron's existing house). He has 30 cubits of wall material and needs an enclosed area of 112 square cubits. Find the possible dimensions. [5 marks]

**6.** The patron asks Al-Khwarizmi: "For what values of *k* would *x*² + *kx* + 9 = 0 have exactly one solution — a perfect square touching the ground once?" Find the values of *k*. [4 marks]

*Hint: Δ = 0 means k² − 36 = 0.*

**7.** The patron's second plot requires solving 2*x*² + 12*x* + 7 = 0. Complete the square to find the dimensions in surd form. [5 marks]

**8.** The patron proposes a garden where *x*² + 3*x* + 5 = 0 would give the boundary. Show that this equation has no real roots — the garden cannot exist. [3 marks]

---

### Sahih (Proof and extension)

**9.** Prove that for any quadratic *ax*² + *bx* + *c* = 0 with real roots *x*₁ and *x*₂: [6 marks]

(a) *x*₁ + *x*₂ = −*b*/*a*

(b) *x*₁ × *x*₂ = *c*/*a*

*Hint: use the two roots from the quadratic formula directly. Add them. Multiply them.*

**10.** The patron returns. He now wants to add strips of width *x* to all *four* sides of his original 10 × 10 garden, making the new garden (10 + 2*x*) × (10 + 2*x*). He wants the area to triple — reaching 300 square cubits. [7 marks]

(a) Show that the equation reduces to 4*x*² + 40*x* − 200 = 0, or equivalently *x*² + 10*x* − 50 = 0.

(b) Solve for *x* in exact surd form.

(c) Explain why only one of the two solutions is physically valid.

**11.** The patron's architect submits designs where the constraint equation is 2*x*² − 3*x* + *p* = 0, with *p* depending on the site. Find the range of values of *p* for which two distinct layouts are possible. [5 marks]

**12.** Starting from *x*² + 20*x* = 100 (the patron's original problem), complete the square *geometrically*. Draw the square, the two strips, and the missing corner. Label every area. Show that filling the corner gives (*x* + 10)² = 200. This is how al-Khwarizmi solved quadratics in *Kitab al-Jabr wa'l-Muqabala*. Reproduce his method. [6 marks]

---

## ٦. Exam Technique

### Completing the Square vs. the Quadratic Formula

Both solve any quadratic. The formula IS completing the square, done once in general. On an exam, the choice matters.

**Use completing the square when:**
- The question says "by completing the square"
- You need (*x* + *p*)² = *q* form (e.g., finding a parabola's vertex)
- *a* = 1 and *b* is even — clean arithmetic
- You want to show reasoning, not just produce roots

**Use the quadratic formula when:**
- Coefficients are messy (fractions, large numbers)
- You only need roots, not the squared form
- You need the nature of the roots via Δ without fully solving
- Time is short

**Use factoring when:**
- The roots are obviously integers. Check: does *c* factor into two numbers that sum to *b*?
- A common factor is visible: 2*x*² − 8*x* = 0 has 2*x* factored out immediately
- You can see it in under 10 seconds. If not, use the formula.

### Reading the Discriminant

Δ = *b*² − 4*ac* tells you the nature of the roots WITHOUT solving.

| Δ | Nature of roots |
|---|----------------|
| Δ > 0, perfect square | Two distinct rational roots |
| Δ > 0, not perfect square | Two distinct irrational roots (surds) |
| Δ = 0 | One repeated root |
| Δ < 0 | No real roots |

**Exam pattern:** "Show that the equation has no real roots" = show Δ < 0. Compute it, show it is negative, state the conclusion. Three lines, full marks.

**Exam pattern:** "Find the values of *k* for which..." = the discriminant involves *k*. Set Δ = 0 (repeated roots), Δ > 0 (two distinct roots), or Δ < 0 (no real roots). Solve the resulting equation or inequality for *k*.

### Common Errors

**1. Sign error in −*b*.** If *b* = −5, then −*b* = +5. Write out the substitution. Do not compute in your head.

**2. Dividing only part of the numerator by 2*a*.** The ENTIRE expression −*b* ± √Δ is divided by 2*a*. Not just the square root. Not just −*b*.

**3. Wrong sign in Δ.** Δ = *b*² − 4*ac*, not *b*² + 4*ac*. When *c* is negative: −4*a*(*c*) becomes positive. The double negative is where errors hide.

**4. "One repeated root" does not mean "one root."** The equation *has* two roots that happen to be equal. (*x* − 5)² = 0 gives *x* = 5 with multiplicity two. This distinction matters in later work.

**5. Forgetting to check physical context.** The formula may give *x* = 3 and *x* = −13. If *x* is a length, discard the negative. Always return to the problem's meaning.

---

## ٧. Log Pose

```
ISLAND 0.7 — QUADRATICS
========================

    Unlocked:
    +-- Completing the square (geometric, then algebraic)
    +-- The quadratic formula
    +-- The discriminant: Δ = b² - 4ac
    +-- Classification of roots by Δ

    Callbacks:
    +-- 0.1 — Equality: add the same to both sides (completing the square)
    +-- 0.3 — Distributive law: expanding (x + p)² requires it
    +-- 0.4 — Negatives: the ± sign, and Δ < 0
    +-- 0.5 — Al-jabr as restoration: from 'awl to completing the square
    +-- 0.6 — Variables: a, b, c are unknowns themselves

    Forward:
    +-- 0.8 — Irrationals: √2 appeared and it is not a fraction
    +-- Arc 1 — Complex Numbers: Δ < 0 demands √(-1)
    +-- The pattern: equation honest, system incomplete → EXTEND

    The chain so far:
    1 = 1
    +-- Equality (the scale)
    +-- Counting (the shepherd)
    +-- Multiplication (the grain)
    +-- Zero and negatives (the debt)
    +-- Fractions (the inheritance)
    +-- Variables (the unknown estate)
    +-- Quadratics (the garden)     <-- YOU ARE HERE
```

---

## ٨. Reflection

The patron came with one question. How wide must the strips be?

The answer: 10(√2 − 1). About 4.14 cubits. His builders will mark it out tomorrow. The garden doubles.

But the method I found works for any equation where the unknown is squared. The patron had one garden. I have a tool for every garden, every storehouse, every problem that bends the unknown back on itself. He came with one question. I leave with a formula that answers all questions of its kind.

Al-jabr is restoration. In Island 0.5, the shares exceeded the whole — 27/24 > 1 — and 'awl restored them proportionally. Here, *x*² + 20*x* = 100 was an incomplete figure, and completing the square restored it to wholeness. Different problems. Same principle. The name of my book is not a metaphor. It is what I do.

And the discriminant — it speaks before I solve. Δ > 0: two answers. Δ = 0: one answer, doubled. Δ < 0: no answer in any number I possess. The formula does not fail. The system is not yet large enough. The pattern repeats: subtraction demanded negatives, division demanded fractions, and now the discriminant demands something I cannot yet name. Al-jabr will restore it. Not today.

But there is a more immediate question. The patron's answer contained √2. I used it. I approximated it. I never asked: what IS it?

Is it a fraction? Can I write it as *p*/*q* for integers *p* and *q*? I assumed I could approximate it — 1.414, close enough for builders. But is there an exact fraction?

A builder arrives at the courtyard. Calloused hands, chalk dust on his sleeves, a measuring cord looped over his shoulder. He is laying tiles for a square courtyard — one cubit per side — and he needs the length of the diagonal.

"I measured it," he says. "About one and two-fifths. But when I check — seven-fifths squared is forty-nine twenty-fifths. That is 1.96. Not 2."

He has tried other fractions. None of them square to exactly 2. The cord has a definite length. He can hold it in his hands. But he cannot write it.

I recognize the shape of the problem. The number exists — the diagonal is real, physical, measurable. The number system has a hole where this measurement should live. The tools are not wrong. Creation is richer than my categories.

The Quran says: *"Do they not look at how it is created?"* (88:17). I looked. I found something my numbers cannot hold.

The builder is waiting. I will need a new island.

---

*1 = 1 has not been lost.*

---