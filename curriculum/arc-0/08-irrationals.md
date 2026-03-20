# Island 0.8: Irrationals — The Builder's Diagonal

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> أَفَلَا يَنظُرُونَ إِلَى الْإِبِلِ كَيْفَ خُلِقَتْ ۝ وَإِلَى السَّمَاءِ كَيْفَ رُفِعَتْ ۝ وَإِلَى الْجِبَالِ كَيْفَ نُصِبَتْ ۝ وَإِلَى الْأَرْضِ كَيْفَ سُطِحَتْ
>
> "Do they not look at the camels, how they are created? And at the sky, how it is raised? And at the mountains, how they are erected? And at the earth, how it is spread out?"
> *— Surah Al-Ghashiyah (88:17-20)*

**Connection grade: HONEST CHAIN** — The Quran commands observation of creation (88:17). Obeying that command — looking at the simplest geometric shape, a unit square — reveals a diagonal whose length no fraction can name. The Quran did not name √2. It commanded the looking that discovers it. Chain: command to observe → observation of a square → measurement of the diagonal → proof that √2 is not rational. Three links, each real.

**The problem this ayah creates:** A builder needs the exact diagonal of his square courtyard. When I obey the command and look — truly look — at this shape, I find a length my fractions cannot hold.

---

## ٢. Al-Khwarizmi Thinks

Something has shifted.

For seven islands, I built tools because people needed them. The buyer needed equality. The shepherd needed counting. The farmer, the debtor, the grieving family, the merchant, the patron — each brought a human problem, and each problem forced a new piece of mathematics into existence. The tools served the people. The Quran commanded justice, division, recording — and the mathematics obeyed.

Now a different command. Not "divide justly." Not "record the debt." The Quran says: *do they not look at how it is created?*

Not compute. Not divide. *Look.*

A builder stands in my courtyard. Calloused hands. Chalk dust on his forearms, ground into the creases of his knuckles. A measuring cord hangs over his shoulder, knotted at regular intervals. He is laying tiles for a square courtyard — one cubit per side. He wants a decorative band running corner to corner, along the diagonal.

"I need the diagonal's length," he says. "Exact. The tile-cutter charges by the cubit and I will not pay for waste."

I draw his courtyard in the dust.

```
   1
+-----+
|    /|
| d / | 1
|  /  |
| /   |
|/    |
+-----+
```

By the theorem that bears another man's name but belongs to truth: if the sides are 1 and 1, the diagonal *d* satisfies `d² = 1² + 1² = 2`. So `d = √2`.

"Good," the builder says. "What fraction is that?"

I reach for the answer. Every number I have ever used is a fraction. The naturals: `3 = 3/1`. The integers: `−5 = −5/1`. Zero: `0/1`. Every quantity I computed for the inheritance, the zakat, the garden — fractions. My entire arithmetic lives inside Q, the rational numbers. So √2 must be a fraction. I just need to find it.

"7/5," I say. That gives 1.4. Close to the right length.

The builder squints. "You are sure?"

I check. `(7/5)² = 49/25 = 1.96`. Not 2.

"Try again," he says.

I try 141/100. Squared: `19881/10000 = 1.9881`. Closer. Not 2.

I try 1414/1000. Squared: `1999396/1000000 = 1.999396`. Closer still. Not 2.

The builder watches me scratch fractions in the dust and cross them out. He has seen apprentices do this — guess, check, fail, guess again. He is patient because he thinks I will get there. I think I will get there. There must be a fraction whose square is exactly 2. I just have not found it yet.

I try 99/70. Squared: `9801/4900 = 2.000204...` Too large. I try 140/99. Squared: `19600/9801 = 1.99979...` Too small. I try 577/408. Squared: `332929/166464 = 1.999994...` Six decimal places of agreement. Still not 2.

> *Margin note: Each fraction gets closer. None arrives. The gap shrinks but never closes. I am chasing a number that runs faster than my fractions can follow.*

The builder is no longer patient. "You are the mathematician," he says. "Give me the number."

I cannot. Not because I have not tried enough fractions. Something worse. A suspicion: perhaps no fraction exists. Perhaps the diagonal of the simplest shape in geometry — a unit square — falls between every pair of rational numbers without being one of them. Perhaps my number system has a hole where this measurement should be.

