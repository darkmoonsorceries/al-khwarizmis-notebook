# Island 0.10: Limits — The Traveler's Approach

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> تَعْرُجُ الْمَلَائِكَةُ وَالرُّوحُ إِلَيْهِ فِي يَوْمٍ كَانَ مِقْدَارُهُ خَمْسِينَ أَلْفَ سَنَةٍ
>
> "The angels and the Spirit ascend to Him in a day whose measure is fifty thousand years."
> *— Surah Al-Ma'arij (70:4)*

**Connection grade: HONEST CHAIN** — the verse describes approach across an immeasurable span. Fifty thousand years of ascending — toward Him, never arriving, the distance conceptually shrinking without terminus. The verse is about divine majesty, not mathematics. But the structure it describes — directed approach across a scale that dwarfs the traveler — is the phenomenon that limits formalize. The chain: Quran describes ascending approach toward a destination (70:4) → observation of approach-without-arrival reveals the need for limits → limits formalize what "approaches" means.

**The problem this ayah creates:** A thing approaches. The distance shrinks. It is always positive — fifty thousand years is not zero. And yet the ascent is real, the destination governs the motion. How do I write mathematics for something that is always getting closer but never arriving — and prove that arrival still happens?

---

## ٢. Al-Khwarizmi Thinks

A traveler stands at the courtyard gate.

Dusty cloak, cracked lips, an empty water-skin hanging from his belt like a dead thing. He has been walking since dawn. I can see the road behind him — flat, pale, vanishing into heat.

"The city walls," he says. "How far?"

I know this road. I walked it once. "Sixteen miles from where you stand."

He nods. He is not asking out of curiosity. His water-skin is empty. His lips are split. Sixteen miles is the distance between this man and water.

"I will reach it," he says. He shifts his pack higher on his shoulders and turns east.

I watch him go. And because my mind does what it does, I begin to count.

> *Margin note: The inheritance problem taught me that mathematics either serves people or it is vanity. This man needs water. That is not a metaphor.*

At noon he is sixteen miles from the city. I know this road — the ground is soft, the heat thick, and travelers slow as the hours pass. Suppose each hour he covers half the remaining distance. Not because he chooses to, but because fatigue halves his effort with every stretch. At noon: sixteen miles. At the first hour: eight remain. At the second: four. At the third: two.

I scratch the sequence in the dust:

```
Noon:    16 miles remaining
Hour 1:  8
Hour 2:  4
Hour 3:  2
Hour 4:  1/2
Hour 5:  1/4
Hour 6:  1/8
```

The distances shrink. They shrink fast. After six hours the man is one-eighth of a mile from the gate — close enough to see the grain of the wood, close enough to hear voices inside.

But I keep going:

```
Hour 7:  1/16
Hour 8:  1/32
Hour 9:  1/64
Hour 10: 1/128
```

The distance is always positive. Always. `16/2ⁿ` is never zero, no matter how large n becomes. Halve a number forever and you get smaller and smaller numbers, each one still positive, each one still a real distance between the man and the gate.

He never arrives.

I stare at the dust. The mathematics says the distance is always positive. His feet are still moving. The gate is right there. Every fool on this road can see he is almost at the city. And yet — `16/2ⁿ > 0` for every n. Always greater than zero. Always short of the gate.

The math and the road disagree.

I know which one is wrong. The man WILL reach the city. He has legs, the ground is solid, the gate does not recede. But my tools — functions, equations, arithmetic — cannot express what is happening. I can compute his distance at any hour. I cannot compute the hour at which the distance is zero, because there is no such hour in my sequence. The function `d(n) = 16/2ⁿ` never outputs zero.

> *Margin note: The builder in Island 0.8 found a length he could not write as a fraction. I face something stranger: a destination I can see, a man who will arrive, and a formula that says he won't.*

I try something else. Forget the remaining distance. Ask instead: how far has he walked in total?

```
After hour 1:  8 miles walked
After hour 2:  8 + 4 = 12
After hour 3:  8 + 4 + 2 = 14
After hour 4:  8 + 4 + 2 + 1 = 15
After hour 5:  15 + 1/2 = 15.5
After hour 6:  15.5 + 1/4 = 15.75
After hour 7:  15.75 + 1/8 = 15.875
```

The total is growing. But it is not growing without bound. It crawls toward something. Fifteen. Fifteen and a half. Fifteen and three-quarters. Fifteen and seven-eighths.

