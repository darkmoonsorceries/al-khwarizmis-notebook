# Island 0.9: Functions — The Muezzin's Rule

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> هُوَ الَّذِي جَعَلَ الشَّمْسَ ضِيَاءً وَالْقَمَرَ نُورًا وَقَدَّرَهُ مَنَازِلَ لِتَعْلَمُوا عَدَدَ السِّنِينَ وَالْحِسَابَ
> "It is He who made the sun a shining light and the moon a derived light
> and determined for it phases — that you may know the number of years
> and the account."
> *— Surah Yunus (10:5)*

**Connection grade: Hasan** — The verse is about divine design of
celestial bodies. Its primary meaning is theological: Allah set the
moon's phases so that people can reckon time. But the STRUCTURE —
"determined phases that you may know the number" — IS a function:
input (time) maps to output (phase). The verse does not name
functions. The function is in the verse's structure.

**The problem this ayah creates:** The moon has determined phases.
The sun has a determined arc. Prayer times depend on both. A man
who has watched the sky for forty years KNOWS when to call. A boy
who has watched for one year does not. The phases are determined —
meaning a rule exists. How do you write that rule so that anyone
who reads it arrives at the same answer?

---

## ٢. Al-Khwarizmi Discovers

Bilal climbs the minaret stairs slowly. His knees have the thick
calluses of a man who has prostrated five times a day for longer
than I have been alive. His hands grip the stone rail — weathered,
cracked at the knuckles, steady. He has climbed these stairs at
every prayer for forty years.

At the top, he turns east. The sun sits two fists above the
horizon. He looks at the shadow of the gnomon — the vertical stick
fixed to the minaret floor. The shadow stretches long across the
stone. Bilal watches it the way a reader watches a page.

Behind him, a boy. Yusuf. Eighteen years old, thin, earnest. A
scrap of parchment and a reed pen. He writes everything Bilal says.

---

"How will I know when it is Asr?" Yusuf asks.

Bilal points at the gnomon's shadow. "When the shadow equals the
post's height plus the shadow at noon."

Yusuf writes this down.

"And Maghrib?"

"When the sun disappears below the horizon."

"And Fajr?"

"When the first light appears on the eastern horizon. Not the false
dawn — the true dawn. The false dawn is a column. The true dawn is
a line that spreads."

Yusuf writes. Five rules now. He looks up. "And these work every
day?"

Bilal is quiet. Then: "No."

---

The problem is the seasons. In summer the sun climbs high and the
noon shadow is short. In winter it hangs low and the noon shadow is
long. The shadow at which Asr begins CHANGES — not because the rule
changes, but because the noon shadow changes.

Yusuf stares at his parchment. "So the Asr shadow depends on the
day of the year?"

Bilal nods.

"How do I know the noon shadow for each day?"

Bilal closes his eyes. He has watched this shadow for forty years.
He knows the noon shadow in Rajab is about half the post's height.
In Dhul Hijjah it is nearly the full height. In between it shifts
— gradually through some months, quickly through others. He KNOWS
this. It is in his bones, in the rhythm of four decades of climbing
and watching and calling.

He opens his eyes. "I cannot explain it all at once."

---

I have been sitting at the base of the minaret, working on the
builder's diagonal problem. But I hear Bilal's frustration and I
recognize it. He has knowledge that is real — tested against the
sky every day for forty years — and he cannot hand it to the boy.
Not because Yusuf is slow. Because the knowledge is trapped in a
form that requires a lifetime to absorb.

I climb the stairs.

"Bilal. Show me everything."

He does. Over the next hour he lays out every rule he has. I write
them as he speaks. For Fajr: the true dawn appears when the
whiteness spreads across the east. For Dhuhr: when the shadow
begins to lengthen past its shortest point. For Asr: the shadow
equals the post height plus the noon shadow. For Maghrib: the
moment the disc vanishes. For Isha: when the red glow is gone.

Each rule depends on the sun. The sun depends on the day. The day
determines the shadow. The shadow determines the prayer. And some
of these chain through three or four intermediate observations.

