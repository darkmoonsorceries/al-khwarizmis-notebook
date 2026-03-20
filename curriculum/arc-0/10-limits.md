# Island 0.10: Limits — The Traveler's Approach

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> وَأَنَّ إِلَىٰ رَبِّكَ الْمُنتَهَىٰ
> "And that to your Lord is the final destination."
> *— Surah An-Najm (53:42)*

**Connection grade: Hasan** — The verse is about the akhirah. All motion, all striving, all approach terminates at Allah. The primary meaning is eschatological, not mathematical. But the STRUCTURE — a final destination that governs the approach, that is reached even when no single finite step arrives there — genuinely maps to the mathematical limit. The limit IS "the final destination" of a converging sequence. Structural correspondence, different primary purpose.

**The problem this ayah creates:** A thing moves toward a destination. Each step closes the gap. The gap is always positive — always short of arrival. And yet the destination is real, the motion is directed, the arrival is certain. How does mathematics speak of a destination that governs the journey when no single step completes it?

---

## ٢. Al-Khwarizmi Discovers

The traveler arrives near midday. Dust on his cloak. Cracked lips. His water-skin hangs empty.

"The city. How far?"

I know the eastern road. "Sixteen miles."

He shifts his pack and turns east. Sixteen miles between this man and water.

I watch him go. And because my mind does what it does, I begin to count.

> *Margin note: Bilal's functions gave me rules — input in, output out. This man gives me something harder: a process that never ends, aimed at a destination it never reaches.*

---

The ground is soft, the heat thick. Travelers slow on this road. Suppose each hour he covers half the remaining distance — not by choice, but because fatigue halves his effort with every stretch.

I scratch the sequence in the dust:

<!-- diagram: halving-journey -->

> *A line from here to the city gate. Each hour, the remaining distance is halved. The marks crowd together. The gate is right there.*

```
Noon:    16 miles remaining
Hour 1:  8
Hour 2:  4
Hour 3:  2
Hour 4:  1
Hour 5:  1/2
Hour 6:  1/4
```

After six hours he is a quarter-mile from the gate. Close enough to hear voices inside. I keep going:

```
Hour 7:  1/8
Hour 8:  1/16
Hour 9:  1/32
Hour 10: 1/64
```

The distance is always positive. Always. `16/2^n` is never zero, no matter how large n becomes. Halve a number forever and you get smaller and smaller numbers, each one still positive, each one still a real distance between the man and the gate.

He never arrives.

---

I stare at the dust. The mathematics says the distance is always positive. His feet are still moving. The gate is right there. Every fool on this road can see he is almost at the city.

And yet — `16/2^n > 0` for every n. Always greater than zero. Always short.

The math and the road disagree. I know which one is wrong.

The man WILL reach the city. He has legs, the ground is solid, the gate does not recede. But my tools — functions, equations, arithmetic — cannot express what is happening. The function `d(n) = 16/2^n` never outputs zero. I can compute his distance at any hour. I cannot compute the hour at which the distance IS zero, because there is no such hour.

> *Margin note: The builder found a length he could not write as a fraction. I face something stranger: a destination I can see, a man who will arrive, and a formula that says he will not.*

---

I try something else. Forget the remaining distance. Ask instead: how far has he WALKED?

<!-- diagram: convergent-sum -->

> *Bars stacking: 8, then 4, then 2, then 1... The total grows but never passes the dashed line at 16. It crowds against the ceiling but does not break through.*

```
After hour 1:  8 miles walked
After hour 2:  8 + 4 = 12
After hour 3:  8 + 4 + 2 = 14
After hour 4:  14 + 1 = 15
After hour 5:  15 + 1/2 = 15.5
After hour 6:  15.5 + 1/4 = 15.75
After hour 7:  15.75 + 1/8 = 15.875
```

The total is growing. But it is not growing without bound. It crawls toward something. Fifteen. Fifteen and a half. Fifteen and three-quarters. Fifteen and seven-eighths.