Sixteen?

I add more terms. The total after ten hours: `8 + 4 + 2 + 1 + 1/2 + 1/4 + 1/8 + 1/16 + 1/32 + 1/64`. I compute: `15 + 63/64 = 15.984375`. After twenty hours, the sum is closer still — `16 - 1/2²⁰`, a number so close to sixteen that the difference would not fill a grain of sand.

The sum never exceeds 16. It never reaches 16. But name any number less than 16 — say, 15.999 — and I can find enough terms to surpass it. The sum passes every checkpoint below 16 and stops at none of them. It is going somewhere.

I do not have a word for this. The function never reaches zero. The sum never reaches sixteen. But both are headed there — drawn there — as surely as the traveler is drawn to the gate.

I need a word for "the value a thing approaches without necessarily reaching." I need mathematics that can say: this is where it IS GOING, even if no single step takes it there.

I call it the limit.

```
lim {n → ∞} 16/2ⁿ = 0
```

Not: "16/2ⁿ equals zero for some n." It never does. But: "16/2ⁿ can be made as close to zero as you demand, by choosing n large enough." Name your tolerance. One mile? n = 5 gives 1/2. A thousandth of a mile? n = 14 gives less than that. A billionth? Choose n = 34. Whatever closeness you require, I can meet it. That guarantee IS the limit.

And the sum:

```
lim {n → ∞} (8 + 4 + 2 + ... + 8/2ⁿ) = 16
```

The series converges to 16. The traveler's total journey: 16 miles. Finite. Complete. He arrives.

The paradox dissolves. The math and the road never disagreed. I was asking the wrong question. I asked: "At which step does the distance equal zero?" There is no such step. The right question is: "What does the distance approach?" Zero. "What does the total distance approach?" Sixteen. The limit answers the question my old tools could not even phrase.

The traveler reaches the city. He drinks.

> *Margin note: The inheritance shares summed to 27/24 — more than the whole. That was a finite overflow, and 'awl restored it. Here the sum approaches 16 — exactly the whole. No overflow. The infinite process is better behaved than the finite one.*

But this idea reaches further than the road.

I think of Bilal's functions from Island 0.9. Suppose I have a function — not a sequence, but a rule `f(x)` — and I want to know what happens as `x` approaches some value `a`. Take a simple case:

```
f(x) = (x² − 1)/(x − 1)
```

What happens at `x = 1`? The denominator is zero. The function is not defined. There is nothing there — a hole in the road. But I can compute nearby:

```
x = 0.9:   f(x) = (0.81 − 1)/(0.9 − 1) = (−0.19)/(−0.1) = 1.9
x = 0.99:  f(x) = (0.9801 − 1)/(0.99 − 1) = 1.99
x = 0.999: f(x) = 1.999
x = 1.001: f(x) = 2.001
x = 1.01:  f(x) = 2.01
x = 1.1:   f(x) = 2.1
```

From both sides, the function approaches 2. The hole at `x = 1` does not destroy the pattern. I factor:

```
(x² − 1)/(x − 1) = (x + 1)(x − 1)/(x − 1) = x + 1    (for x ≠ 1)
```

As `x` approaches 1, `x + 1` approaches 2. The limit is 2. The function never takes the value 2 at `x = 1` — it is not defined there — but it approaches 2 from every direction.

A limit at a point. The same idea as the traveler, in a different form. Approach without arrival. The value that governs the neighborhood even when the point itself is missing.

And now: what if the function IS defined at the point, and the limit IS the value? Then there is no gap. The approach and the arrival agree. The function does what you expect when you get there.

I have a word for that too. Continuity. A continuous function has no surprises at the doorstep. The traveler's distance function `d(t) = 8 - 5t` — linear, smooth, no holes — is continuous everywhere. When d(t) reaches zero, it IS zero. No paradox. No gap.

But when a function is continuous and it changes sign — positive at one end, negative at the other — then somewhere between, it must cross zero. It cannot jump over. A continuous function on a solid number line has no gaps to skip through. The completeness of the reals, which the builder found in Island 0.8, guarantees this.

The traveler's distance starts positive (he is far from the city) and — if we use the continuous model — eventually becomes negative (he has passed through). Somewhere in between, it was exactly zero. He crossed the threshold. The mathematics now proves what his feet already knew.

---

## ٣. The Derivation

### Limits of Sequences

