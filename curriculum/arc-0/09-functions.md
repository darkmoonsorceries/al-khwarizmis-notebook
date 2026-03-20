# Island 0.9: Functions — The Muezzin's Rule

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> أَقِمِ الصَّلَاةَ لِدُلُوكِ الشَّمْسِ إِلَىٰ غَسَقِ اللَّيْلِ وَقُرْآنَ الْفَجْرِ ۖ إِنَّ قُرْآنَ الْفَجْرِ كَانَ مَشْهُودًا
>
> "Establish prayer at the decline of the sun until the darkness of the night and the Quran of dawn. Indeed, the recitation of dawn is witnessed."
> *— Surah Al-Isra (17:78)*

**Connection grade: HONEST CHAIN** — The Quran commands prayer at specific times: the sun's decline, the darkness of night, the dawn. Obeying this command requires knowing WHEN — and "when" depends on the sun's position, which depends on the day of the year, which depends on the latitude. The chain: verse commands prayer at specific times (17:78, 11:114) → determining those times requires observing sun and shadow → observations must be encoded as repeatable rules mapping inputs to outputs → functions.

**The problem this ayah creates:** The verse commands prayer at the sun's decline, at the darkness of night, at dawn. Five prayers, each triggered by a celestial event. A man who has watched the sky for forty years can obey. A boy who has watched for one year cannot. How do you write a rule that turns what the old man KNOWS into what the young man can COMPUTE?

---

## ٢. Al-Khwarizmi Thinks

Bilal climbs the minaret stairs slowly. His knees have the thick calluses of a man who has prostrated five times a day for longer than I have been alive. His hands grip the stone rail — weathered, cracked at the knuckles, steady. He has climbed these stairs at every prayer for forty years. His body knows the count before his mind does.

At the top, he turns east. The sun sits two fists above the horizon. He looks at the shadow of the post — the gnomon, the vertical stick fixed to the minaret floor. The shadow stretches long across the stone. Bilal watches it the way a reader watches a page. He is reading the sky.

Behind him, a boy. Yusuf. Eighteen years old, thin, earnest. He has a scrap of parchment and a reed pen. He writes everything Bilal says.

"How will I know when it is Asr?" Yusuf asks.

Bilal points at the gnomon's shadow. "When the shadow is equal to the post's height plus the shadow at noon, it is Asr."

Yusuf writes this down.

"And Maghrib?"

"When the sun disappears below the horizon."

"And Isha?"

"When the red glow is gone from the west."

"And Fajr?"

"When the first light appears on the eastern horizon. Not the false dawn — the true dawn. The false dawn is a column of light. The true dawn is a line that spreads."

Yusuf writes. He has five rules now. He looks up. "And these work every day?"

Bilal is quiet. Then: "No."

> *Margin note: "li-duluki al-shams" — at the decline of the sun. The Arabic duluk means both the sun's zenith and its setting. The ambiguity is resolved by observation, not by grammar. Observation requires a rule.*

The problem is the seasons. In summer, the sun climbs high and the noon shadow is short. In winter, it hangs low and the noon shadow is long. The shadow at which Asr begins CHANGES — not because the rule changes, but because the noon shadow changes. Bilal's rule said "the post's height PLUS the shadow at noon." The post's height is fixed. The noon shadow is not.

Yusuf stares at his parchment. "So the Asr shadow depends on the day of the year?"

Bilal nods.

"How do I know the noon shadow for each day?"

Bilal closes his eyes. He has watched this shadow for forty years. He knows the noon shadow in Rajab is about half the post's height. In Dhul Hijjah it is nearly the post's full height. In between, it shifts — gradually through some months, quickly through others. He KNOWS this. It is in his bones, in the rhythm of four decades of climbing and watching and calling.

He opens his eyes. "I cannot explain it all at once."

I have been sitting at the base of the minaret, working on the builder's diagonal problem from yesterday. But I hear Bilal's frustration and I recognize it. He has knowledge that is real — tested against the sky every day for forty years — and he cannot hand it to the boy. Not because Yusuf is slow. Because the knowledge is trapped in a form that requires a lifetime to absorb.

I climb the stairs.

"Bilal," I say. "Show me everything."

He does. Over the next hour, he lays out every rule he has accumulated. I write them as he speaks.