The cord is still stretched across the builder's courtyard. The length is real. I can hold it in my hands. The diagonal *exists*. But I cannot write it as *a*/*b* for any integers *a* and *b*.

> *Margin note: The inheritance overflow (27/24 > 1) was solvable — 'awl restored it. The debtor's position (3 − 5) was solvable — negatives absorbed it. Every previous gap in my number system could be closed by extending the system. What if this gap is different? What if it is not a gap in my tools but a fact about creation?*

I must stop guessing and prove it. Not "I haven't found the fraction yet." I need to know: does the fraction exist, or doesn't it?

Suppose it does. Suppose √2 = *a*/*b*, where *a* and *b* are integers with no common factor. The fraction is in lowest terms. If such a fraction exists, I will find what it requires.

Square both sides: `2 = a²/b²`, so `a² = 2b²`.

Then *a*² is even — it equals 2 times something. Can *a* be odd? If *a* were odd, then *a*² would be odd, because odd × odd = odd. But *a*² = 2*b*² is even. So *a* cannot be odd. *a* is even. Write *a* = 2*k*.

Substitute: `(2k)² = 2b²`, so `4k² = 2b²`, so `b² = 2k²`.

Now *b*² is even. By the same argument, *b* is even.

I stop.

Both *a* and *b* are even. Both divisible by 2. But I assumed *a*/*b* was in lowest terms — they share no common factor. They share 2. The assumption has destroyed itself. I assumed √2 was a fraction in lowest terms, and the assumption forced both numerator and denominator to share a factor. No escape. No fraction. Not one I haven't found — one that *cannot exist*.

√2 is not a rational number.

The builder is still waiting. He does not care about proofs. He needs tiles.

"The diagonal is √2 cubits," I tell him. "Between 1.414 and 1.415. Tell the tile-cutter 1.414 and trim the excess. No mortal hand lays tiles more precisely than that."

He nods. Wraps the cord around his fist. Goes back to his courtyard.

The approximation serves the builder. The proof serves the truth. He got a number he can use. I got a fact I cannot escape: his diagonal is real, it is exact, and my fractions will never name it exactly.

I look at the dust where I drew the square. The simplest shape. Four equal sides. One diagonal. And that diagonal contains a number my entire system — naturals, integers, rationals — cannot express. Not because the system is wrong. Because creation is richer than the system.

The Quran said: *do they not look at how it is created?*

I looked. I found that the Creator's geometry exceeds my arithmetic.

> *Margin note: This is the pivot. For seven islands I built tools to serve human needs — division, debt, inheritance. Now creation itself demands tools I do not have. The command shifts from "divide justly" to "look at how it is created." Obedience to the first gave me Q. Obedience to the second demands R.*

I need a number system that holds every fraction *and* every length I can construct. Every point on the number line, with no gaps. The rationals, plus whatever lives between them.

I need the real numbers.

---

## ٣. The Derivation

### Proof that √2 is irrational

**Theorem.** There is no rational number whose square is 2. That is, √2 ∉ Q.

**Proof** (by contradiction).

Assume, for the sake of contradiction, that √2 ∈ Q.

Then there exist integers *a*, *b* with *b* ≠ 0 such that:

```
√2 = a/b
```

where gcd(*a*, *b*) = 1 (the fraction is in lowest terms).

**Step 1.** Square both sides:

```
2 = a²/b²   →   a² = 2b²
```

**Step 2.** Since *a*² = 2*b*², the integer *a*² is even. An even square implies an even root: if *a* were odd, then *a*² = (2m+1)² = 4m² + 4m + 1 would be odd. Therefore *a* is even. Write *a* = 2*k* for some integer *k*.

**Step 3.** Substitute *a* = 2*k*:

```
(2k)² = 2b²   →   4k² = 2b²   →   b² = 2k²
```

**Step 4.** Since *b*² = 2*k*², the integer *b*² is even. By the same reasoning, *b* is even.

**Step 5.** Both *a* and *b* are even, so gcd(*a*, *b*) ≥ 2. This contradicts the assumption that gcd(*a*, *b*) = 1.

**Conclusion.** The assumption that √2 ∈ Q leads to contradiction. Therefore √2 ∉ Q. ∎