**Definition.** A sequence `a₁, a₂, a₃, ...` has limit L if: for every ε > 0 (however small), there exists N such that for all n > N, `|aₙ − L| < ε`.

In words: pick any distance from L, no matter how tiny. Eventually the sequence gets that close and stays that close. Not just once — permanently.

**Example.** The traveler's distance: `aₙ = 16/2ⁿ`.

Claim: `lim {n → ∞} 16/2ⁿ = 0`.

```
Given ε > 0, I need |16/2ⁿ − 0| < ε.
That is: 16/2ⁿ < ε.
That is: 2ⁿ > 8/ε.
Choose N so that 2^N > 8/ε. (Such N always exists
because 2ⁿ grows without bound.)
Then for all n > N: 2ⁿ > 2^N > 16/ε, so 16/2ⁿ < ε.  ∎
```

**The traveler's total distance (geometric series).**

The sum of the first n terms:

```
Sₙ = 8 + 4 + 2 + ... + 8/2ⁿ⁻¹
```

This is a geometric series with first term `a = 8` and ratio `r = 1/2`. The partial sum formula:

```
Sₙ = a × (1 − rⁿ)/(1 − r) = 8 × (1 − (1/2)ⁿ)/(1/2) = 16 × (1 − 1/2ⁿ)
```

As `n → ∞`, `1/2ⁿ → 0`, so:

```
lim {n → ∞} Sₙ = 16 × (1 − 0) = 16
```

The series converges to 16. The traveler covers exactly 16 miles. He arrives.

**General geometric series.** For `|r| < 1`:

```
┌─────────────────────────────────────────┐
│  a + ar + ar² + ar³ + ... = a/(1 − r)  │
│  (converges when |r| < 1)              │
└─────────────────────────────────────────┘
```

When `|r| ≥ 1`, the series diverges — the terms do not shrink, so the sum grows without bound.

### Limits of Functions at a Point

**Definition.** We write

```
lim {x → a} f(x) = L
```

to mean: for every ε > 0, there exists δ > 0 such that whenever `0 < |x − a| < δ`, we have `|f(x) − L| < ε`.

The key: `0 < |x − a|`. We never ask what happens AT `x = a`. We ask what happens NEAR it. Approaching, not arriving.

**Intuition (the challenge game).** Your opponent names ε — how close `f(x)` must be to L. You respond with δ — how close `x` must be to `a`. If you can always respond, no matter how small ε is, the limit is L.

**Example.** `lim {x → 1} (x² − 1)/(x − 1) = 2`.

For `x ≠ 1`: `(x² − 1)/(x − 1) = x + 1`.

Given ε > 0, choose δ = ε. Then for `0 < |x − 1| < δ`:

```
|(x + 1) − 2| = |x − 1| < δ = ε  ∎
```

The function is undefined at `x = 1`. The limit exists anyway.

**Example.** `lim {x → 3} (2x + 1) = 7`.

Given ε > 0, choose δ = ε/2. Then for `0 < |x − 3| < δ`:

```
|2x + 1 − 7| = |2x − 6| = 2|x − 3| < 2δ = ε  ∎
```

### Limits at Infinity

**Definition.** We write

```
lim {x → ∞} f(x) = L
```

to mean: for every ε > 0, there exists N such that for all `x > N`, `|f(x) − L| < ε`.

Same idea as sequences — eventually the function enters the ε-band around L and stays there.

**Technique for rational functions.** Divide numerator and denominator by the highest power of x in the denominator.

**Example.** `lim {x → ∞} (3x + 1)/(x + 2)`.

```
(3x + 1)/(x + 2) = (3 + 1/x)/(1 + 2/x)
```

As `x → ∞`: `1/x → 0`, `2/x → 0`. The limit is `(3 + 0)/(1 + 0) = 3`.

Check: `x = 100` gives `301/102 ≈ 2.95`. `x = 1000` gives `3001/1002 ≈ 2.997`. Approaching 3.

### One-Sided Limits

Sometimes a function approaches different values from the left and the right.

**Definition.** `lim {x → a⁺} f(x) = L` means: the limit as x approaches a from ABOVE (x > a). `lim {x → a⁻} f(x) = L` means: from BELOW (x < a).

The two-sided limit `lim {x → a} f(x)` exists if and only if both one-sided limits exist and are equal.

**Example.** Let `f(x) = |x|/x` for `x ≠ 0`.