For Fajr: the true dawn appears when the sun is 18 degrees below the horizon. But Bilal does not say "18 degrees." He says "when the whiteness spreads across the east, not the column — the line." He has no angle. He has a visual.

For Dhuhr: when the sun passes its highest point and the shadow begins to lengthen. In summer this is late — the sun is high, the shadow is short, and the wait is long. In winter this is early.

For Asr: the shadow equals the post height plus the noon shadow. But the noon shadow depends on the sun's maximum altitude, which depends on the day of the year and the latitude.

For Maghrib: the moment the sun's disc vanishes below the horizon.

For Isha: when the twilight — the red glow — disappears.

Each rule depends on the sun. The sun's position depends on the day. The day determines the shadow. The shadow determines the prayer. And some of these relationships are simple — Maghrib is just the moment of sunset — while others chain through three or four intermediate observations.

I stare at the notes. They cover both sides of the parchment. Dozens of rules. Cross-references between rules. Special cases for extreme latitudes where the sun never fully sets in summer. Notes on the false dawn. Corrections for mountains on the horizon. Adjustments Bilal learned from his teacher, who learned from his teacher.

The knowledge is real. Every rule has been verified against the sky. But the FORM is chaos.

> *Margin note: The inheritance problem had one estate, one family, known numbers. This is different. Bilal needs a rule that works for ANY day, ANY location. The unknown is not a single number — it is a relationship.*

Yusuf looks at the parchment. He looks at Bilal. He looks at me. I see it in his face — the same thing I felt when I first saw 27/24. Too much. The tools are not wrong. There are just too many of them, in too many forms, depending on too many conditions.

I try to organize. I write the Asr rule:

```
Shadow for Asr = post height + noon shadow
```

But the noon shadow depends on the day. So I need:

```
Noon shadow on day d = ???
```

And the Asr time depends on when the shadow reaches that length. So:

```
Asr time on day d = time when shadow = post height + noon shadow on day d
```

Each piece refers to another piece. I am writing RULES that take INPUTS and produce OUTPUTS. The day goes in. A shadow length comes out. The shadow length goes in. A prayer time comes out.

Each rule does one thing. Each rule is deterministic — the same day always gives the same noon shadow. The same shadow length always gives the same time. No ambiguity. No contradiction.

I have been writing these rules since the souk. The wife's share: take the estate, divide by 8. The farmer's zakat: take the harvest, multiply by 1/40. The merchant's equation: take the unknown wealth, apply the zakat rule. Every one of these was an input going in and an output coming out, governed by a fixed rule.

But I never NAMED the pattern. I never needed to. Each problem had one rule, applied once, to one input. Bilal's problem has dozens of rules, applied in sequence, to inputs that change every day.

I need a name for a rule that takes an input and produces an output. I need a way to write it. I need a way to chain rules together — the output of one becoming the input of the next.

I write:

```
f(d) = noon shadow length on day d
```

I look at this notation. f is the rule. d is the input. f(d) is the output. Three things — the rule, what goes in, what comes out — written in a single expression. The same day always gives the same shadow. A different day may give a different shadow. But the RULE does not change.

I call this a **function**.

Bilal watches me write. He does not read mathematical notation. But when I say, "f takes the day and gives you the noon shadow," he nods. He has been DOING this function for forty years. He just never wrote it down.

> *Margin note: I did not create the function. The sky has been running it since before Bilal was born. I am writing down what was already there.*

The prayer times are not one function. They are a CHAIN of functions. The day determines the sun's altitude. The sun's altitude determines the shadow. The shadow determines the prayer time. Three rules, applied in sequence. The output of one feeds into the input of the next.

For Yusuf, this changes everything. He does not need forty years of watching. He needs the functions — written, precise, computable. Give him the day, and he can follow the chain to the prayer time. Not by intuition. By computation.

I go back down the stairs. Bilal and Yusuf follow. I have the form. Now I need the formalism.

---

## ٣. The Derivation

### Definition

A **function** f from a set A to a set B is a rule that assigns to each element x in A **exactly one** element f(x) in B.

```
f : A → B
x ↦ f(x)
```