---

### The real number line ℝ

The rationals Q are *dense*: between any two rationals, there is another rational. This might suggest they fill the number line completely. They do not. The proof above shows there are points on the line — such as √2 — that no rational number occupies.

**Definition.** The **real numbers** ℝ are the set of all numbers that correspond to points on the number line. ℝ contains every rational number and fills every gap the rationals leave.

**Irrational numbers** are real numbers that are not rational:
- **Surds:** √2, √3, √5, (1 + √5)/2 — roots that do not simplify to rationals
- **Transcendentals:** numbers that are not roots of any polynomial with integer coefficients. The ratio of a circle's circumference to its diameter is one. But that is a discovery for another time.

**Decimal test.** A number is rational if and only if its decimal expansion terminates or eventually repeats:
- `1/3 = 0.333...` (repeating → rational)
- `1/4 = 0.25` (terminating → rational)
- `√2 = 1.41421356...` (non-repeating, non-terminating → irrational)

---

### The hierarchy of number systems

Each extension was forced. Not invented for elegance. Forced by a problem the previous system could not solve.

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

Every natural is an integer. Every integer is rational. Every rational is real. But not every real is rational — √2 proves this. And not every equation's solution is real — the discriminant Δ < 0 proves *that*. Even the reals will not be enough.

---

### Properties of irrational numbers

**Closure under arithmetic is partial.** Unlike ℚ, the irrationals alone do not form a closed system:
- √2 + (−√2) = 0 (rational). Sum of two irrationals can be rational.
- √2 × √2 = 2 (rational). Product of two irrationals can be rational.
- √2 + √3 is irrational. (But proving this requires more work — see Sahih problem 10.)

**Density.** Between any two real numbers, there is both a rational and an irrational number. The rationals and irrationals are interleaved everywhere, infinitely, with no gaps.

---

### Surds and simplification

A **surd** is an expression containing an irrational root that cannot be simplified to a rational number.

**The product rule for roots:**

```
√(ab) = √a × √b       (a, b ≥ 0)
√(a/b) = √a / √b       (a ≥ 0, b > 0)
(√a)² = a
```

**Simplifying surds** — extract the largest perfect square factor:

```
√72 = √(36 × 2) = 6√2
√50 = √(25 × 2) = 5√2
√48 = √(16 × 3) = 4√3
```

**Adding and subtracting surds** — combine like terms only:

```
3√2 + 5√2 = 8√2
4√3 − √3 = 3√3
2√2 + 3√3  →  cannot be simplified (unlike surds)
```

**Multiplying surds:**

```
√2 × √3 = √6
3√2 × 4√5 = 12√10
(2 + √3)(2 − √3) = 4 − 3 = 1
```

The last identity is the **difference of squares**: `(a + √b)(a − √b) = a² − b`. This eliminates the surd.

**Rationalizing the denominator** — remove surds from the denominator.

For a single surd, multiply top and bottom by the surd:

```
1/√2 = (1 × √2)/(√2 × √2) = √2/2
```

For a binomial with a surd, multiply by the **conjugate**:

```
1/(3 + √2) = (3 − √2)/((3 + √2)(3 − √2)) = (3 − √2)/(9 − 2) = (3 − √2)/7
```

The conjugate of `a + √b` is `a − √b`. Their product is `a² − b`, which is rational.

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

The builder returns. His actual courtyard is not 1 cubit per side — it is 5. He needs the diagonal length for the full courtyard.

By Pythagoras:

```
d² = 5² + 5² = 25 + 25 = 50
d = √50
```

Simplify — find the largest perfect square factor of 50:

```
50 = 25 × 2
√50 = √(25 × 2) = 5√2
```

As a decimal: `5 × 1.41421... ≈ 7.071`.

The builder orders 7.1 cubits of decorative tile to account for cutting waste. The surd `5√2` gives the exact answer. The decimal gives the practical one. Both are honest — they serve different needs.

---

### Example 2: Prove that √3 is irrational

The builder asks about an equilateral triangle. Its height involves √3. Is that also irrational?

**Proof** (by contradiction).