Sixteen?

After ten hours: `8 + 4 + 2 + 1 + 1/2 + ... + 1/64 = 16 - 1/1024`. A number so close to sixteen that the difference would not fill a grain of sand.

The sum never exceeds 16. It never reaches 16. But name any number less than 16 — say, 15.999 — and I can find enough terms to surpass it. The sum passes every checkpoint below 16 and stops at none of them.

It is GOING somewhere.

---

I need a word for "the value a thing approaches without necessarily reaching." Mathematics that can say: this is where it IS GOING, even if no single step takes it there.

I call it the limit.

```
lim {n -> infinity} 16/2^n = 0
```

Not: "16/2^n equals zero for some n." It never does. But: "16/2^n can be made as close to zero as you demand, by choosing n large enough."

Name your tolerance. One mile? n = 5 gives 1/2. A thousandth of a mile? n = 14 gives less than that. A billionth? Choose n = 34. Whatever closeness you require, I can meet it. That guarantee IS the limit.

<!-- diagram: epsilon-band -->

> *A horizontal band around zero, shrinking. The sequence enters the band and stays inside. No matter how narrow the band, eventually every term fits.*

And the sum:

```
lim {n -> infinity} (8 + 4 + 2 + ... + 8/2^(n-1)) = 16
```

The series converges to 16. The traveler's total journey: sixteen miles. Finite. Complete.

<!-- diagram: the-arrival -->

> *The point exists. The marks crowd toward it, the sum stacks up to it, the band closes around it. The limit is reached.*

He arrives.

---

The paradox dissolves. The math and the road never disagreed. I was asking the wrong question. I asked: "At which step does the distance equal zero?" There is no such step. The right question: "What does the distance APPROACH?" Zero. "What does the total distance approach?" Sixteen. The limit answers the question my old tools could not phrase.

The traveler reaches the city. He drinks.

> *Margin note: The inheritance shares summed to 27/24 — more than the whole. That was a finite overflow, and 'awl restored it. Here the sum approaches 16 — exactly the whole. No overflow. The infinite process is better behaved than the finite one.*

---

But this idea reaches further than the road.

I think of Bilal's functions from Island 0.9. Suppose I have a function `f(x) = (x^2 - 1)/(x - 1)`. What happens at `x = 1`? The denominator is zero. The function is not defined. There is nothing there — a hole in the road.

But I can compute nearby:

```
x = 0.9:   f(x) = 1.9
x = 0.99:  f(x) = 1.99
x = 0.999: f(x) = 1.999
x = 1.001: f(x) = 2.001
x = 1.01:  f(x) = 2.01
```

From both sides the function approaches 2. The hole at `x = 1` does not destroy the pattern. I factor: `(x^2 - 1)/(x - 1) = (x+1)(x-1)/(x-1) = x + 1` for `x != 1`. As x approaches 1, `x + 1` approaches 2.

A limit at a point. The same idea as the traveler. Approach without arrival. The value that governs the neighborhood even when the point itself is missing.

---

And now: what if the function IS defined at the point, and the limit IS the value? Then there is no gap. The approach and the arrival agree. The function does what you expect when you get there.

I have a word for that too. Continuity. A continuous function has no surprises at the doorstep. The traveler's distance function `d(t) = 16 - 10t` — linear, smooth, no holes — is continuous everywhere. When `d(t)` reaches zero, it IS zero.

But when a function is continuous and changes sign — positive at one end, negative at the other — then somewhere between, it MUST cross zero. It cannot jump over. A continuous function on a solid number line has no gaps to skip through. The completeness of the reals, which the builder found in Island 0.8, guarantees this.

The traveler's distance starts positive. Eventually it becomes negative — he has passed through. Somewhere in between, it was exactly zero. He crossed the threshold. The mathematics now proves what his feet already knew.

---

## ٣. The Derivation

### Limits of Sequences

