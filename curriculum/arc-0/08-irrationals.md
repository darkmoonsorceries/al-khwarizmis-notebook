# Island 0.8: Irrationals — The Builder's Diagonal

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> أَفَلَا يَنظُرُونَ إِلَى الْإِبِلِ كَيْفَ خُلِقَتْ
> "Do they not look at the camels, how they are created?"
> *— Surah Al-Ghashiyah (88:17)*

**Connection grade: Honest Chain** — The Quran commands observation. Obeying that command — looking at a unit square — reveals a diagonal no fraction can name. Chain: command to observe → observe a square → measure the diagonal → √2 is not rational. Three links, each real.

**The problem this ayah creates:** A builder needs the exact diagonal of his courtyard. When I look — truly look — at this shape, I find a length my fractions cannot hold.

---

## ٢. Al-Khwarizmi Discovers

Something has shifted.

For seven islands I built tools because people needed them. The buyer, the shepherd, the farmer, the debtor, the grieving family, the merchant, the patron — each brought a problem. Each problem forced new mathematics. The tools obeyed.

Now a different command. Not "divide justly." Not "record the debt."

*Do they not look at how it is created?*

Not compute. Not divide. Look.

---

A builder stands in my courtyard. Calloused hands. Chalk dust in the creases of his knuckles. A measuring cord over his shoulder, knotted at regular intervals. He is laying tiles for a square courtyard — one cubit per side.

"I need the diagonal's length," he says. "Exact. The tile-cutter charges by the cubit and I will not pay for waste."

I draw his courtyard in the dust.

<!-- diagram: unit-square -->

> *A square. One cubit per side. The simplest shape in geometry.*

By the theorem of right triangles: if the sides are 1 and 1, the diagonal *d* satisfies `d² = 1² + 1² = 2`. So `d = √2`.

"Good," the builder says. "What fraction is that?"

---

Every number I have ever used is a fraction. Every quantity I computed for the inheritance, the zakat, the garden — fractions. My entire arithmetic lives inside ℚ. So √2 must be a fraction. I just need to find it.

<!-- diagram: diagonal -->

> *The diagonal drawn. It has a length. I can hold the cord in my hands. What fraction is it?*

"7/5," I say. That gives 1.4.

The builder squints. "You are sure?"

I check. `(7/5)² = 49/25 = 1.96`. Not 2.

---

<!-- diagram: fraction-attempts -->

> *Each fraction tried. Each fraction crossed out. 7/5, then 99/70, then 577/408. The gap shrinks. It never closes.*

I try 99/70. Squared: `9801/4900 = 2.000204...` Too large. I try 140/99. Squared: `19600/9801 = 1.99979...` Too small. I try 577/408. Squared: `332929/166464 = 1.999994...` Six decimal places of agreement. Still not 2.

> *Margin note: Each fraction gets closer. None arrives. I am chasing a number that runs faster than my fractions can follow.*

The builder is no longer patient. "You are the mathematician," he says. "Give me the number."

I cannot. Not because I have not tried enough. Perhaps no fraction exists. The cord is still stretched across the courtyard. The length is REAL. I can hold it. But I cannot write it as *a*/*b* for any integers *a* and *b*.

---

I must stop guessing and prove it.

Suppose √2 is a fraction. Suppose √2 = *a*/*b*, where *a* and *b* are integers with no common factor. Lowest terms. If such a fraction exists, I will find what it requires.

Square both sides: `2 = a²/b²`, so `a² = 2b²`.

Then *a*² is even. Can *a* be odd? If *a* were odd, *a*² would be odd. But *a*² = 2*b*² is even. So *a* is even. Write *a* = 2*k*.

Substitute: `(2k)² = 2b²`, so `4k² = 2b²`, so `b² = 2k²`.

Now *b*² is even. By the same argument, *b* is even.

I stop.

<!-- diagram: contradiction -->

> *Assume √2 = a/b in lowest terms. Both a and b forced even. The assumption destroys itself.*