Assume √3 = *a*/*b* in lowest terms, so gcd(*a*, *b*) = 1.

Then `3 = a²/b²`, so `a² = 3b²`.

Since *a*² is divisible by 3, *a* must be divisible by 3. Why? If *a* were not divisible by 3, then *a* = 3*m* + 1 or *a* = 3*m* + 2. In the first case, *a*² = 9*m*² + 6*m* + 1, which leaves remainder 1 when divided by 3. In the second case, *a*² = 9*m*² + 12*m* + 4, which also leaves remainder 1 when divided by 3. Either way, *a*² is not divisible by 3 — contradiction. So *a* is divisible by 3.

Write *a* = 3*k*. Substitute: `9k² = 3b²`, so `b² = 3k²`.

Now *b*² is divisible by 3, so *b* is divisible by 3 (same argument).

Both *a* and *b* divisible by 3 contradicts gcd(*a*, *b*) = 1. Therefore √3 ∉ ℚ. ∎

The key step: if a *prime* *p* divides *a*², then *p* divides *a*. This holds because primes cannot split across factors. The same method proves √*p* irrational for any prime *p*.

---

### Example 3: Simplify and rationalize

**Simplify** `3√50 − 2√18 + √32`.

Extract the largest perfect square factor from each:
- `√50 = √(25 × 2) = 5√2`
- `√18 = √(9 × 2) = 3√2`
- `√32 = √(16 × 2) = 4√2`

So: `3(5√2) − 2(3√2) + 4√2 = 15√2 − 6√2 + 4√2 = 13√2`

All three surds were disguised multiples of √2. Simplification revealed it.

**Rationalize** the denominator of `5/(3 − √2)`:

Multiply numerator and denominator by the conjugate `3 + √2`:

```
5(3 + √2) / ((3 − √2)(3 + √2))
= (15 + 5√2) / (9 − 2)
= (15 + 5√2) / 7
```

The denominator is rational.

---

## ٥. Your Turn

### Da'if (Guided)

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

**4.** A square courtyard has area 18 square cubits. The builder needs the side length and the diagonal length, both in simplified surd form. [5 marks]

(a) Find the side length.
(b) Find the diagonal length.
(c) The builder orders tiles in strips of 0.5 cubits. How many strips does he need for the full diagonal? Give your answer as a whole number.

**5.** The builder measures a pentagonal tile with side √5 cubits. He needs to compute `(3 + √5)²` to find the area of an outer frame. Express the result in the form `a + b√5` where *a* and *b* are integers. [3 marks]

**6.** The builder calculates timber lengths: `(√50 + √32) / √2`. Simplify to a single integer. [4 marks]

**7.** The builder asks: "Is √2 + 1 a ratio I can measure exactly?" Show that `√2 + 1` is irrational. [4 marks]

*Hint: assume it is rational, so √2 + 1 = r where r ∈ ℚ. Then √2 = r − 1. But r − 1 ∈ ℚ...*

**8.** The builder divides two timber lengths and gets `(4 + √3) / (2 − √3)`. Rationalize the denominator and simplify. [4 marks]

---

### Sahih (Proof and extension)

**9.** The builder encounters a second unmeasurable diagonal: √5. Prove that √5 is irrational. [6 marks]

Follow the method from the derivation: assume √5 = *a*/*b* in lowest terms, show *a*² = 5*b*² implies 5 | *a*, substitute *a* = 5*k*, show 5 | *b*, reach contradiction. You must justify: if 5 | *a*², then 5 | *a* (use the fact that 5 is prime).

**10.** The builder discovers that two unmeasurable lengths combined are still unmeasurable. Prove that √2 + √3 is irrational. [7 marks]

*Hint: assume √2 + √3 = r ∈ ℚ. Then √3 = r − √2. Square both sides: 3 = r² − 2r√2 + 2. Isolate √2 and observe what this means.*

---

## ٦. Exam Technique