**Definition.** A sequence `a_1, a_2, a_3, ...` has limit L if: for every `epsilon > 0` (however small), there exists N such that for all `n > N`, `|a_n - L| < epsilon`.

Pick any distance from L, no matter how tiny. Eventually the sequence gets that close and stays that close. Not just once — permanently.

<!-- diagram: formal-limit-def -->

> *The epsilon-delta picture. A horizontal strip of width 2epsilon centered on L. Beyond some index N, every term of the sequence lies inside the strip.*

**Example.** The traveler's distance: `a_n = 16/2^n`.

Claim: `lim {n -> infinity} 16/2^n = 0`.

```
Given epsilon > 0, I need |16/2^n - 0| < epsilon.
That is: 16/2^n < epsilon.
That is: 2^n > 16/epsilon.
Choose N so that 2^N > 16/epsilon.
(Such N exists because 2^n grows without bound.)
Then for all n > N: 16/2^n < epsilon.  []
```

**The traveler's total distance (geometric series).**

The sum of the first n terms:

```
S_n = 8 + 4 + 2 + ... + 8/2^(n-1)
```

Geometric series with first term `a = 8` and ratio `r = 1/2`:

```
S_n = a x (1 - r^n)/(1 - r) = 8 x (1 - (1/2)^n)/(1/2) = 16 x (1 - 1/2^n)
```

As `n -> infinity`, `1/2^n -> 0`, so:

```
lim {n -> infinity} S_n = 16 x (1 - 0) = 16
```

**General geometric series.** For `|r| < 1`:

```
a + ar + ar^2 + ar^3 + ... = a/(1 - r)
```

When `|r| >= 1`, the series diverges.

### Limits of Functions at a Point

**Definition.** `lim {x -> a} f(x) = L` means: for every `epsilon > 0`, there exists `delta > 0` such that whenever `0 < |x - a| < delta`, we have `|f(x) - L| < epsilon`.

The key: `0 < |x - a|`. We never ask what happens AT `x = a`. We ask what happens NEAR it.

<!-- diagram: formal-continuity -->

> *The epsilon-delta picture for functions. On the y-axis, a band around L. On the x-axis, a band around a. Every point in the delta-band maps into the epsilon-band.*

**The challenge game.** Your opponent names epsilon. You respond with delta. If you can always respond, the limit is L.

### Limits at Infinity

**Definition.** `lim {x -> infinity} f(x) = L` means: for every `epsilon > 0`, there exists N such that for all `x > N`, `|f(x) - L| < epsilon`.

**Technique for rational functions.** Divide every term by the highest power of x in the denominator. The `1/x` terms vanish.

### One-Sided Limits

`lim {x -> a+} f(x)`: approach from above. `lim {x -> a-} f(x)`: from below. The two-sided limit exists if and only if both one-sided limits exist and are equal.

### Limit Laws

If `lim {x -> a} f(x) = L` and `lim {x -> a} g(x) = M`:

| Law | Statement |
|-----|-----------|
| Sum | `lim [f(x) + g(x)] = L + M` |
| Product | `lim [f(x) x g(x)] = L x M` |
| Quotient | `lim [f(x)/g(x)] = L/M`, provided `M != 0` |
| Scalar | `lim [c x f(x)] = c x L` |
| Power | `lim [f(x)]^n = L^n` |

### Continuity

**Definition.** A function f is **continuous at a** if:

```
1. f(a) is defined.
2. lim {x -> a} f(x) exists.
3. lim {x -> a} f(x) = f(a).
```

Continuity: the limit IS the value. No gap between approach and arrival. Polynomials are continuous everywhere. Rational functions are continuous wherever the denominator is nonzero.

### The Intermediate Value Theorem (IVT)

**Theorem.** If f is continuous on [a, b], and f(a) and f(b) have opposite signs, then there exists c in (a, b) with f(c) = 0.

It cannot jump over. The number line has no gaps (Island 0.8), and a continuous function has no jumps. Together: no escape. The root exists.