Both even. Both divisible by 2. But I assumed lowest terms — no common factor. They share 2. The assumption has destroyed itself. Not a fraction I have not found. A fraction that CANNOT exist.

√2 is not a rational number.

---

The builder does not care about proofs. He needs tiles.

"Between 1.414 and 1.415," I tell him. "Tell the tile-cutter 1.414 and trim the excess."

He nods. Wraps the cord around his fist. Goes.

The approximation serves the builder. The proof serves the truth.

> *Margin note: The inheritance overflow was solvable — 'awl restored it. The debtor's position was solvable — negatives absorbed it. Every previous gap could be closed by extending the system. This gap is different. The rationals are not broken. They are incomplete.*

I need a number system that holds every fraction AND every constructible length. Every point on the line, no gaps. I need the real numbers.

**Omar Khayyam** — mathematician, astronomer, poet of Nishapur. He argued what the Greeks could not accept: that irrational numbers ARE legitimate numbers. His *Treatise on Demonstration of Problems of Algebra* classified equations demanding these numbers. His Jalali calendar measured the year to six decimal places — more precise than the Gregorian calendar that replaced it five centuries later. He looked at creation and measured what he found.

---

## ٣. The Derivation

### Proof that √2 is irrational

**Theorem.** There is no rational number whose square is 2. That is, √2 ∉ ℚ.

**Proof** (by contradiction).

Assume, for the sake of contradiction, that √2 ∈ ℚ.

Then there exist integers *a*, *b* with *b* ≠ 0 such that:

```
√2 = a/b
```

where gcd(*a*, *b*) = 1 (the fraction is in lowest terms).

<!-- diagram: formal-proof -->

> *The proof skeleton: assume → square → deduce → substitute → deduce → contradict → conclude.*

**Step 1.** Square both sides:

```
2 = a²/b²   →   a² = 2b²
```

**Step 2.** *a*² = 2*b*² is even. If *a* were odd, *a*² = (2m+1)² = 4m²+4m+1 would be odd. So *a* is even. Write *a* = 2*k*.

**Step 3.** Substitute *a* = 2*k*:

```
(2k)² = 2b²   →   4k² = 2b²   →   b² = 2k²
```

**Step 4.** *b*² = 2*k*² is even. Same reasoning: *b* is even.

**Step 5.** Both even → gcd(*a*, *b*) ≥ 2. Contradicts gcd(*a*, *b*) = 1. Therefore √2 ∉ ℚ. ∎

---

### The real number line ℝ

The rationals are *dense*: between any two, there is another. They still do not fill the line. √2 proves a gap exists.

**Definition.** The **real numbers** ℝ are all numbers corresponding to points on the number line. ℝ contains every rational and fills every gap.

**Irrational numbers** — reals that are not rational:
- **Surds:** √2, √3, √5 — roots that do not simplify to rationals
- **Transcendentals:** not roots of any integer-coefficient polynomial. Another time.

**Decimal test.** Rational ↔ terminates or eventually repeats:
- `1/3 = 0.333...` (repeating → rational)
- `√2 = 1.41421356...` (non-repeating, non-terminating → irrational)

---

### The hierarchy of number systems

<!-- diagram: formal-number-hierarchy -->

> *Each extension forced by a problem the previous system could not solve. ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ.*

| System | Symbol | What forced it | What it adds |
|--------|--------|----------------|--------------|
| Naturals | ℕ | Counting (0.2) | 0, 1, 2, 3, ... |
| Integers | ℤ | Subtraction: 3 − 5 = ? (0.4) | Negative numbers |
| Rationals | ℚ | Division: 1 ÷ 3 = ? (0.5) | Fractions |
| Reals | ℝ | Geometry: diagonal of unit square (0.8) | Irrational numbers |
| Complex | ℂ | Algebra: √(−1) = ? | *Arc 1* |

```
ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ
```

Every natural is an integer. Every integer is rational. Every rational is real. Not every real is rational — √2 proves this.

---

### Surds and simplification

A **surd** is an irrational root that cannot simplify to a rational number.

**Rules:**