> **Proof by contradiction — the skeleton**
>
> Every irrationality proof at this level follows one structure:
>
> ```
> 1. ASSUME: √p = a/b in lowest terms, gcd(a, b) = 1
> 2. SQUARE: a² = pb²
> 3. DEDUCE: p | a² → p | a (because p is prime)
> 4. SUBSTITUTE: a = pk → b² = pk²
> 5. DEDUCE: p | b² → p | b
> 6. CONTRADICT: p divides both a and b, but gcd(a, b) = 1
> 7. CONCLUDE: √p ∉ ℚ
> ```
>
> This works for any prime *p*. For composite numbers, check first — √4 = 2 is rational. The method works because primes have the property: if *p* | *a*², then *p* | *a*. Composite numbers lack this: 4 | 36 but 4 ∤ 6.
>
> **What examiners want:** State your assumption clearly. Write "gcd(*a*, *b*) = 1" or "in lowest terms" — this is the fulcrum. Without it, there is no contradiction to reach.

> **Rationalizing denominators — when and why**
>
> An answer with a surd in the denominator is not wrong, but it is not fully simplified. Examiners expect rationalized denominators.
>
> - **Single surd:** multiply top and bottom by the surd. `k/√n = k√n/n`.
> - **Binomial with surd:** multiply by the conjugate. `k/(a ± √b) = k(a ∓ √b)/(a² − b)`.
>
> **Common error:** forgetting to multiply the *entire* numerator by the conjugate. If the numerator is `(3 + √2)`, distribute fully.

> **Surd simplification — the method**
>
> Always extract the largest perfect square factor first. Missing it still works but costs time:
>
> ```
> √72 = √(4 × 18) = 2√18 = 2√(9 × 2) = 6√2    (two steps)
> √72 = √(36 × 2) = 6√2                           (one step — faster)
> ```
>
> Both earn full marks. The second saves time and reduces errors.

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

For seven islands I built tools because human beings needed them. A buyer needed fair weights. A shepherd needed certainty. A farmer, a debtor, a grieving family, a merchant, a patron — each stood before me with a problem that demanded new mathematics. I built the tool. The problem was solved. The person left with what they came for.

The builder left too. He has his 1.414. His tiles will be cut, his courtyard will be built, and the diagonal band will run from corner to corner, close enough to perfect that no eye could tell the difference.

But I am not done. Because the builder's problem revealed something the inheritance never did.

The inheritance overflow — 27/24 > 1 — was solvable. 'Awl restored the proportions. The debtor's position was solvable: extend to the integers. The division 1 ÷ 3 was solvable: extend to the rationals. Each time, the extension absorbed the problem, and the system closed again, whole and sufficient.

√2 is different. The gap between ℚ and the diagonal is not a failure to be repaired. It is a feature of creation. The rationals are not broken — they are *incomplete*. They describe every ratio of whole numbers faithfully, without error. But creation does not confine itself to ratios of whole numbers. A square exists. Its diagonal exists. The diagonal's length is not a ratio.

The Quran said: *do they not look at the camels, how they are created? At the sky, how it is raised?*

I looked at a square. I looked at how it is created. And I found that the Creator's geometry exceeds my arithmetic. My tools are not wrong. They are smaller than the reality they attempt to describe. This is the first time the mathematics was not demanded by a human need but discovered through obedience to a command to *look*.

That is the pivot of this arc. The first seven islands answered: what tools does justice require? This island answers a different question: what does creation contain?

Both questions come from the Quran. Both demand mathematics. But the second question has no end — because creation is not a problem set with a final answer. It is an invitation to keep looking.

The builder's courtyard is built. The diagonal is tiled. The number √2 can be approximated as closely as his hands require, but it can never be written exactly as a fraction. He does not need it exact. I do. Because I now know that ℝ — the real numbers — is where mathematics lives when it stops serving only human problems and starts reading what is *there*.

Outside, the sun is low. An old man climbs the steps of the minaret. Bilal. Forty years he has called the prayer. His knees are callused from prostration. His hands are weathered from decades on the roof in wind and heat. Tonight he watches the sky — not for beauty, but for the rule. The moon's phase changes night by night, the same night always giving the same face. Not chance. Pattern. He can read it in his bones, but his successor Yusuf cannot.

Bilal needs to write the rule down. An input — the day — and an output — the prayer time. Something Yusuf can follow without forty years of watching.

A rule that takes one input and gives exactly one output. He does not know it yet, but he is asking for a function.

---

*End of Island 0.8 — The Builder's Diagonal*

*Next: Island 0.9 — Functions: The Muezzin's Rule*

---