I stare at the notes. Both sides of the parchment. Dozens of rules.
Cross-references. Special cases. Corrections Bilal learned from his
teacher, who learned from his teacher.

The knowledge is real. Every rule has been verified against the sky.
But the FORM is chaos.

<!-- diagram: scattered-rules -->

> *Bilal's knowledge: dozens of rules, scattered across the page.
> Each one true. None of them organized.*

> *Margin note: The inheritance problem had one estate, one family,
> known numbers. This is different. Bilal needs a rule that works
> for ANY day, ANY location. The unknown is not a single number
> — it is a relationship.*

---

I try to organize. I write the Asr rule:

```
Shadow for Asr = post height + noon shadow
```

But the noon shadow depends on the day. So I need:

```
Noon shadow on day d = ???
```

And the Asr time depends on when the shadow reaches that length:

```
Asr time on day d = time when shadow = post height + noon shadow on day d
```

Each piece refers to another piece. I am writing RULES that take
INPUTS and produce OUTPUTS. The day goes in. A shadow length comes
out. The shadow length goes in. A prayer time comes out.

Each rule does one thing. Each rule is deterministic — the same
day always gives the same noon shadow. No ambiguity. No
contradiction.

I have been writing rules like this since the souk. The wife's
share: take the estate, divide by 8. The farmer's zakat: take the
harvest, multiply by 1/40. Every one of these was an input going
in and an output coming out.

But I never NAMED the pattern.

<!-- diagram: input-output -->

> *A box with one arrow entering from the left and one arrow
> leaving from the right. Input enters. Rule transforms. Output
> emerges.*

I need a name for a rule that takes an input and produces exactly
one output. I write:

```
f(d) = noon shadow length on day d
```

f is the rule. d is the input. f(d) is the output. Three things —
the rule, what goes in, what comes out — in a single expression.
The same day always gives the same shadow. A different day may
give a different shadow. But the RULE does not change.

I call this a **function**.

Bilal watches me write. He does not read mathematical notation. But
when I say, "f takes the day and gives you the noon shadow," he
nods. He has been DOING this function for forty years. He just
never wrote it down.

> *Margin note: I did not create the function. The sky has been
> running it since before Bilal was born. I am writing down what
> was already there.*

---

But the prayer times are not one function. They are a CHAIN. The
day determines the sun's altitude. The altitude determines the
shadow. The shadow determines the prayer time. Three rules, applied
in sequence. The output of one feeds the input of the next.

<!-- diagram: composition -->

> *Two boxes chained: the output arrow of the first enters the
> second. Day goes in the left. Prayer time comes out the right.*

For Yusuf, this changes everything. He does not need forty years of
watching. He needs the functions — written, precise, computable.
Give him the day, and he follows the chain to the prayer time. Not
by intuition. By computation.

I go back down the stairs. I have the form. Now I need the
formalism.

---

## ٣. The Derivation

### Definition

A **function** f from a set A to a set B is a rule that assigns
to each element x in A **exactly one** element f(x) in B.

```
f : A → B
x ↦ f(x)
```

<!-- diagram: formal-function-def -->

**f** is the function — the rule itself.
**A** is the **domain** — the set of all valid inputs.
**B** is the **codomain** — the set where outputs are permitted
to live.
**f(x)** is the **image** of x — the specific output for input x.
**Range** = { f(x) : x ∈ A } — the set of outputs that actually
occur.

The range sits inside the codomain but need not fill it.

<!-- diagram: domain-codomain -->

> *Two ovals. Left oval labeled A (domain), right oval labeled B
> (codomain). Arrows from each element in A reach exactly one
> element in B. Some elements in B have no arrow pointing to them.
> The elements that DO receive arrows form the range.*

### The Rule That Matters

The critical property: **each input produces exactly one output.**

If Bilal inputs "day 14 of Rajab" and gets two different Asr
times, the rule is not a function. A function does not contradict
itself. This is 1 = 1 at work — f(14) = f(14). Always.

Different inputs CAN produce the same output. Summer days near the
solstice give nearly identical noon shadows. That is permitted.
What is forbidden: one input giving two outputs.