**f** is the function — the rule itself.
**A** is the **domain** — the set of all valid inputs.
**B** is the **codomain** — the set where outputs are permitted to live.
**f(x)** is the **image** of x — the specific output for input x.
**Range** = { f(x) : x ∈ A } — the set of outputs that actually occur.

The range sits inside the codomain but need not fill it.

### The Rule That Matters

The critical property: **each input produces exactly one output.**

If Bilal inputs "day 14 of Rajab" and gets two different Asr times, the rule is not a function. A function does not contradict itself. This is 1 = 1 at work — a thing is itself, and the output of a deterministic rule is itself. f(14) = f(14). Always.

Different inputs CAN produce the same output. Summer days near the solstice may give nearly identical noon shadows. That is permitted. What is forbidden: one input giving two outputs.

### Function Notation

When I write f(x) = x/8, I am saying:

- **f** is the name of the rule.
- **x** is a placeholder for any valid input.
- **x/8** is what the rule does: divide the input by 8.

The notation f(x) does NOT mean "f times x." It means "f applied to x."

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

**Example.** Bilal's noon shadow function.

```
f : {1, 2, 3, ..., 365} → ℝ
f(d) = noon shadow length on day d
```

Domain: the days of the year (1 through 365). Day 0 or day 400 are not valid inputs.
Codomain: ℝ (any real number of shadow length).
Range: some subset of ℝ — the shadow lengths that actually occur. The shadow is never negative, never longer than some maximum. The range is smaller than the codomain.

**Domain restrictions from algebra.** When the function is a formula, the domain is determined by what the formula permits:

- **Division by zero:** f(x) = 1/(x − 3) is defined for all x except x = 3.
- **Square roots of negatives:** f(x) = √(x − 5) is defined only for x ≥ 5.
- **Context:** If f(E) = E/8 represents the wife's share from estate E, then E > 0 — you cannot divide a negative estate.

### Types of Functions

#### Injective (One-to-One)

A function f is **injective** if different inputs always produce different outputs:

```
f(a) = f(b) → a = b
```

Equivalently: no two inputs share the same output. Every output in the range was produced by exactly one input.

**Example.** f(x) = 2x + 3. If f(a) = f(b), then 2a + 3 = 2b + 3. Subtract 3: 2a = 2b. Divide by 2: a = b. So f is injective.

**Example.** g(x) = x². Then g(3) = 9 and g(−3) = 9. Two different inputs, same output. g is NOT injective.

**Bilal's test:** If two different days give the same noon shadow, the shadow function is not injective. And they do — a day in spring and a day in autumn can produce identical shadows, because the sun reaches the same altitude on both days. Bilal's shadow function is not injective.

#### Surjective (Onto)

A function f : A → B is **surjective** if every element of the codomain B is actually hit by some input:

```
For every y ∈ B, there exists x ∈ A such that f(x) = y.
```

Equivalently: the range equals the codomain. No element of B is left unused.

**Example.** f : ℝ → ℝ, f(x) = 2x + 3. For any y ∈ ℝ, solve 2x + 3 = y: x = (y − 3)/2 ∈ ℝ. Every real number is hit. f is surjective (onto ℝ).

**Example.** g : ℝ → ℝ, g(x) = x². The output is always ≥ 0. The value −4 ∈ ℝ is never hit. g is NOT surjective onto ℝ. But g : ℝ → [0, ∞) IS surjective — the codomain matters.

#### Bijective (One-to-One and Onto)

A function that is both injective and surjective is **bijective**. Every output is produced by exactly one input. A perfect pairing — no duplicates, no gaps.

```
Bijective = Injective + Surjective
```

Bijections are the functions that can be perfectly reversed.

### Roots and Zeros

A **root** (or **zero**) of a function f is a value x₀ such that:

```
f(x₀) = 0
```

This is where the function's output is zero — where the function "crosses" zero.

Every equation I have ever solved can be rewritten as: find the roots of a function.

```
x² + 20x − 100 = 0    →    Find x where f(x) = x² + 20x − 100 equals 0
```

The patron's garden (Island 0.7). The quadratic formula gives the roots. The discriminant tells me how many:

```
b² − 4ac > 0  → two distinct real roots
b² − 4ac = 0  → one repeated root
b² − 4ac < 0  → no real roots
```

**Roots connect functions to equations.** Solving an equation IS finding where a function equals zero.