```
For x > 0: f(x) = x/x = 1
For x < 0: f(x) = −x/x = −1
```

`lim {x → 0⁺} f(x) = 1` and `lim {x → 0⁻} f(x) = −1`. The one-sided limits exist but disagree, so `lim {x → 0} f(x)` does not exist.

### Limit Laws

If `lim {x → a} f(x) = L` and `lim {x → a} g(x) = M`, then:

| Law | Statement |
|-----|-----------|
| Sum | `lim {x → a} [f(x) + g(x)] = L + M` |
| Product | `lim {x → a} [f(x) × g(x)] = L × M` |
| Quotient | `lim {x → a} [f(x)/g(x)] = L/M`, provided `M ≠ 0` |
| Scalar | `lim {x → a} [c × f(x)] = c × L` |
| Power | `lim {x → a} [f(x)]ⁿ = Lⁿ` |

These follow from the epsilon-delta definition. The proofs are technical; the intuition is immediate. If f approaches L and g approaches M, their sum approaches L + M. I state them without proof — the rigor is available, the intuition is sufficient here.

### Continuity

**Definition.** A function f is **continuous at a** if three conditions hold:

```
┌────────────────────────────────────────────────────┐
│  1. f(a) is defined.                               │
│  2. lim {x → a} f(x) exists.                      │
│  3. lim {x → a} f(x) = f(a).                      │
│                                                    │
│  Continuity: the limit IS the value. No gap        │
│  between approach and arrival.                     │
└────────────────────────────────────────────────────┘
```

**Polynomials** are continuous everywhere. For any polynomial `p(x)`, `lim {x → a} p(x) = p(a)`. Substitute directly.

**Rational functions** `p(x)/q(x)` are continuous wherever `q(x) ≠ 0`.

**The traveler's continuous model.** If d(t) = 8 − 5t (a polynomial, hence continuous), then `lim {t → 8/5} d(t) = d(8/5) = 0`. No gap. The distance IS zero at `t = 8/5`. He arrives because the function is continuous — the approach and the arrival are the same event.

### The Intermediate Value Theorem (IVT)

**Theorem.** If f is continuous on the closed interval [a, b], and f(a) and f(b) have opposite signs, then there exists some c in (a, b) such that f(c) = 0.

A continuous function that starts negative and ends positive (or vice versa) must cross zero somewhere in between. It cannot jump over. The number line has no gaps (Island 0.8 — the completeness of ℝ), and a continuous function has no jumps. Together: no escape. The root exists.

**Proof sketch.** Bisect [a, b]. Check the sign of f at the midpoint. The root lies in whichever half still has the sign change. Bisect again. And again. Each bisection traps the root in a smaller interval. The intervals shrink to a point. That point is the root. (The full proof uses the completeness of ℝ — that every bounded sequence of reals has a limit. Without irrationals, there would be gaps to skip through, and the IVT would fail.)  ∎

**Application to the traveler.** His distance function d(t) = 8 − 5t is continuous. At t = 0, d(0) = 8 > 0 (he is far from the city). At t = 2, d(2) = −2 < 0 (he has passed through). By the IVT, there exists some c in (0, 2) with d(c) = 0. He crosses the threshold. The IVT guarantees what his legs already knew: a man walking steadily toward a city on a continuous road will reach it.

**The chain from 1 = 1:**

```
1 = 1 (Island 0.1)
→ ℕ, ℤ, ℚ, ℝ (Islands 0.2–0.8, building the complete number line)
→ functions f : A → B (Island 0.9)
→ limits of sequences: lim {n → ∞} aₙ = L means aₙ can be made
  as close to L as desired by choosing n large enough
→ limits of functions: lim {x → a} f(x) = L means f(x) can be made
  as close to L as desired by choosing x close enough to a
→ continuity: lim {x → a} f(x) = f(a) — approach equals arrival
→ IVT: continuous functions on ℝ cannot skip values — the
  completeness of ℝ (Island 0.8) guarantees it
```

---

## ٤. Al-Khwarizmi Solves

### Problem 1: The Traveler's Distance (the person's problem, worked fully)

The traveler halves his remaining distance each hour. At noon: 8 miles. Compute his distance and total distance walked at each stage.

**Step 1.** The distance remaining at hour n:

```
dₙ = 16/2ⁿ
```

**Step 2.** Compute:

```
n = 0: d₀ = 8
n = 1: d₁ = 4
n = 2: d₂ = 2
n = 3: d₃ = 1
n = 4: d₄ = 1/2
n = 5: d₅ = 1/4
n = 10: d₁₀ = 8/1024 ≈ 0.0078
```

**Step 3.** The limit:

```
lim {n → ∞} 16/2ⁿ = 0
```

The distance approaches zero. He approaches the city.

**Step 4.** Total distance walked (partial sum of geometric series):

```
Sₙ = 8 + 4 + 2 + ... + 8/2ⁿ⁻¹ = 16 × (1 − 1/2ⁿ)
```

```
S₃ = 16 × (1 − 1/8) = 14
S₅ = 16 × (1 − 1/32) = 15.5
S₁₀ = 16 × (1 − 1/1024) ≈ 15.984
```

**Step 5.** The limit of the sum:

```
lim {n → ∞} Sₙ = 16
```

The city is 16 miles from his starting point. The series converges. He arrives.

### Problem 2: A Hole in the Function

Evaluate `lim {x → 2} (x³ − 8)/(x − 2)`.

**Step 1.** Direct substitution: `(8 − 8)/(2 − 2) = 0/0`. Undefined. There is a hole.

**Step 2.** Factor. Recall the difference of cubes: `a³ − b³ = (a − b)(a² + ab + b²)`.

```
x³ − 8 = (x − 2)(x² + 2x + 4)
```

**Step 3.** Simplify for `x ≠ 2`:

```
(x³ − 8)/(x − 2) = (x − 2)(x² + 2x + 4)/(x − 2) = x² + 2x + 4
```

**Step 4.** Take the limit:

```
lim {x → 2} (x² + 2x + 4) = 4 + 4 + 4 = 12
```

The function has a hole at `x = 2`, but it approaches 12. The limit sees through the hole.

### Problem 3: Using the IVT to Guarantee a Root

Show that `f(x) = x³ − 3x + 1` has a root in (0, 1).

**Step 1.** Evaluate at the endpoints:

```
f(0) = 0 − 0 + 1 = 1 > 0
f(1) = 1 − 3 + 1 = −1 < 0
```

**Step 2.** Sign change: f(0) > 0 and f(1) < 0.

**Step 3.** f is a polynomial, hence continuous on [0, 1].

**Step 4.** By the IVT, there exists some c in (0, 1) with f(c) = 0.  ∎

I do not know what c is. I know it exists. The function changed sign across a continuous interval. The root is trapped. The IVT is the net; the completeness of ℝ is the ground beneath it.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** The traveler's companion sets out from a different point, 12 miles from the city. He too halves his remaining distance each hour.

(a) Write his remaining distance at hour n.
(b) Compute his distance at hours 1, 2, 3, 4, 5.
(c) What is the limit of his distance as n → ∞?
(d) Write the total distance walked as a series. What does it converge to?

*Hint: Same pattern as the traveler. First term is 12, ratio is 1/2. Use the geometric series formula.*

**2.** Evaluate `lim {x → 3} (x² − 9)/(x − 3)`.

*Hint: Factor the numerator as a difference of squares: x² − 9 = (x − 3)(x + 3).*

**3.** A water merchant fills a tank that holds 100 liters. Each hour, he adds half the remaining capacity. After hour 1: 50 liters. After hour 2: 75 liters. After hour 3: 87.5 liters.

(a) Write the amount in the tank after n hours.
(b) Does the tank ever reach 100 liters?
(c) What is the limit of the amount as n → ∞?

*Hint: After n hours the amount is `100 × (1 − 1/2ⁿ)`. This is the same structure as the traveler's total distance.*

### Hasan (Exam-level)

**4.** The traveler has a second route to the city. On this route, the remaining distance at hour n is `dₙ = 10 × (2/3)ⁿ`. [6 marks]

(a) Compute d₁, d₂, d₃, d₄. [2 marks]
(b) Show that `lim {n → ∞} dₙ = 0`. [1 mark]
(c) Write the total distance as a geometric series and find its sum. [2 marks]
(d) How far is the city from the starting point on this route? [1 mark]

**5.** The traveler watches two caravans on a long road. Their distances are governed by `(4x² − x + 3)/(2x² + 5x − 1)`. As the road stretches toward the horizon, evaluate `lim {x → ∞} (4x² − x + 3)/(2x² + 5x − 1)`. [3 marks]