**Proof sketch.** Bisect [a, b]. The root lies in whichever half has the sign change. Bisect again. The intervals shrink to a point. That point is the root. (The full proof uses completeness of the reals.)

**The chain from 1 = 1:**

```
1 = 1 (Island 0.1)
-> N, Z, Q, R (Islands 0.2-0.8, the complete number line)
-> functions f : A -> B (Island 0.9)
-> limits: lim {n -> infinity} a_n = L, lim {x -> a} f(x) = L
-> continuity: approach equals arrival
-> IVT: continuous functions on R cannot skip values
```

**Geometry spec for Layer (Mode A):**
Subject: a line segment, full length. Verb: halving marks crowd toward the endpoint, convergent rings close inward, epsilon band shrinks. Object: the limit point glows.

**Scholar — Ibn al-Haytham (965-1040 CE, Basra):**
He computed `sum(k^4)` to find the volume of a paraboloid — dividing into n slices, letting n approach infinity. This IS the limit process. Father of optics, pioneer of the experimental method.

---

## ٤. Al-Khwarizmi Solves

### Problem 1: The Traveler's Journey

The traveler halves his remaining distance each hour. Starting distance: 16 miles. Compute his remaining distance and total distance walked.

<!-- diagram: example-geometric-series -->

> *The geometric series laid out: first term 8, ratio 1/2, partial sums climbing toward 16.*

**Step 1.** Remaining distance at hour n: `d_n = 16/2^n`.

**Step 2.** Compute:

```
d_0 = 16, d_1 = 8, d_2 = 4, d_3 = 2, d_4 = 1, d_5 = 1/2
d_10 = 16/1024 ~ 0.0156
```

**Step 3.** `lim {n -> infinity} 16/2^n = 0`. He approaches the city.

**Step 4.** Total distance walked:

```
S_n = 8(1 - (1/2)^n)/(1 - 1/2) = 16(1 - 1/2^n)
```

**Step 5.** `lim {n -> infinity} S_n = 16`. He arrives.

### Problem 2: A Hole in the Function

Evaluate `lim {x -> 2} (x^3 - 8)/(x - 2)`.

<!-- diagram: example-limit-computation -->

> *The function near x = 2. A smooth curve with a hole at x = 2, the curve passing through y = 12 on both sides of the gap.*

**Step 1.** Direct substitution: `(8 - 8)/(2 - 2) = 0/0`. Undefined.

**Step 2.** Factor using difference of cubes: `x^3 - 8 = (x - 2)(x^2 + 2x + 4)`.

**Step 3.** Simplify for `x != 2`: `(x - 2)(x^2 + 2x + 4)/(x - 2) = x^2 + 2x + 4`.

**Step 4.** `lim {x -> 2} (x^2 + 2x + 4) = 4 + 4 + 4 = 12`.

The function has a hole at `x = 2`, but it approaches 12. The limit sees through the hole.

### Problem 3: The IVT Guarantees Arrival

Show that `f(x) = x^3 - 3x + 1` has a root in (0, 1).

**Step 1.** `f(0) = 0 - 0 + 1 = 1 > 0`.
**Step 2.** `f(1) = 1 - 3 + 1 = -1 < 0`.
**Step 3.** Sign change: `f(0) > 0`, `f(1) < 0`.
**Step 4.** f is a polynomial, hence continuous on [0, 1].
**Step 5.** By the IVT, there exists c in (0, 1) with `f(c) = 0`.  []

I do not know what c is. I know it exists. The function changed sign across a continuous interval. The root is trapped.

---

## ٥. Your Turn

### Da'if (Guided)

**1.** The traveler's companion sets out from 12 miles away. He too halves his remaining distance each hour.

<!-- diagram: ex-daif-sequence -->

> *A second journey line, shorter, with the same halving pattern.*

(a) Write his remaining distance at hour n.
(b) Compute his distance at hours 1, 2, 3, 4, 5.
(c) What is `lim {n -> infinity}` of his distance?
(d) Write the total distance walked as a series. What does it converge to?