### Composition of Functions

Bilal's problem is not one function. It is a chain: the day determines the sun's altitude. The sun's altitude determines the shadow. The shadow determines the prayer time. Three functions, applied in sequence.

If I have two functions f and g, the **composite function** f ∘ g (also written fg) is defined by:

```
(f ∘ g)(x) = f(g(x))
```

Apply g first, then f. Read right to left — the function nearest to x acts first.

**Example.** Let g(x) = x + 3 and f(x) = 2x.

```
fg(x) = f(g(x)) = f(x + 3) = 2(x + 3) = 2x + 6
gf(x) = g(f(x)) = g(2x) = 2x + 3
```

fg(x) = 2x + 6, but gf(x) = 2x + 3. These are **different**.

**Composition is not commutative.** fg ≠ gf in general. Order matters. Adding 3 then doubling is not the same as doubling then adding 3. The sequence of operations changes the result.

**For composition to work, the range of g must sit inside the domain of f.** The output of the first function must be a valid input for the second. If g produces shadow lengths (positive real numbers) and f requires angles (0 to 90 degrees), the chain breaks. The domain of the outer function must contain the range of the inner function.

**Bilal's chain as composition:**

```
h(d) = sun's altitude at noon on day d        (day → angle)
s(α) = shadow length when sun is at angle α    (angle → shadow)
t(ℓ) = time when shadow reaches length ℓ       (shadow → time)

Prayer time = t(s(h(d))) = (t ∘ s ∘ h)(d)
```

Three functions composed. Day goes in. Prayer time comes out. Yusuf does not need to look at the sky. He follows the chain.

### Inverse Functions

If a function f is bijective — one-to-one AND onto — then every output was produced by exactly one input. I can reverse the process: given the output, recover the input.

The **inverse function** f⁻¹ satisfies:

```
f⁻¹(f(x)) = x    for all x in the domain of f
f(f⁻¹(y)) = y    for all y in the range of f
```

f undoes f⁻¹. f⁻¹ undoes f. They are mirror operations.

**Example.** f(x) = 2x + 3. Solve for x: y = 2x + 3 → x = (y − 3)/2. So f⁻¹(y) = (y − 3)/2.

Check: f(f⁻¹(y)) = f((y − 3)/2) = 2 × (y − 3)/2 + 3 = (y − 3) + 3 = y. ✓

**Only bijections have inverses.** If f is not injective, two inputs give the same output — so given that output, which input do I reverse to? If f is not surjective, some outputs in the codomain were never produced — there is nothing to reverse from.

**Bilal's question reversed:** Yusuf asks, "If I know the shadow length, what time is it?" That is asking for the inverse of the time-to-shadow function. The inverse only exists if the function is bijective — if each shadow length corresponds to exactly one time. In the afternoon, shadows grow monotonically (strictly increasing), so the function IS injective during that interval, and the inverse exists. Yusuf can read the time from the shadow.

**The notation f⁻¹ does NOT mean 1/f.** f⁻¹(x) is the inverse function. 1/f(x) is the reciprocal. Different operations entirely.

**The chain from 1 = 1:**

```
1 = 1 (reflexive, Island 0.1)
→ successor function gives ℕ (Island 0.2)
→ multiplication on ℕ (Island 0.3)
→ additive inverse gives ℤ (Island 0.4)
→ multiplicative inverse gives ℚ (Island 0.5)
→ variables generalize to expressions (Island 0.6)
→ quadratic formula over ℝ (Islands 0.7–0.8)
→ function: a rule f : A → B assigning each input exactly one output
→ types: injective, surjective, bijective
→ composition: chaining functions, (f ∘ g)(x) = f(g(x))
→ inverse: reversing a bijection, f⁻¹(f(x)) = x
```

---

## ٤. Al-Khwarizmi Solves

### Problem 1: Bilal's Shadow Rule

Bilal says: "At my latitude, near the equinox, the sun reaches 62 degrees at noon. The gnomon is 1 cubit tall."

I write the shadow length as a function of the sun's altitude α:

```
s(α) = 1 / tan(α)
```

But I do not have trigonometric functions yet — those belong to Arc 1. I will use Bilal's observations directly. He gives me a table from forty years of watching.

