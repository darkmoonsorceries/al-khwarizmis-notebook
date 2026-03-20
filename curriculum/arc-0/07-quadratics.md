# Island 0.7: Quadratics --- The Patron's Garden

بسم الله الرحمن الرحيم

---

## ١. The Ayah

This island is different. In every previous island, I began with a verse. Here the problem comes from my own book --- *Kitab al-Jabr wa'l-Muqabala*. No verse prescribes quadratic equations.

The chain, honestly:

```
Quran (4:11-12) -> inheritance demands computation
  -> computation demands tools (0.1--0.6) -> tools become al-jabr
    -> the method generates new problems (this island)
```

**Connection grade: Honest** --- No verse poses this problem. The chain runs through human scholarship, not through text.

**The problem this generates:** A patron wants to expand his square garden by adding strips of equal width, doubling the area. The equation has the unknown *squared*. Linear tools break.

---

## ٢. Al-Khwarizmi Discovers

A patron stands in his courtyard. Silk-bordered robe, ink under his nails --- the kind of man who supervises his own builders. In the center: a square garden, green against pale stone.

"Ten cubits," he says. "Ten by ten. One hundred."

He walks to the east wall. "A strip along the east, a strip along the south, same width. The corner fills in naturally. I want two hundred --- double."

He turns back to me. "What width?"

---

Ten by ten. He adds strips of width *x* to east and south. The new garden: (10 + *x*) by (10 + *x*).

<!-- diagram: original-garden -->

> *A square garden. Ten cubits on each side. Area one hundred.*

```
(10 + x)^2 = 200
```

The distributive law (0.3):

```
(10 + x)(10 + x) = x^2 + 20x + 100
```

Subtract 100 from both sides (0.1):

```
x^2 + 20x = 100
```

I stare at this.

---

In Island 0.6, the merchant's equation was *x*/40 = 20. Multiply both sides. Done. Linear --- the unknown appears once.

Here it appears twice. *x* and *x*^2. Twenty lengths and one area --- different dimensions. I cannot collect them.

I try dividing by *x*:

```
x + 20 = 100/x
```

The *x* moved. Not isolated.

<!-- diagram: strips-added -->

> *Strips of width x attached to east and south. The garden grows. But the equation resists.*

I try subtracting 20*x*:

```
x^2 = 100 - 20x
```

Still there. Every operation pushes the unknown from one side to the other. It is tangled with itself.

The patron is waiting. I am stuck.

---

Then I look at the garden itself. Not the equation. The garden.

Strips are rectangles. The garden is a square. This is geometry, not symbols.

I kneel and draw in the dust. *x*^2 is a square. 20*x* is a rectangle --- but I split it. Two strips, each *x* by 10. One along the right edge. One along the bottom.

<!-- diagram: L-shape -->

> *The x^2 square. Two rectangles of 10x flanking it. An L-shaped gap pulses in the corner --- the figure is not complete.*

Total area so far: *x*^2 + 10*x* + 10*x* = *x*^2 + 20*x* = 100. The equation holds.

But the figure is not a square. There is a gap --- a missing corner, bottom-right. A square hole, 10 by 10.

---

If I fill that corner --- a 10 x 10 square, area 100 --- the entire figure becomes a perfect square with side (*x* + 10).

I add 100 to complete the figure. But I must add 100 to the right side too. The scales hold (0.1):

```
x^2 + 20x + 100 = 100 + 100
(x + 10)^2 = 200
```

<!-- diagram: completing -->

> *The corner filled. The figure is whole. A perfect square, side (x + 10), area 200.*

Al-jabr means restoration. In Island 0.5, I restored shares that exceeded the whole. Here I restore an incomplete figure to a perfect square. The same word. The same principle.

Now I have a perfect square on the left. Its area is 200. Its side is (*x* + 10).

```
x + 10 = sqrt(200)
```

200 = 100 x 2. So sqrt(200) = 10sqrt(2).

```
x = 10sqrt(2) - 10 = 10(sqrt(2) - 1)
```

sqrt(2) ~ 1.414. So *x* ~ 4.14. Verification: (14.14)^2 ~ 200. Yes.

---

I stand up and brush the dust from my hands.

"About four cubits and one-seventh," I tell the patron. "More precisely: ten times the square root of two, minus ten."

He frowns. "That is not a whole number."

"No."

"Not even a fraction?"