```
√(ab) = √a × √b       (√a)² = a       √(a/b) = √a / √b
```

**Simplifying** — extract the largest perfect square factor:

```
√72 = √(36 × 2) = 6√2       √50 = 5√2       √48 = 4√3
```

**Arithmetic** — combine like surds only:

```
3√2 + 5√2 = 8√2       2√2 + 3√3 → cannot simplify
(2 + √3)(2 − √3) = 4 − 3 = 1       ← difference of squares
```

**Rationalizing the denominator:**

```
1/√2 = √2/2                       (multiply by √2/√2)
1/(3 + √2) = (3 − √2)/7          (multiply by conjugate)
```

The **conjugate** of `a + √b` is `a − √b`. Product: `a² − b`, rational.

---

**The chain from 1 = 1:**

```
1 = 1 (reflexive, 0.1)
  → equality preserved under operations (0.1)
    → multiplication, distributive law (0.3)
      → fractions: a/b with b ≠ 0 (0.5)
        → assume √2 = a/b in lowest terms
          → a² = 2b² → both a, b even → contradicts lowest terms
            → √2 ∉ ℚ → ℝ required
```

---

## ٤. Al-Khwarizmi Solves

### Example 1: The builder's five-cubit courtyard

The builder returns. His actual courtyard is 5 cubits per side. He needs the full diagonal.

<!-- diagram: example-diagonal-length -->

> *A 5-cubit square. The diagonal: √50 = 5√2.*

By Pythagoras:

```
d² = 5² + 5² = 50
d = √50
```

Simplify — the largest perfect square factor of 50:

```
50 = 25 × 2
√50 = √(25 × 2) = 5√2
```

As a decimal: `5 × 1.414... ≈ 7.071`. The surd is exact. The decimal is practical.

---

### Example 2: Simplify and rationalize

**Simplify** `3√50 − 2√18 + √32`.

Extract the largest perfect square factor from each:

```
√50 = √(25 × 2) = 5√2
√18 = √(9 × 2) = 3√2
√32 = √(16 × 2) = 4√2
```

<!-- diagram: example-surds -->

> *Three disguised surds. All multiples of √2. Simplification reveals it.*

So: `3(5√2) − 2(3√2) + 4√2 = 15√2 − 6√2 + 4√2 = 13√2`.

**Rationalize** `5/(3 − √2)` — multiply by conjugate `3 + √2`:

```
5(3 + √2) / (9 − 2) = (15 + 5√2) / 7
```

---

## ٥. Your Turn

### Da'if (Guided)

<!-- diagram: ex-daif-surds -->

**1.** The builder measures a rectangular courtyard with sides 1 cubit and 2 cubits. Find the exact diagonal length. Is it rational or irrational?

*Hint: d² = 1² + 2² = 5. Is 5 a perfect square?*

**2.** Simplify each surd:

(a) √75

(b) √200

(c) 2√27 + 3√12

*Hint for (c): simplify each surd first, then combine like terms.*

**3.** The builder needs to cut a tile strip for a diagonal of length `4/√2` cubits. Rationalize the denominator and simplify.

*Hint: multiply top and bottom by √2.*

---

### Hasan (Exam-level)

<!-- diagram: ex-hasan-proof -->

**4.** A square courtyard has area 18 square cubits. The builder needs the side length and the diagonal length, both in simplified surd form. [5 marks]

(a) Find the side length.
(b) Find the diagonal length.
(c) The builder orders tiles in strips of 0.5 cubits. How many strips does he need for the full diagonal? Give your answer as a whole number.

**5.** The builder calculates timber lengths: `(√50 + √32) / √2`. Simplify to a single integer. [4 marks]

**6.** The builder divides two timber lengths and gets `(4 + √3) / (2 − √3)`. Rationalize the denominator and simplify. [4 marks]

**7.** Show that `√2 + 1` is irrational. [4 marks]

*Hint: assume it is rational, so √2 + 1 = r where r ∈ ℚ. Then √2 = r − 1. But r − 1 ∈ ℚ...*