**6.** The traveler measures a spring's flow rate: `f(x) = (x² − 4)/(x − 2)` litres per hour, but at hour `x = 2` the spring surges and the formula breaks. [5 marks]

(a) Simplify f(x) for `x ≠ 2`. [1 mark]
(b) Find the flow rate the spring approaches: `lim {x → 2} f(x)`. [1 mark]
(c) The traveler's companion records `g(x) = f(x)` for `x ≠ 2` and writes `g(2) = 5`. Is g continuous at `x = 2`? Justify by checking all three conditions. [2 marks]
(d) What value of g(2) would make the record continuous at `x = 2`? [1 mark]

**7.** The traveler's path follows `x³ + 2x − 5 = 0` where x is the crossing point of a river. Show that a crossing exists in the interval (1, 2). [4 marks]

State clearly:
- That the function is a polynomial (hence continuous).
- The values f(1) and f(2) and their signs.
- Which theorem guarantees the crossing and its conditions.

### Sahih (Proof and extension)

**8.** The traveler needs to find where a valley floor crosses sea level. The elevation is `f(x) = x² − 7`. [6 marks]

(a) Show that f(2) < 0 (below sea level) and f(3) > 0 (above). [1 mark]
(b) By the IVT, there exists a crossing point c in (2, 3) with f(c) = 0. What is c? [1 mark]
(c) The traveler cannot mark this point exactly on his rope. Explain why — connect to Island 0.8. [1 mark]
(d) He narrows the location by bisection: evaluate f(2.5), determine which half contains the crossing, then bisect again. [3 marks]

**9.** A geometric series has first term a and common ratio r, with `|r| < 1`. [5 marks]

(a) Derive the partial sum formula: `Sₙ = a(1 − rⁿ)/(1 − r)`. [2 marks]
(b) Show that `lim {n → ∞} rⁿ = 0` when `|r| < 1`. (You may use the fact that `|r|ⁿ` is a decreasing sequence bounded below by 0.) [1 mark]
(c) Hence show that the infinite sum is `a/(1 − r)`. [1 mark]
(d) The traveler covers 8, 4, 2, 1, ... miles. Verify that the formula gives 16 as the total. [1 mark]

---

## ٦. Exam Technique

```
┌─────────────────────────────────────────────────────────────────┐
│                    LIMITS — WHAT EXAMINERS WANT                 │
│                                                                 │
│  "SHOW THAT A ROOT EXISTS IN THE INTERVAL..."                  │
│  This appears on nearly every FP1 paper. The method is rigid:  │
│                                                                 │
│  1. Write f(x) = [equation rearranged so one side is 0].       │
│  2. Evaluate f(a) and f(b) at the endpoints.                   │
│  3. State: "f(a) = ... > 0 and f(b) = ... < 0" — explicitly   │
│     note the SIGN CHANGE.                                      │
│  4. State: "f is continuous on [a, b]" and say WHY             │
│     (e.g., "f is a polynomial").                               │
│  5. Conclude: "By the IVT, there exists c in (a, b)           │
│     with f(c) = 0."                                            │
│                                                                 │
│  Miss step 3 or 4 → marks lost. The examiner needs to see     │
│  the sign change AND the continuity statement.                  │
│                                                                 │
│  COMMON ERRORS:                                                 │
│  × Forgetting to state continuity. The IVT requires it.        │
│  × Computing f(a) and f(b) correctly but not stating the       │
│    sign change explicitly. The mark is for the statement,      │
│    not the computation.                                         │
│  × Applying IVT across a discontinuity (e.g., a rational      │
│    function with a zero denominator inside the interval).       │
│                                                                 │
│  LIMITS BY SUBSTITUTION:                                        │
│  For polynomials where the denominator is non-zero,            │
│  the limit IS the substitution: lim {x → a} p(x) = p(a).     │
│  Only factor/simplify when direct substitution gives 0/0.      │
│                                                                 │
│  LIMITS AT INFINITY:                                            │
│  For rational functions: divide every term by the highest      │
│  power of x in the denominator. Then the 1/x, 1/x² terms     │
│  vanish. The limit is the ratio of leading coefficients        │
│  (when degrees match) or 0 or ∞ (when they don't).            │
│                                                                 │
│  SERIES CONVERGENCE:                                            │
│  Geometric series with |r| < 1 → state sum = a/(1 − r).       │
│  Show your substitution. Examiners want to see a and r         │
│  identified explicitly.                                         │
└─────────────────────────────────────────────────────────────────┘
```