I pause. sqrt(2). I have been using this number without examining it. Is it a fraction? Is it *p*/*q* for some integers *p* and *q*?

I do not know. The answer bothers me. I set it aside. The patron has his measurement. His builders will manage.

But the number will come back.

---

The patron leaves. I stay in the courtyard, looking at the figure in the dust.

The method worked. I completed the square --- literally. Filled the missing piece, got a perfect square, extracted the side. Geometry solved what algebra could not.

But one garden is not enough. I need this for ANY equation of this kind.

Thabit ibn Qurra --- born in Harran, working in Baghdad --- reads Greek but thinks in shapes. I showed him the figure. He did not look at the equation. He said: "Your method works for any equation of this form. Let me prove it."

---

## ٣. The Derivation

### Completing the Square --- General Method

Every quadratic equation can be written:

```
ax^2 + bx + c = 0
```

where *a* != 0. If *a* were zero, this would be linear, and Island 0.6 handles it.

**Step 1. Make the leading coefficient 1.**

Divide everything by *a*:

```
x^2 + (b/a)x + c/a = 0
```

**Step 2. Move the constant to the right.**

```
x^2 + (b/a)x = -c/a
```

This is the shape I recognize. A square (*x*^2) plus a rectangle ((*b*/*a*)*x*).

<!-- diagram: formal-completing -->

> *The general completing-the-square figure. x^2 is the central square. The coefficient b/a splits into two strips of b/(2a). The missing corner is [b/(2a)]^2.*

**Step 3. Complete the square.**

Half the coefficient of *x*: *b*/(2*a*). Missing corner: [*b*/(2*a*)]^2 = *b*^2/(4*a*^2). Add to both sides:

```
(x + b/(2a))^2 = (b^2 - 4ac) / (4a^2)
```

**Step 4. Take the square root and isolate x.**

```
        -b +/- sqrt(b^2 - 4ac)
  x  = -------------------------
                 2a
```

<!-- diagram: formal-quadratic-formula -->

> *The quadratic formula. Every quadratic equation --- past, present, future --- is solved by this expression.*

**This is the quadratic formula.**

It is completing the square done once in full generality so it never needs to be done again.

**The chain from 1 = 1:**

```
1 = 1 (reflexive, 0.1)
  -> equality preserved under operations (0.1)
    -> distributive law: a(b + c) = ab + ac (0.3)
      -> additive inverse: a + (-a) = 0 (0.4)
        -> multiplicative inverse: a x (1/a) = 1 for a != 0 (0.5)
          -> variable substitution (0.6)
            -> completing the square -> quadratic formula
```

---

### The Discriminant

The expression under the square root governs everything. I name it:

```
D = b^2 - 4ac
```

The **discriminant**. It discriminates --- it tells me the nature of the roots before I compute them.

**Case 1: D > 0 --- Two distinct real roots.**

The square root of a positive number exists. The +/- gives two different values:

```
x_1 = (-b + sqrt(D)) / (2a)
x_2 = (-b - sqrt(D)) / (2a)
```

If D is a perfect square, the roots are rational. If not, the roots involve surds.

**Case 2: D = 0 --- One repeated root.**

The +/- adds nothing:

```
x = -b / (2a)
```

One root, counted twice.

**Case 3: D < 0 --- No real roots.**

The formula demands the square root of a negative number.

I stop.

No number I have built squares to a negative. The equation is honest. The number system is incomplete. The pattern repeats: 0.4 demanded negatives, 0.5 demanded fractions, and now D < 0 demands something that does not yet exist. The door opens in Arc 1.

---

## ٤. Al-Khwarizmi Solves

### Example 1: The Patron's Garden (completing the square)

<!-- diagram: example-garden-solved -->

> *x^2 + 20x = 100, completed geometrically. Half of 20 is 10. Corner: 100. Perfect square: (x + 10)^2 = 200.*

```
x^2 + 20x + 100 = 200
(x + 10)^2 = 200
x = -10 +/- 10sqrt(2)
```

Width cannot be negative: *x* = 10(sqrt(2) - 1) ~ 4.14 cubits. Check: (14.14)^2 ~ 200.

---

### Example 2: The Patron's Neighbour (quadratic formula)

The patron's neighbour has a square garden. Its area plus six of its sides equals 27. What is the side?

The equation: *x*^2 + 6*x* - 27 = 0. Here *a* = 1, *b* = 6, *c* = -27.

<!-- diagram: example-discriminant -->

> *The discriminant decides. D = 144 = 12^2. Two rational roots.*

The discriminant:

```
D = 6^2 - 4(1)(-27) = 36 + 108 = 144
```

Since 144 = 12^2:

```
x = (-6 +/- 12) / 2
```

Two solutions:

```
x_1 = (-6 + 12) / 2 = 3
x_2 = (-6 - 12) / 2 = -9
```

The side cannot be negative. So *x* = 3.

Verification: 3^2 + 6(3) = 9 + 18 = 27.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** The patron asks about a different expansion. He wants to add strips of width *x* to a 6 x 6 garden, producing a total area of 100. Set up and solve by completing the square.

*Hint: (6 + x)^2 = 100. Expand to x^2 + 12x = 64. Half of 12 is 6. Add 36 to both sides.*