---

### Sahih (Proof and extension)

**8.** Prove that √5 is irrational. [6 marks]

*Method: assume √5 = a/b in lowest terms, show 5 | a and 5 | b, contradict. Justify: if 5 | a², then 5 | a (5 is prime).*

**9.** Prove that √2 + √3 is irrational. [7 marks]

*Hint: assume √2 + √3 = r ∈ ℚ. Square (r − √2)² = 3. Isolate √2.*

---

## ٦. Exam Technique

> **Proof by contradiction — the skeleton**
>
> ```
> 1. ASSUME: √p = a/b, gcd(a, b) = 1
> 2. SQUARE: a² = pb²
> 3. DEDUCE: p | a (p prime)
> 4. SUBSTITUTE: a = pk → p | b
> 5. CONTRADICT: gcd ≥ p ≠ 1
> ```
>
> Works for any prime *p*. Not composites: √4 = 2 is rational. **What examiners want:** state "gcd(*a*, *b*) = 1" explicitly. This is the fulcrum — without it, no contradiction.

> **Rationalizing denominators**
>
> - **Single surd:** `k/√n = k√n/n`
> - **Binomial:** multiply by conjugate. `k/(a ± √b) = k(a ∓ √b)/(a² − b)`
> - **Common error:** forgetting to distribute across the entire numerator.

> **Surd simplification**
>
> Extract the largest perfect square factor first. `√72 = √(36 × 2) = 6√2` — one step, not two.

---

## ٧. Log Pose

```
ISLAND 0.8 — IRRATIONALS
=========================

    Unlocked:
    +-- Proof that √2 is irrational (by contradiction)
    +-- The real numbers ℝ
    +-- Number hierarchy: ℕ ⊂ ℤ ⊂ ℚ ⊂ ℝ ⊂ ℂ
    +-- Surds: simplification, arithmetic, rationalization

    Callbacks:
    +-- 0.1 — Equality: the proof rests on a = a (a thing is itself)
    +-- 0.3 — Multiplication: (2k)² = 4k² uses it
    +-- 0.5 — Fractions: a/b in lowest terms IS the rational assumption
    +-- 0.7 — Quadratic formula gave √200 = 10√2; now I know what it is

    Forward:
    +-- 0.9 — Functions: with ℝ as domain, functions map every real number
    +-- Arc 1 — Complex Numbers: ℝ → ℂ, the final extension
    +-- Pattern: equation honest, system incomplete → EXTEND

    The chain so far:
    1 = 1
    +-- Equality (the scale)
    +-- Counting (the shepherd)
    +-- Multiplication (the grain)
    +-- Zero and negatives (the debt)
    +-- Fractions (the inheritance)
    +-- Variables (the unknown estate)
    +-- Quadratics (the garden)
    +-- Irrationals (the diagonal)     <-- YOU ARE HERE
```

---

## ٨. Reflection

Something has changed.

For seven islands I built tools because people needed them. Each stood before me with a problem. I built the tool. The person left.

The builder left too. He has his 1.414. His tiles will be cut. Close enough to perfect that no eye could tell.

But I am not done. √2 is different from every gap before it. The inheritance overflow was solvable. The debtor's position was solvable. Each extension closed the system. This gap does not close. The rationals are not broken — they are incomplete. Creation does not confine itself to ratios of whole numbers.

The Quran said: *do they not look at how it is created?*

I looked at a square. The Creator's geometry exceeds my arithmetic.

That is the pivot. Seven islands answered: what tools does justice require? This island: what does creation contain? The second question has no end.

Outside, the sun is low. An old man climbs the minaret steps. Bilal. Forty years he has called the prayer. Tonight he watches the sky — not for beauty, but for the rule. The moon's phase changes night by night. He can read it in his bones, but his successor Yusuf cannot.

Bilal needs to write the rule down. An input — the day. An output — the prayer time. Something Yusuf can follow without forty years of watching.

He does not know it yet, but he is asking for a function.

*1 = 1 has not been lost.*

---