| Sun's noon altitude α | Noon shadow (cubits) |
|---|---|
| 30° | 1.73 |
| 45° | 1.00 |
| 60° | 0.58 |
| 75° | 0.27 |
| 90° | 0.00 |

Bilal's rule for Asr: the shadow must equal the gnomon height (1 cubit) PLUS the noon shadow.

```
Asr shadow = 1 + noon shadow
```

On a day when the noon altitude is 60°:

```
Noon shadow = 0.58 cubits
Asr shadow = 1 + 0.58 = 1.58 cubits
```

I define the Asr shadow as a function of the noon shadow:

```
a(n) = 1 + n

Domain: n ≥ 0 (noon shadow is never negative)
Codomain: ℝ
Range: [1, ∞) — the Asr shadow is always at least 1 cubit
```

Is this function injective? If a(n₁) = a(n₂), then 1 + n₁ = 1 + n₂, so n₁ = n₂. Yes — different noon shadows give different Asr shadows. The function is injective.

Is it surjective onto ℝ? No — a(n) ≥ 1 for all valid inputs. But onto [1, ∞)? For any y ≥ 1, set n = y − 1 ≥ 0. Then a(n) = y. Yes — surjective onto [1, ∞).

Injective and surjective onto [1, ∞). The function is bijective (on this codomain), so the inverse exists:

```
a⁻¹(y) = y − 1
```

Yusuf can go both ways: from noon shadow to Asr shadow, and from Asr shadow back to noon shadow.

Bilal nods. "The boy can use this." He runs his finger down the table. "And when he learns the noon shadow for each day of the year, he chains them."

Composition. The output of one function feeds into the input of the next.

### Problem 2: The Wife's Share as a Function

The wife's Quranic share after 'awl (Island 0.5) is 3/27 of the estate. I write:

```
w(E) = (3/27) × E = E/9

Domain: E > 0 (the estate is positive)
Codomain: ℝ⁺
Range: ℝ⁺ (every positive value is achieved)
```

Evaluate: the estate is 2700 dinars.

```
w(2700) = 2700/9 = 300 dinars
```

The wife receives 300 dinars.

Is w injective? If w(E₁) = w(E₂), then E₁/9 = E₂/9, so E₁ = E₂. Yes.

Is w surjective onto ℝ⁺? For any y > 0, set E = 9y > 0. Then w(E) = y. Yes.

So w is bijective, and the inverse exists:

```
w⁻¹(y) = 9y
```

What does the inverse mean? Given the wife's share, recover the estate. If the wife received 300 dinars, the estate was 9 × 300 = 2700 dinars.

### Problem 3: Composition — From Day to Prayer Time

The noon shadow depends on the day. The Asr shadow depends on the noon shadow. Two functions composed.