<!-- diagram: ex-daif-complete -->

**2.** Solve by completing the square: *x*^2 + 8*x* = 20.

*Hint: Half of 8 is 4. Add 4^2 = 16 to both sides. What perfect square forms on the left?*

**3.** Compute the discriminant of *x*^2 - 4*x* + 4 = 0. How many roots? Solve it.

*Identify a = 1, b = -4, c = 4. Compute D = b^2 - 4ac.*

### Hasan (Exam-level)

**4.** The patron wants a rectangular extension. The length is 4 cubits more than the width. The total area must be 60 square cubits. Find the dimensions. [5 marks]

<!-- diagram: ex-hasan-formula -->

**5.** For what values of *k* does *x*^2 + *kx* + 9 = 0 have exactly one solution? [4 marks]

*Hint: D = 0 means k^2 - 36 = 0.*

**6.** Show that *x*^2 + 3*x* + 5 = 0 has no real roots. [3 marks]

### Sahih (Proof and extension)

**7.** Prove that for any quadratic *ax*^2 + *bx* + *c* = 0 with real roots *x*_1 and *x*_2: [6 marks]

(a) *x*_1 + *x*_2 = -*b*/*a*

(b) *x*_1 x *x*_2 = *c*/*a*

*Hint: Add the two roots from the formula. Multiply them.*

**8.** The patron returns. He adds strips of width *x* to all FOUR sides of his 10 x 10 garden, making it (10 + 2*x*) x (10 + 2*x*). He wants the area to triple --- 300 square cubits. [7 marks]

(a) Show the equation reduces to *x*^2 + 10*x* - 50 = 0.

(b) Solve in exact surd form.

(c) Explain why only one solution is physically valid.

---

## ٦. Exam Technique

**Complete the square** when the question says so, or when you need (*x* + *p*)^2 = *q* form. **Use the formula** when coefficients are messy or you only need roots. **Factor** when you can see integer roots in 10 seconds.

| D | Nature of roots |
|---|----------------|
| D > 0, perfect square | Two distinct rational roots |
| D > 0, not perfect square | Two distinct irrational roots (surds) |
| D = 0 | One repeated root |
| D < 0 | No real roots |

**Exam pattern:** "Show no real roots" = compute D < 0. "Find *k* for which..." = set D = 0 or D > 0 or D < 0 and solve for *k*.

**Common errors:** (1) Sign error in -*b*: if *b* = -5, then -*b* = +5. Write it out. (2) Dividing only PART of the numerator by 2*a*. (3) Wrong sign in D when *c* is negative --- the double negative hides errors.

---

## ٧. Log Pose

```
                    +----------+
                    | Prologue |
                    | 1 = 1    |
                    +----+-----+
                         |
                    +----v-----+
              +-----| 0.1 === |-----+
              |     | Equality |     |
              |     +----+-----+     |
              |          |           |
         +----v---+ +---v----+ +---v----+
         |  0.2   | |  0.3   | |  0.4   |
         | Count  | | Mult   | | Zero/- |
         +----+---+ +---+----+ +---+----+
              |          |         |
              +-----+----+----+----+
                    |         |
              +-----v---+ +--v-----+
              |  0.5    | |  0.6   |
              | Frac    | |  Vars  |
              +-----+---+ +--+-----+
                    |         |
                    +----+----+
                         |
                    +----v-----+
              +-----| 0.7 === |
              |     | Quadr   |
              |     +----------+
              |
         +----v---+
         |  0.8   |
         | Irrat  |
         +--------+
```

**This island unlocks:**
- 0.8 (Irrationals) --- sqrt(2) appeared and it is not a fraction
- Arc 1 (Complex Numbers) --- D < 0 demands sqrt(-1)
- The pattern: equation honest, system incomplete -> EXTEND

---

## ٨. Reflection

The patron came with one question. The answer: 10(sqrt(2) - 1) ~ 4.14 cubits. His builders will mark it out tomorrow.

But one garden became a formula for every garden. Al-jabr is restoration --- in 0.5, 'awl restored overflowing shares; here, completing the square restores an incomplete figure to wholeness. The name of my book is not a metaphor.

The discriminant speaks before I solve. D > 0: two answers. D = 0: one. D < 0: none in any number I possess. The formula does not fail. The system is not yet large enough.

But the patron's answer contained sqrt(2). I used it. I never asked: what IS it?

A builder arrives at the courtyard. Calloused hands, a measuring cord over his shoulder. He needs the diagonal of a square courtyard --- one cubit per side.

"Seven-fifths squared is forty-nine twenty-fifths," he says. "That is 1.96. Not 2."

No fraction works. The cord has a definite length. He can hold it. But he cannot write it.

The builder is waiting. I will need a new island.

*1 = 1 has not been lost.*

---