*Hint: Same structure. First term 6, ratio 1/2. Use the geometric series formula: a/(1 - r).*

**2.** Evaluate `lim {x -> 3} (x^2 - 9)/(x - 3)`.

*Hint: Factor the numerator as a difference of squares: `x^2 - 9 = (x - 3)(x + 3)`.*

**3.** A water merchant fills a tank that holds 100 litres. Each hour he adds half the remaining capacity. After hour 1: 50 litres. After hour 2: 75. After hour 3: 87.5.

(a) Write the amount in the tank after n hours.
(b) Does the tank ever reach 100 litres?
(c) What is the limit as `n -> infinity`?

*Hint: After n hours, the amount is `100 x (1 - 1/2^n)`. Same structure as the traveler's sum.*

### Hasan (Exam-level)

**4.** A second route to the city. Remaining distance at hour n: `d_n = 10 x (2/3)^n`. [6 marks]

<!-- diagram: ex-hasan-epsilon -->

> *The epsilon-band challenge: given epsilon, find N such that all terms beyond N lie inside the band.*

(a) Compute `d_1, d_2, d_3, d_4`. [2 marks]
(b) Show that `lim {n -> infinity} d_n = 0`. [1 mark]
(c) Write the total distance as a geometric series and find its sum. [2 marks]
(d) How far is the city from the starting point on this route? [1 mark]

**5.** Two caravans on a long road. Their separation is governed by `(4x^2 - x + 3)/(2x^2 + 5x - 1)`. Evaluate `lim {x -> infinity} (4x^2 - x + 3)/(2x^2 + 5x - 1)`. [3 marks]

**6.** A spring's flow rate: `f(x) = (x^2 - 4)/(x - 2)` litres per hour. At hour `x = 2` the formula breaks. [5 marks]

(a) Simplify f(x) for `x != 2`. [1 mark]
(b) Find `lim {x -> 2} f(x)`. [1 mark]
(c) The traveler's companion records `g(x) = f(x)` for `x != 2` and writes `g(2) = 5`. Is g continuous at `x = 2`? Check all three conditions. [2 marks]
(d) What value of `g(2)` would make the function continuous at `x = 2`? [1 mark]

**7.** Show that `x^3 + 2x - 5 = 0` has a root in (1, 2). [4 marks]

State clearly: that f is a polynomial (hence continuous), the values `f(1)` and `f(2)` and their signs, and which theorem guarantees the root.

### Sahih (Proof and extension)

**8.** The traveler needs to find where a valley floor crosses sea level. Elevation: `f(x) = x^2 - 7`. [6 marks]

(a) Show that `f(2) < 0` and `f(3) > 0`. [1 mark]
(b) By the IVT, there exists c in (2, 3) with `f(c) = 0`. What is c? [1 mark]
(c) The traveler cannot mark this point exactly on his rope. Explain why — connect to Island 0.8. [1 mark]
(d) Narrow the location by bisection: evaluate `f(2.5)`, determine which half contains the crossing, then bisect again. [3 marks]

**9.** Derive the geometric series sum formula. [5 marks]

(a) Derive the partial sum: `S_n = a(1 - r^n)/(1 - r)`. [2 marks]
(b) Show that `lim {n -> infinity} r^n = 0` when `|r| < 1`. [1 mark]
(c) Hence show the infinite sum is `a/(1 - r)`. [1 mark]
(d) Verify the formula gives 16 for the traveler's journey (a = 8, r = 1/2). [1 mark]

---

## ٦. Exam Technique