---

## ٧. Log Pose

```
0.8 Irrationals ────┐
(completeness of ℝ) │
                     │
0.9 Functions ───────┤
(the objects whose   │
limits I take)       ▼
                ╔═══════════════════╗
                ║  0.10  LIMITS     ║  ◄── YOU ARE HERE
                ║  The Traveler's   ║
                ║  Approach         ║
                ╚════════╤══════════╝
                         │
                         │  "I can describe what a function
                         │   approaches. Now: how FAST is
                         │   it changing at a single instant?"
                         │
                         ▼
                ┌───────────────────┐
                │  0.11 DERIVATIVES │
                │  The Fajr Call    │
                └───────────────────┘
                         │
                         ├──→ Arc 3: Numerical Methods
                         │    (bisection uses IVT,
                         │     Newton-Raphson uses derivatives)
                         │
                         └──→ Arc 4: Series & Convergence
                              (geometric series → power series
                               → Taylor series)

This island unlocks:
  × 0.11 Derivatives — the derivative IS a limit: f'(x) = lim {h → 0}
    [f(x+h) − f(x)]/h. Without limits, the derivative has no foundation.
  × Numerical methods — bisection narrows intervals using sign changes
    (IVT). Newton-Raphson uses the derivative to leap toward roots.
  × Series — convergence of infinite sums is DEFINED by limits.
    The geometric series here is the first example.

Dependencies satisfied:
  ← 0.9 Functions (the objects whose limits I take)
  ← 0.8 Irrationals (completeness of ℝ — the IVT needs no gaps)
```

---

## ٨. Reflection

The sun is low. The shadow of the minaret has crossed the courtyard and climbed the far wall.

Somewhere on the eastern road, the traveler is walking. Or running. His water-skin is empty and the city gate is ahead and the distance shrinks with every step. The sequence `8, 4, 2, 1, 1/2, ...` says the distance is always positive. The limit says it approaches zero. The series says his total journey converges to 16 miles. He was always going to arrive. The mathematics never disagreed with the road — I was asking the wrong question. Not "when does the distance equal zero?" but "what does the distance approach?"

The limit is different from every tool I built before. Equality was definite: `a = a`. Counting was exhaustive: 47 out, 47 back. Fractions were precise: `3/24` of the estate. Functions were rules: input, output, done. The limit does not give a definite answer at a definite point. It gives the answer at the edge — the value a function is headed toward, whether or not it arrives.

And yet it is no less certain. `lim {n → ∞} 16/2ⁿ = 0` is as true as `1 + 1 = 2`. The guarantee is not weaker for being about approach rather than arrival. The epsilon-delta definition IS the guarantee: name your tolerance, and I will meet it. Every time. No exceptions.

I think of the inheritance from the prologue. The shares summed to `27/24` — a finite overflow that 'awl resolved by proportional reduction. Here, an infinite sum converges to exactly 16 — no overflow, no reduction needed. The infinite process, governed by a limit, is better behaved than the finite one that started this journey.

Ten tools. Equality. Counting. Multiplication. Zero. Fractions. Variables. Quadratics. Irrationals. Functions. And now limits — the mathematics of approach, the language of "getting closer."

One tool remains. I can describe what a function approaches. I cannot yet describe how fast it is changing at a single instant. The function tells me WHERE something is. The limit tells me where it is GOING. But I need the rate — not the position, not the destination, but the speed at a single frozen moment. Rate is change divided by time. At a single instant, the time interval is zero. Division by zero is what the qadi encountered in Island 0.4: forbidden.

Unless I take the limit.

Tomorrow at dawn. Young Yusuf — Bilal's apprentice — will stand on the minaret roof alone for the first time. The sky will brighten. He will need to call the fajr prayer at the exact moment true dawn breaks. Not the position of the light. Not where the light is going. How FAST the light is changing — right now, at this instant. The derivative.

> تَعْرُجُ الْمَلَائِكَةُ وَالرُّوحُ إِلَيْهِ
> *"The angels and the Spirit ascend to Him..."*

The ascent is real. The destination governs the motion. The limit is how mathematics speaks of approach — and approach, in this creation, is everywhere.

*1 = 1 has not been lost.*

---

*Next: Island 0.11 — Derivatives. Yusuf on the roof at fajr. The sky brightens. How fast is the light changing — right now?*