Let me define simplified versions (Bilal's approximation near the equinox):

```
n(d) = 1.2 − 0.01d    for d in [1, 90] (days from winter solstice)
```

This says the noon shadow decreases as days move from winter toward spring — the sun climbs higher. (This is a rough linear model. The real relationship requires trigonometry I do not yet have.)

```
a(n) = 1 + n           (Asr shadow = gnomon + noon shadow)
```

Compose:

```
(a ∘ n)(d) = a(n(d)) = 1 + (1.2 − 0.01d) = 2.2 − 0.01d
```

On day 30 from the winter solstice:

```
(a ∘ n)(30) = 2.2 − 0.01(30) = 2.2 − 0.3 = 1.9 cubits
```

On day 90:

```
(a ∘ n)(90) = 2.2 − 0.01(90) = 2.2 − 0.9 = 1.3 cubits
```

The Asr shadow is shorter in spring (sun higher, noon shadow shorter). Bilal confirms: "In spring, Asr comes later — the shadow takes longer to reach its mark because it starts shorter."

The composition turned two separate rules into one rule. Day goes in. Asr shadow length comes out. Yusuf needs only the composed function and a way to measure the shadow.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** Let f(x) = 3x + 7. Find f(0), f(1), f(−2), and f(10).
*(Hint: substitute each value for x and compute.)*

**2.** Bilal gives Yusuf the rule: "The Asr shadow equals the gnomon height plus the noon shadow." The gnomon is 1.5 cubits tall. The noon shadow on a certain day is 0.8 cubits.
(a) Write the Asr shadow as a function a(n) where n is the noon shadow.
(b) Compute the Asr shadow for that day.
(c) State the domain of a, given that n must be non-negative.
*(Hint: the gnomon height replaces the "1" in the worked example.)*

**3.** Let g(x) = x² − 9. Find the roots of g — that is, solve g(x) = 0.
*(Hint: factor as a difference of squares.)*

### Hasan (Exam-level)

**4.** Bilal's mosque receives an inheritance. The father's share after 'awl is 4/27 of the estate. [5 marks]
(a) Write the father's share as a function f(E). State the domain and range. [2 marks]
(b) Compute f(5400). [1 mark]
(c) Bilal asks: for what estate value E does the father receive exactly 800 dinars? [1 mark]
(d) Write the inverse function f⁻¹(y). Verify that f⁻¹(f(5400)) = 5400. [1 mark]

**5.** Bilal teaches Yusuf composition. He defines two rules: f(x) = 2x + 1 and g(x) = x² − 3. [6 marks]
(a) Find fg(x) and gf(x). [2 marks]
(b) Evaluate fg(2) and gf(2). [2 marks]
(c) Yusuf asks: "When do the two orders give the same answer?" Show that fg(x) = gf(x) has no real solutions. [2 marks]

**6.** Bilal records noon shadow lengths at his latitude. He approximates the noon shadow as n(d) = 1.5 − 0.012d cubits, where d is the number of days from the winter solstice. The gnomon is 1 cubit. [5 marks]
(a) State the domain of n, given that noon shadows must be non-negative. Find the largest valid d. [2 marks]
(b) The Asr shadow is a(n) = 1 + n. Write the composed function (a ∘ n)(d). [1 mark]
(c) On what day does the Asr shadow equal 2 cubits? [2 marks]

### Sahih (Proof and extension)

**7.** Bilal defines two prayer-time rules: f(x) = 2x + 5 and g(x) = (x − 5)/2. [6 marks]
(a) Show that f(g(x)) = x and g(f(x)) = x. [2 marks]
(b) What does this tell you about the relationship between f and g? [1 mark]
(c) Bilal explains to Yusuf: "Any rule that never confuses two inputs and covers all outputs can be reversed." Prove that if f is injective and surjective (bijective), then the inverse function f⁻¹ exists and satisfies f⁻¹(f(x)) = x for all x in the domain of f. [3 marks]

**8.** Yusuf models the brightness at the horizon as f(t) = t² − kt + (k + 3), where k depends on the season. [7 marks]
(a) Find the discriminant of f(t) = 0 in terms of k. [2 marks]
(b) Find the values of k for which the brightness touches zero exactly once (equal roots). [2 marks]
(c) For each such value of k, state when this occurs. [1 mark]
(d) For what values of k does the brightness never reach zero? [2 marks]

---

## ٦. Exam Technique

```
┌─────────────────────────────────────────────────────────────────┐
│                    FUNCTIONS — WHAT MARKERS WANT                │
│                                                                 │
│  1. NOTATION IS NOT OPTIONAL.                                   │
│     When a question says "the function f is defined by          │
│     f(x) = ...", every evaluation must show f(a) = ...          │
│     explicitly before simplifying. Do not skip to the answer.   │
│     Method marks are awarded for f(a), not for the number.      │
│                                                                 │
│  2. DOMAIN QUESTIONS — look for:                                │
│     • Division by zero → exclude values where denominator = 0   │
│     • Square roots of negatives → exclude where radicand < 0    │
│     • Context → estate values positive, days non-negative, etc. │
│     State the domain using set notation or inequalities.         │
│                                                                 │
│  3. RANGE vs. CODOMAIN.                                         │
│     "State the range" means: what outputs does the function     │
│     actually produce? For f(x) = x², the codomain may be ℝ     │
│     but the range is [0, ∞). Do not confuse them.               │
│                                                                 │
│  4. COMPOSITION — APPLY INNER FIRST.                            │
│     fg(x) = f(g(x)). Apply g to x first. Then apply f          │
│     to the result. The most common error: applying f first.     │
│     Write it in steps:                                          │
│         fg(x) = f(g(x))                                        │
│               = f(x² − 3)        ← substitute g(x)             │
│               = 2(x² − 3) + 1    ← apply f to the result       │
│               = 2x² − 5                                        │
│                                                                 │
│  5. INVERSE — SWAP AND SOLVE.                                   │
│     To find f⁻¹: write y = f(x), then solve for x in terms     │
│     of y. The result is f⁻¹(y). Always verify by checking       │
│     f(f⁻¹(y)) = y. Remember: only bijections have inverses.     │
│                                                                 │
│  6. ROOTS vs. GENERAL SOLUTIONS.                                │
│     "Find the roots of f" means solve f(x) = 0.                │
│     "Solve f(x) = 5" is NOT finding roots. Be precise.          │
│                                                                 │
│  Common mistake: writing fg(x) = f(x) × g(x). That is the     │
│  PRODUCT, not the COMPOSITION. fg(x) means f(g(x)).             │
└─────────────────────────────────────────────────────────────────┘
```

---

## ٧. Log Pose

```
0.8 Irrationals ──→ [0.9 FUNCTIONS] ──→ 0.10 Limits
                          │
                          ├──→ 0.11 Derivatives (functions to differentiate)
                          ├──→ Arc 1: Trigonometric functions (the moon's
                          │          true curve, Bilal's shadow formula)
                          ├──→ Arc 1: Exponential functions (growth/decay)
                          └──→ Arc 2: Coordinate Geometry (functions as curves)
```

**This island unlocks:**
- **Island 0.10: Limits** — I can write the rule. But what happens as the input approaches a boundary? What does f(x) get close to when x gets close to something it cannot reach?
- **Island 0.11: Derivatives** — Yusuf needs the RATE: how fast is the light changing at dawn? That requires the derivative of a function — a concept that needs limits first.

**Dependencies satisfied:**
- ← 0.7 Quadratics (polynomial roots, discriminant)
- ← 0.8 Irrationals (ℝ as domain/codomain)
- ← 0.5 Fractions (rational functions, inheritance shares as linear functions)
- ← 0.6 Variables (functions generalize what variables began)

**Introduced here for the first time:**
- Function notation: f(x), f : A → B
- Domain, codomain, range
- Injective, surjective, bijective
- Roots/zeros of functions
- Composition: f(g(x))
- Inverse functions

---

## ٨. Reflection

Bilal folds the page and places it inside his robe. The notation is strange to him. But the meaning is not. Every rule I wrote, he already knew. What he could not do was hand it to Yusuf in a form Yusuf could carry.

A function is the bridge between knowing and transmitting. Bilal watches the sky and knows. Yusuf reads the function and computes. The knowledge passes from the master to the student not through years of watching, but through a rule written precisely enough that anyone who follows it arrives at the same answer.

The Quran commanded: establish prayer at the decline of the sun. The command is absolute. The method of determining "when" is human work — observation encoded into rules, rules written as functions, functions chained through composition. The worship does not wait for us to formalize the mathematics. But the formalization lets the worship persist beyond one man's lifetime.

Tomorrow, Yusuf will climb the minaret stairs alone for the first time. He will carry Bilal's page. He will check the shadow against the gnomon. He will compute. And when the shadow reaches the mark, he will call the Asr prayer — not because he watched Bilal do it, but because the function told him it was time.

The inheritance problem is far behind me now. But it taught me this: every tool I build exists because a person needed it. The buyer needed a true scale. The shepherd needed to count. The farmer needed to multiply. The debtor needed zero. The family needed fractions. The merchant needed variables. The patron needed quadratics. The builder needed irrationals. And Bilal — Bilal needed a way to write what he knows so that it outlasts him.

I have the rule. But I do not yet have the space between the values. Bilal's shadow does not jump from one length to the next — it sweeps continuously, growing through every real number between two marks. What happens between the entries in his table? What does the shadow approach when the sun is at the horizon — a boundary it touches for only an instant?

A traveler has arrived at the courtyard gate. Dusty cloak. Cracked lips. An empty water-skin. He has been walking toward the city walls for hours. Every hour, the distance halves. He is always getting closer. He is never quite there.

He will need limits.

---

> أَقِمِ الصَّلَاةَ لِدُلُوكِ الشَّمْسِ
> *"Establish prayer at the decline of the sun..."*

*1 = 1 has not been lost.*