### Function Notation

When I write f(x) = x/8, I am saying:

- **f** is the name of the rule.
- **x** is a placeholder for any valid input.
- **x/8** is what the rule does: divide the input by 8.

f(x) does NOT mean "f times x." It means "f applied to x."

To evaluate: replace x with the specific input.

```
f(x) = x/8
f(2400) = 2400/8 = 300
```

The wife receives 300 dinars from an estate of 2400.

### Domain and Range

The **domain** is every input for which the rule makes sense.
The **codomain** is the set of all possible outputs we allow.
The **range** is the set of outputs the function actually produces.

```
f : A → B

Domain A = set of valid inputs
Codomain B = set where outputs live
Range = { f(x) : x ∈ A } ⊆ B
```

**Domain restrictions from algebra.** When the function is a
formula, the domain is determined by what the formula permits:

- **Division by zero:** f(x) = 1/(x − 3) is defined for all x
  except x = 3.
- **Square roots of negatives:** f(x) = √(x − 5) is defined
  only for x ≥ 5.
- **Context:** If f(E) = E/8 is the wife's share, then E > 0.

### Types of Functions

<!-- diagram: formal-types -->

#### Injective (One-to-One)

A function f is **injective** if different inputs always produce
different outputs:

```
f(a) = f(b)  →  a = b
```

No two inputs share the same output.

**Example.** f(x) = 2x + 3. If f(a) = f(b), then 2a + 3 = 2b + 3.
Subtract 3: 2a = 2b. Divide by 2: a = b. Injective.

**Example.** g(x) = x². Then g(3) = 9 and g(−3) = 9. Two inputs,
same output. NOT injective.

**Bilal's test:** A spring day and an autumn day can produce
identical noon shadows — the sun reaches the same altitude on
both. The shadow function is not injective.

#### Surjective (Onto)

A function f : A → B is **surjective** if every element of B is
hit by some input:

```
For every y ∈ B, there exists x ∈ A such that f(x) = y.
```

Range equals codomain. Nothing in B is left unused.

**Example.** f : ℝ → ℝ, f(x) = 2x + 3. For any y ∈ ℝ, solve
2x + 3 = y: x = (y − 3)/2 ∈ ℝ. Every real number is hit.
Surjective.

**Example.** g : ℝ → ℝ, g(x) = x². The value −4 is never hit.
NOT surjective onto ℝ. But g : ℝ → [0, ∞) IS surjective — the
codomain matters.

#### Bijective (One-to-One and Onto)

A function that is both injective and surjective is **bijective**.
Every output is produced by exactly one input. A perfect pairing.

```
Bijective = Injective + Surjective
```

Bijections can be perfectly reversed.

### Composition of Functions

If I have two functions f and g, the **composite function**
f ∘ g is defined by:

```
(f ∘ g)(x) = f(g(x))
```

Apply g first, then f. Read right to left.

**Example.** Let g(x) = x + 3 and f(x) = 2x.

```
fg(x) = f(g(x)) = f(x + 3) = 2(x + 3) = 2x + 6
gf(x) = g(f(x)) = g(2x) = 2x + 3
```

fg(x) = 2x + 6. gf(x) = 2x + 3. **Different.**

**Composition is not commutative.** fg ≠ gf in general. Adding 3
then doubling is not the same as doubling then adding 3.

**For composition to work:** the range of g must sit inside the
domain of f. The output of the first function must be a valid
input for the second.

**Bilal's chain as composition:**

```
h(d) = sun's altitude at noon on day d       (day → angle)
s(α) = shadow length at angle α              (angle → shadow)
t(ℓ) = time when shadow reaches length ℓ     (shadow → time)

Prayer time = t(s(h(d))) = (t ∘ s ∘ h)(d)
```

Three functions composed. Day goes in. Prayer time comes out.

### Inverse Functions

If f is bijective, every output was produced by exactly one input.
The process can be reversed.

The **inverse function** f⁻¹ satisfies:

```
f⁻¹(f(x)) = x    for all x in the domain of f
f(f⁻¹(y)) = y    for all y in the range of f
```