> **"SHOW THAT A ROOT EXISTS IN THE INTERVAL..."**
>
> This appears on nearly every FP1 paper. The method is rigid:
>
> 1. Write `f(x) = [equation rearranged so one side is 0]`.
> 2. Evaluate `f(a)` and `f(b)` at the endpoints.
> 3. State: "f(a) = ... > 0 and f(b) = ... < 0" — note the SIGN CHANGE explicitly.
> 4. State: "f is continuous on [a, b]" and say WHY (e.g., "f is a polynomial").
> 5. Conclude: "By the IVT, there exists c in (a, b) with f(c) = 0."
>
> Miss step 3 or 4 and you lose marks. The examiner needs the sign change AND the continuity statement.
>
> **COMMON ERRORS:**
> - Forgetting to state continuity. The IVT requires it.
> - Computing `f(a)` and `f(b)` correctly but not stating the sign change explicitly. The mark is for the STATEMENT, not the computation.
> - Applying IVT across a discontinuity (e.g., a rational function with a zero denominator inside the interval).
>
> **LIMITS BY SUBSTITUTION:**
> For polynomials where the denominator is nonzero, the limit IS the substitution: `lim {x -> a} p(x) = p(a)`. Only factor when direct substitution gives 0/0.
>
> **LIMITS AT INFINITY:**
> For rational functions: divide every term by the highest power of x in the denominator. The 1/x and 1/x^2 terms vanish. The limit is the ratio of leading coefficients (when degrees match), 0 (numerator degree < denominator), or infinity (numerator degree > denominator).
>
> **GEOMETRIC SERIES:**
> State `a` and `r` explicitly. Write `sum = a/(1 - r)`. Show the substitution. Examiners want to see `a` and `r` identified, not just the answer.

---

## ٧. Log Pose

```
0.8 Irrationals --------+
(completeness of R)     |
                        |
0.9 Functions ----------+
(the objects whose      |
limits I take)          v
                 +==================+
                 |  0.10  LIMITS    |  <-- YOU ARE HERE
                 |  The Traveler's  |
                 |  Approach        |
                 +=======+==========+
                         |
                         |  "I can describe what a function
                         |   approaches. Now: how FAST is
                         |   it changing at a single instant?"
                         |
                         v
                 +------------------+
                 |  0.11 DERIVATIVES|
                 |  The Fajr Call   |
                 +------------------+
                         |
                         +--> Arc 3: Numerical Methods
                         |    (bisection uses IVT,
                         |     Newton-Raphson uses derivatives)
                         |
                         +--> Arc 4: Series & Convergence
                              (geometric series -> power series
                               -> Taylor series)

This island unlocks:
  x 0.11 Derivatives — the derivative IS a limit:
    f'(x) = lim {h -> 0} [f(x+h) - f(x)]/h.
    Without limits, the derivative has no foundation.
  x Numerical methods — bisection narrows intervals
    using sign changes (IVT).
  x Series — convergence of infinite sums is DEFINED
    by limits. The geometric series here is the first.

Dependencies satisfied:
  <- 0.9 Functions (the objects whose limits I take)
  <- 0.8 Irrationals (completeness of R — the IVT needs no gaps)
```

---

## ٨. Reflection

The sun is low. Somewhere on the eastern road the traveler is walking. His water-skin is empty and the distance shrinks with every step. The series converges to sixteen miles. He was always going to arrive. I was asking the wrong question — not "when does the distance equal zero?" but "what does the distance approach?"

The limit gives the answer at the edge. The value a function is headed toward, whether or not it arrives. And yet it is no less certain. Name your tolerance, and I will meet it. Every time.

Ten tools. One remains. I can describe what a function approaches. I cannot describe how FAST it is changing at a single instant. Rate is change divided by time. At a single instant, the time interval is zero. Division by zero — forbidden since the qadi's courtyard in Island 0.4.

Unless I take the limit.

Tomorrow at dawn. Young Yusuf — Bilal's apprentice — will stand on the minaret roof alone for the first time. The sky will brighten. He will need to know not where the light is going, but how FAST it is changing — right now, at this instant.

*1 = 1 has not been lost.*

---

*Next: Island 0.11 — Derivatives. Yusuf on the minaret at fajr. The sky brightens. He needs to know how fast the light is changing — not how much, but how fast.*