**Example.** f(x) = 2x + 3. Solve for x: y = 2x + 3 →
x = (y − 3)/2. So f⁻¹(y) = (y − 3)/2.

Check: f(f⁻¹(y)) = f((y − 3)/2) = 2 × (y − 3)/2 + 3 =
(y − 3) + 3 = y. ✓

**Only bijections have inverses.** If f is not injective, two
inputs gave the same output — which input do I reverse to? If f
is not surjective, some outputs were never produced — there is
nothing to reverse from.

**f⁻¹ does NOT mean 1/f.** f⁻¹(x) is the inverse function.
1/f(x) is the reciprocal. Different operations entirely.

**The chain from 1 = 1:**

```
1 = 1 (reflexive, Island 0.1)
→ successor gives ℕ (Island 0.2)
→ multiplication on ℕ (Island 0.3)
→ additive inverse gives ℤ (Island 0.4)
→ multiplicative inverse gives ℚ (Island 0.5)
→ variables generalize to expressions (Island 0.6)
→ quadratic formula over ℝ (Islands 0.7–0.8)
→ function: f : A → B, each input exactly one output
→ types: injective, surjective, bijective
→ composition: (f ∘ g)(x) = f(g(x))
→ inverse: f⁻¹(f(x)) = x
```

**Geometry spec for Layer (Mode A):**
Subject: scattered dots (Bilal's unorganized rules). Verb: dots
sort into two columns, arrows draw from left to right — each left
dot hits exactly one right dot. Then a second box appears, arrows
chain through both boxes. Object: clean composition diagram, all
arrows resolved. End card: Functions — الدوال — Al-Biruni —
973–1048 CE — Khwarezm — 10:5.

---

## ٤. Al-Khwarizmi Solves

### Problem 1: Bilal's Shadow Rule

Bilal says: "At my latitude, near the equinox, the sun reaches
62 degrees at noon. The gnomon is 1 cubit tall."

He gives me a table from forty years of watching.

<!-- diagram: example-prayer-times -->

| Sun's noon altitude α | Noon shadow (cubits) |
|---|---|
| 30° | 1.73 |
| 45° | 1.00 |
| 60° | 0.58 |
| 75° | 0.27 |
| 90° | 0.00 |

The Asr shadow as a function of the noon shadow:

```
a(n) = 1 + n

Domain: n ≥ 0
Codomain: ℝ
Range: [1, ∞)
```

On a day when the noon altitude is 60°:

```
Noon shadow = 0.58 cubits
Asr shadow = a(0.58) = 1 + 0.58 = 1.58 cubits
```

Injective? If a(n₁) = a(n₂), then 1 + n₁ = 1 + n₂, so n₁ = n₂.
Yes.

Surjective onto [1, ∞)? For any y ≥ 1, set n = y − 1 ≥ 0. Then
a(n) = y. Yes.

Bijective on this codomain. Inverse exists:

```
a⁻¹(y) = y − 1
```

Yusuf can go both ways: noon shadow to Asr shadow, Asr shadow
back to noon shadow.

### Problem 2: Composition — Day to Asr Shadow

Bilal's approximation near the equinox (linear model):

```
n(d) = 1.2 − 0.01d    for d in [1, 90]
```

The noon shadow decreases as winter moves toward spring. Compose
with the Asr rule:

<!-- diagram: example-composition -->

```
(a ∘ n)(d) = a(n(d)) = 1 + (1.2 − 0.01d) = 2.2 − 0.01d
```

On day 30:

```
(a ∘ n)(30) = 2.2 − 0.01(30) = 2.2 − 0.3 = 1.9 cubits
```

On day 90:

```
(a ∘ n)(90) = 2.2 − 0.01(90) = 2.2 − 0.9 = 1.3 cubits
```

The Asr shadow is shorter in spring. Bilal confirms: "In spring,
Asr comes later — the shadow takes longer to reach its mark
because it starts shorter."

Two rules became one. Day goes in. Asr shadow comes out.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** Let f(x) = 3x + 7. Find f(0), f(1), f(−2), and f(10).
*(Hint: substitute each value for x and compute.)*

<!-- diagram: ex-daif-mapping -->

**2.** Bilal gives Yusuf the rule: "The Asr shadow equals the
gnomon height plus the noon shadow." The gnomon is 1.5 cubits.
The noon shadow on a certain day is 0.8 cubits.
(a) Write the Asr shadow as a function a(n) where n is the noon
shadow.
(b) Compute the Asr shadow for that day.
(c) State the domain of a, given that n ≥ 0.
*(Hint: the gnomon height replaces the "1" in the worked example.)*

**3.** Let g(x) = x² − 9. Find the roots of g — that is, solve
g(x) = 0.
*(Hint: factor as a difference of squares.)*

### Hasan (Exam-level)

**4.** Bilal's mosque receives an inheritance. The father's share
after 'awl is 4/27 of the estate. [5 marks]
(a) Write the father's share as a function f(E). State the
domain and range. [2 marks]
(b) Compute f(5400). [1 mark]
(c) For what estate value E does the father receive exactly
800 dinars? [1 mark]
(d) Write the inverse function f⁻¹(y). Verify that
f⁻¹(f(5400)) = 5400. [1 mark]

**5.** Bilal teaches Yusuf composition. He defines f(x) = 2x + 1
and g(x) = x² − 3. [6 marks]
(a) Find fg(x) and gf(x). [2 marks]
(b) Evaluate fg(2) and gf(2). [2 marks]
(c) Show that fg(x) = gf(x) has no real solutions. [2 marks]

<!-- diagram: ex-hasan-composition -->

**6.** Bilal records noon shadow lengths. He approximates the noon
shadow as n(d) = 1.5 − 0.012d cubits, where d is the number of
days from the winter solstice. The gnomon is 1 cubit. [5 marks]
(a) State the domain of n, given that noon shadows must be
non-negative. Find the largest valid d. [2 marks]
(b) The Asr shadow is a(n) = 1 + n. Write the composed function
(a ∘ n)(d). [1 mark]
(c) On what day does the Asr shadow equal 2 cubits? [2 marks]

### Sahih (Proof and extension)

**7.** Bilal defines f(x) = 2x + 5 and g(x) = (x − 5)/2.
[6 marks]
(a) Show that f(g(x)) = x and g(f(x)) = x. [2 marks]
(b) What does this tell you about the relationship between f
and g? [1 mark]
(c) Prove that if f is bijective, then the inverse function f⁻¹
exists and satisfies f⁻¹(f(x)) = x for all x in the domain
of f. [3 marks]

**8.** Yusuf models horizon brightness as f(t) = t² − kt + (k + 3),
where k depends on the season. [7 marks]
(a) Find the discriminant of f(t) = 0 in terms of k. [2 marks]
(b) Find the values of k for which the brightness touches zero
exactly once. [2 marks]
(c) For each such value of k, state when this occurs. [1 mark]
(d) For what values of k does the brightness never reach
zero? [2 marks]

---

## ٦. Exam Technique

```
┌─────────────────────────────────────────────────────────────┐
│                FUNCTIONS — WHAT MARKERS WANT                │
│                                                             │
│  1. NOTATION IS NOT OPTIONAL.                               │
│     f(x) = ... must appear before you simplify. Method      │
│     marks are awarded for f(a) = ..., not for the number.   │
│                                                             │
│  2. DOMAIN QUESTIONS — look for:                            │
│     • Division by zero → exclude where denominator = 0      │
│     • Square roots of negatives → exclude radicand < 0      │
│     • Context → estate positive, days non-negative, etc.    │
│     State the domain using set notation or inequalities.    │
│                                                             │
│  3. RANGE vs. CODOMAIN.                                     │
│     "State the range" = what outputs the function actually  │
│     produces. For f(x) = x², codomain may be ℝ but range   │
│     is [0, ∞). Do not confuse them.                         │
│                                                             │
│  4. COMPOSITION — APPLY INNER FIRST.                        │
│     fg(x) = f(g(x)). Apply g first, then f.                │
│     The most common error: applying f first.                │
│     Write it in steps:                                      │
│         fg(x) = f(g(x))                                    │
│               = f(x² − 3)                                  │
│               = 2(x² − 3) + 1                              │
│               = 2x² − 5                                    │
│                                                             │
│  5. INVERSE — SWAP AND SOLVE.                               │
│     Write y = f(x), solve for x. That is f⁻¹(y).          │
│     Always verify: f(f⁻¹(y)) = y. Only bijections have     │
│     inverses.                                               │
│                                                             │
│  Common mistake: writing fg(x) = f(x) × g(x). That is     │
│  the PRODUCT, not the COMPOSITION. fg(x) means f(g(x)).    │
└─────────────────────────────────────────────────────────────┘
```

---

## ٧. Log Pose

```
0.8 Irrationals ──→ [0.9 FUNCTIONS] ──→ 0.10 Limits
                          │
                          ├──→ 0.11 Derivatives (functions
                          │         to differentiate)
                          ├──→ Arc 1: Trig functions (the
                          │         moon's true curve)
                          ├──→ Arc 1: Exponential functions
                          │         (growth and decay)
                          └──→ Arc 2: Coordinate Geometry
                                    (functions as curves)
```

**This island unlocks:**
- **0.10: Limits** — the rule is written, but what happens as the
  input approaches a boundary it cannot reach?
- **0.11: Derivatives** — Yusuf needs the RATE: how fast is the
  light changing at dawn? That requires the derivative of a
  function.

**Dependencies satisfied:**
- ← 0.7 Quadratics (polynomial roots, discriminant)
- ← 0.8 Irrationals (ℝ as domain/codomain)
- ← 0.5 Fractions (inheritance shares as linear functions)
- ← 0.6 Variables (functions generalize what variables began)

**Introduced here for the first time:**
- Function notation: f(x), f : A → B
- Domain, codomain, range
- Injective, surjective, bijective
- Composition: f(g(x))
- Inverse functions

---

## ٨. Reflection

Bilal folds the page and places it inside his robe. The notation
is strange to him. But the meaning is not. Every rule I wrote, he
already knew. What he could not do was hand it to Yusuf in a form
Yusuf could carry.

A function is the bridge between knowing and transmitting. Bilal
watches the sky and knows. Yusuf reads the function and computes.
The knowledge passes not through years of watching but through a
rule written precisely enough that anyone who follows it arrives
at the same answer.

The Quran said: determined phases, that you may know the number
of years. The phases are determined — meaning the rule exists. The
knowledge of years is the output. Between the determined phases
and the knowledge stands computation. That computation is a
function.

Al-Biruni understood this. He sat in Khwarezm — a thousand
farsakhs from Baghdad — and computed the Earth's radius using a
mountain and the horizon. Input: the angle of depression from the
mountaintop. Output: the radius. One measurement. One function.
One answer: 6,339.9 km. The modern value is 6,371. He was off by
half a percent. In the eleventh century. With a mountain.

Bilal's knowledge is forty years compressed into ink. Yusuf will
carry it down the stairs, and when his own knees grow thick with
prostration, he will hand it to the next boy. The function does
not age. The function does not forget.

Tomorrow, Yusuf will climb the minaret alone for the first time.
He will carry the page. He will check the shadow against the
gnomon. And when the shadow reaches its mark, he will call.

But I do not yet have the space between the values. Bilal's shadow
does not jump from one length to the next — it sweeps
continuously. What happens between the entries in his table? What
does the shadow approach when the sun touches the horizon — a
boundary it meets for only an instant?

A traveler has arrived at the courtyard gate. Dusty cloak. Cracked
lips. An empty water-skin. He has been walking toward the city
walls for hours. Every hour, the distance halves. He is always
getting closer. He is never quite there.

He will need limits.

---

> وَقَدَّرَهُ مَنَازِلَ لِتَعْلَمُوا عَدَدَ السِّنِينَ وَالْحِسَابَ
> *"...determined for it phases, that you may know the number
> of years and the account."*

*1 = 1 has not been lost.*
