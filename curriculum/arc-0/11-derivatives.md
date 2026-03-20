# Island 0.11: Derivatives — The Fajr Call

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> أَقِمِ الصَّلَاةَ لِدُلُوكِ الشَّمْسِ إِلَىٰ غَسَقِ اللَّيْلِ وَقُرْآنَ الْفَجْرِ ۖ إِنَّ قُرْآنَ الْفَجْرِ كَانَ مَشْهُودًا
> "Establish prayer at the decline of the sun from its meridian to the darkness of the night, and the Quran at dawn. Indeed, the recitation of dawn is ever witnessed."
> *— Surah Al-Isra (17:78)*

**Connection grade: Honest Chain** — The verse prescribes prayer at times defined by transitions: the sun's decline, the onset of darkness, the break of dawn. These are not fixed positions but RATES — moments when the sky shifts from one state to another. Detecting the exact moment of fajr is a rate-of-change problem. Two links: verse commands prayer at dawn → identifying dawn requires detecting the rate at which light surges → rate at an instant is the derivative. Each link is real.

**The problem this ayah creates:** Prayer is commanded at the moment light transitions — not at a position on the brightness curve, but at the inflection where slow brightening becomes a surge. A muezzin who can read the brightness function at any time still cannot call fajr unless he knows how FAST the brightness is changing at a single instant. Value tells where. Rate tells when.

---

## ٢. Al-Khwarizmi Discovers

It is still dark when Yusuf comes to my door.

He is young. His hands are not yet callused from years of prayer. His robe is clean — he dressed carefully for this, the way a man dresses for something that frightens him. Behind him, the eastern sky is black. Not midnight black. Something has shifted at the edge, though neither of us can name what.

"Tomorrow I call fajr alone. The first time."

Bilal is gone. The old muezzin who gave me the function — L(t), brightness over time — has passed. He left Yusuf the duty, and he left him the notation I wrote on Island 0.9. Yusuf has studied it. He can compute L at any moment.

"I know L(4:00)," he says. "I know L(4:15), L(4:30), L(5:00). I can read the function. But the numbers all say the same thing: dark, dark, dark, less dark, light. Where in that sequence is fajr?"

He sits on the step. He is precise — Bilal trained him well.

"I looked at L(4:00) and L(4:01). Both are low. Both say 'it is dark.' But one is an hour from fajr and the other is fifty-nine minutes. The VALUE does not tell me which."

---

I understand. He does not need brightness at a moment. He needs how fast the brightness is changing at a moment. If the rate is small, dawn is far — the sky brightens slowly, still in the long flat darkness before the transition. If the rate is large, dawn is HERE — the surge has begun.

Bilal felt this in his body. Forty years taught his bones the difference between slow brightening and the surge. Yusuf does not have forty years. He has one function and one night.

> *Margin note: yatabayyana — "becomes distinct." From the root b-y-n, to separate. The white thread DISTINGUISHES itself from the black. The moment of distinction is the moment the rate surges.*

I think about average rate. If L(4:00) = 2 and L(5:00) = 14, the brightness changed by 12 over one hour. Twelve per hour. But this average lies. In the first forty minutes, almost nothing happened. In the last ten, the sky transformed. The average smears the surge into a gentle slope.

Shrink the interval. Compute the average from 4:50 to 5:00. From 4:55 to 5:00. From 4:59 to 5:00. Each narrower window captures more truth.

```
Average rate over interval h:

    L(t + h) − L(t)
    ────────────────
          h
```

But Yusuf needs the rate at an INSTANT. At a single moment, the time interval is zero. Change divided by zero.

I learned on Island 0.4: zero in the denominator is not infinity. It is not a number. It is the place where the definition breaks.

---

I sit with this. The night is quiet. Somewhere a dog barks once and stops.

The fraction [L(t + h) − L(t)] / h exists for every h that is not zero. When h is an hour, the answer is rough. When h is a minute, better. When h is a second, better still.

But zero? At h = 0 the fraction has no meaning.

Except — I have a tool for "closer and closer without arriving." I built it on Island 0.10. The traveler approached the city: his remaining distance was always positive, but the limit was zero. He arrived not by being there, but by getting as close as needed.

What if I take the limit of the average rate as h approaches zero?

Not h EQUALS zero. h APPROACHES zero. The fraction exists for every h ≠ 0. As h shrinks, the average rate converges to something. If that something exists — if the limit exists — then it IS the instantaneous rate.

<!-- diagram: light-curve -->

> *A smooth curve of brightness over time. Flat and low on the left. Rising steeply on the right. The surge is visible but unnamed.*

I draw L(t) on my page. A curve. Flat in the darkness, then climbing, then surging upward where dawn breaks.

Two points on the curve: one at time t, another at time t + h. The line through both points is a secant. Its slope is the average rate of change.

<!-- diagram: secant-line -->

> *Two points on the curve. A straight line through both. The slope of this line is the average rate over the interval.*

Now I slide the second point closer to the first. The interval h shrinks. The secant line ROTATES.

<!-- diagram: secant-slides -->

> *The second point slides along the curve toward the first. The secant line pivots. With each step closer, the line adjusts its angle. It is hunting for something.*

As h shrinks, the secant line turns. Not randomly — it converges. The rotation slows. The line settles.

When the second point reaches the first — when h reaches zero — the secant becomes the tangent. The line that touches the curve at exactly one point. Its slope is the instantaneous rate.

<!-- diagram: tangent -->

> *The limit. The secant has become the tangent — one point of contact, one slope. The rate at an instant.*

I write it. Let f be a function. The instantaneous rate of change of f at x is:

```
f'(x) = lim    f(x + h) − f(x)
        h → 0  ─────────────────
                      h
```

If this limit exists, I call it the **derivative** of f at x.

---

I test it. f(x) = x². The function I have carried since the patron's garden on Island 0.7.

```
f(x + h) − f(x)     (x + h)² − x²
──────────────── = ────────────────
       h                  h
```

I expand (x + h)². The distributive law — Island 0.3:

```
(x + h)² = x² + 2xh + h²
```

Substitute:

```
x² + 2xh + h² − x²     2xh + h²
──────────────────── = ──────────
        h                   h
```

The x² terms cancel. What remains has a factor of h:

```
2xh + h²
──────── = 2x + h
    h
```

I divided by h. Valid because h ≠ 0 — I have not yet taken the limit. Preservation from Island 0.1.

Now:

```
lim (2x + h) = 2x
h → 0
```

Therefore f'(x) = 2x.

At x = 3: the function is at 9, climbing at 6. At x = 0: the function is at 0, momentarily still. The derivative detected the pause.

---

I try f(x) = x³.

```
(x + h)³ = x³ + 3x²h + 3xh² + h³
```

The coefficients 1, 3, 3, 1 — binomial coefficients from the distributive law applied twice.

```
(x³ + 3x²h + 3xh² + h³) − x³     3x²h + 3xh² + h³
─────────────────────────── = ─────────────────────
             h                            h

= 3x² + 3xh + h²
```

As h approaches zero:

```
f'(x) = 3x²
```

The exponent came down as coefficient. The power decreased by one. x² became 2x. x³ became 3x². The pattern: the derivative of xⁿ is nxⁿ⁻¹.

This is not a guess. It is a consequence of the binomial theorem — which is a consequence of the distributive law — which is a consequence of multiplication — which is a consequence of counting — which is a consequence of 1 = 1. I can trace every link.

> *Margin note: I use the binomial theorem without proving it. It can be proved by induction (Island 0.2). Its coefficients arise from counting how many ways the distributive law distributes terms. The chain has a leap I acknowledge.*

---

I look east. The sky above the rooftops is grey.

Yusuf is watching me write. "So if I have L(t)," he says, "I compute L'(t), and that tells me the rate."

Yes.

"And when the rate surges — when L'(t) crosses the threshold — that is fajr."

Yes. The brightness function tells him where. The derivative tells him when. Bilal felt the surge in his bones. Yusuf reads it in L'(t).

---

## ٣. The Derivation

### Scholar: Sharaf al-Din al-Tusi (c. 1135–1213 CE, Tus)

Five hundred years before Newton and Leibniz, Sharaf al-Din al-Tusi analyzed cubic equations by defining a function for each cubic and finding its maximum — by setting the derivative to zero. His method was algebraic, not geometric, and he applied it to determine whether a cubic had solutions at all. He used the derivative as a TOOL before the word existed.

---

### Definition: The Derivative

```
DEFINITION (Derivative):
    Let f be a function defined near x. The derivative of f
    at x is:

        f'(x) = lim    f(x + h) − f(x)
                h → 0  ─────────────────
                              h

    provided this limit exists.

    The expression [f(x + h) − f(x)] / h is called the
    DIFFERENCE QUOTIENT. It measures the average rate of
    change of f over the interval from x to x + h.

    The limit transforms the average into the instantaneous.
```

<!-- diagram: formal-first-principles -->

> *The limit definition. The difference quotient on the left. The arrow toward zero. The derivative on the right.*

### Notation

**Lagrange notation:** f'(x). Read: "f prime of x." The derivative is itself a function.

**Leibniz notation:**

```
    d
   ── [f(x)]     or equivalently     df/dx
   dx
```

Read: "dee f dee x." The operator d/dx acts on a function and produces its derivative. It carries a visual reminder: the ratio of a tiny change in f to a tiny change in x, in the limit.

### Theorem: The Power Rule

```
THEOREM (Power Rule):
    If f(x) = xⁿ where n is a positive integer, then:

        d
       ── [xⁿ] = nxⁿ⁻¹
       dx

PROOF:
    f'(x) = lim    (x + h)ⁿ − xⁿ
            h → 0  ─────────────
                        h

    By the Binomial Theorem:

    (x + h)ⁿ = xⁿ + nxⁿ⁻¹h + C(n,2)xⁿ⁻²h² + ... + hⁿ

    Every term after xⁿ contains at least one factor of h.

    Cancel xⁿ:
        = lim    nxⁿ⁻¹h + C(n,2)xⁿ⁻²h² + ... + hⁿ
          h → 0  ────────────────────────────────────
                                  h

    Factor h:
        = lim   [nxⁿ⁻¹ + C(n,2)xⁿ⁻²h + ... + hⁿ⁻¹]
          h → 0

    As h → 0, every term containing h vanishes:

        = nxⁿ⁻¹                                      ∎

ACKNOWLEDGEMENT:
    The binomial theorem is used but not proved. It follows
    from induction (0.2) and the distributive law (0.3).
    The completeness of ℝ (0.8) ensures the limit exists.
    The chain is visible. Leaps acknowledged.
```

<!-- diagram: formal-power-rule -->

> *The power rule. Exponent descends as coefficient. Power decreases by one. The pattern.*

### Theorem: The Constant Rule

```
THEOREM (Constant Rule):
    If f(x) = c (a constant), then f'(x) = 0.

PROOF:
    f'(x) = lim    c − c     = lim  0  = 0          ∎
            h → 0  ─────       h → 0
                     h

A constant does not change. Its rate of change is zero.
```

### Theorem: The Sum Rule

```
THEOREM (Sum Rule):
    If f(x) = g(x) + p(x), and both g'(x) and p'(x) exist,
    then f'(x) = g'(x) + p'(x).

PROOF:
    f'(x) = lim    [g(x+h) + p(x+h)] − [g(x) + p(x)]
            h → 0  ───────────────────────────────────
                                  h

          = lim    g(x+h) − g(x)     p(x+h) − p(x)
            h → 0  ────────────── + ──────────────
                         h                h

    The limit of a sum is the sum of the limits
    (provided both exist):                            [0.10]

          = g'(x) + p'(x)                            ∎
```

### Theorem: The Constant Multiple Rule

```
THEOREM (Constant Multiple Rule):
    If f(x) = c · g(x), then f'(x) = c · g'(x).

PROOF:
    f'(x) = lim    c · [g(x+h) − g(x)]
            h → 0  ───────────────────
                           h

          = c · lim    g(x+h) − g(x)
                h → 0  ─────────────
                             h

          = c · g'(x)                                ∎
```

### The Chain from 1 = 1

```
1 = 1                              Axiom                    [0.1]
  │
  ├──→ Preservation               a = b → a⊕c = b⊕c        [0.1]
  │
  ├──→ Successor, Addition        After n comes n+1          [0.2]
  │     └──→ Induction            Proof for all n            [0.2]
  │
  ├──→ Multiplication             Repeated addition          [0.3]
  │     └──→ Distributive law     a(b+c) = ab + ac          [0.3]
  │           └──→ Binomial thm   (x+h)ⁿ expansion          [0.3*]
  │                 └──→ POWER RULE nxⁿ⁻¹                   [0.11]
  │
  ├──→ Zero, negatives            Additive identity/inverse  [0.4]
  │     └──→ Subtraction          f(x+h) − f(x)             [0.4]
  │
  ├──→ Fractions                  Multiplicative inverse     [0.5]
  │     └──→ Division             [f(x+h) − f(x)] / h      [0.5]
  │
  ├──→ Variables                  The unknown named           [0.6]
  │
  ├──→ Irrationals, ℝ            Completeness               [0.8]
  │     └──→ Limits exist         Reals have no gaps         [0.8]
  │
  ├──→ Functions                  Input → output rule        [0.9]
  │     └──→ f(x), f(x+h)        The objects differentiated [0.9]
  │
  └──→ Limits                    lim as h → 0               [0.10]
        └──→ DERIVATIVE          lim [f(x+h)−f(x)]/h       [0.11]

THE DERIVATIVE USES EVERY ISLAND.
```

---

## ٤. Al-Khwarizmi Solves

### Example 1: Yusuf's Dawn (from first principles)

Yusuf models pre-dawn brightness as L(t) = t³, where t is hours after the first trace of light.

<!-- diagram: example-fajr -->

> *The brightness curve t³. Flat near zero, then surging. Three time points marked: slow, accelerating, surging.*

```
L'(t) = lim    (t + h)³ − t³
        h → 0  ─────────────
                    h

Expand:
    = lim    3t²h + 3th² + h³
      h → 0  ─────────────────
                    h

Factor h:
    = lim   (3t² + 3th + h²)
      h → 0

    = 3t²
```

Now Yusuf reads the sky:

```
At t = 0.5:  L = 0.125   L' = 0.75
             Brightness barely perceptible. Rate < 1. Not yet.

At t = 1:    L = 1        L' = 3
             Rate has quadrupled. Transition accelerating.

At t = 1.5:  L = 3.375    L' = 6.75
             Rate nearly 7. The surge. Dawn is here.
```

The value told Yusuf the sky was getting brighter. The derivative told him WHEN the brightening became the surge. He calls.

### Example 2: Polynomial (power rule applied)

Find f'(x) for f(x) = 3x⁴ − 2x² + 5x − 7.

<!-- diagram: example-power-rule -->

> *Each term differentiated. The exponent descends. The constant vanishes.*

```
f'(x) = d/dx[3x⁴] − d/dx[2x²] + d/dx[5x] − d/dx[7]

      = 3·4x³  − 2·2x   + 5·1  − 0

      = 12x³ − 4x + 5
```

Check at x = 1: f(1) = 3 − 2 + 5 − 7 = −1, and f'(1) = 12 − 4 + 5 = 13. At −1 and climbing at 13.

Check at x = 0: f(0) = −7, and f'(0) = 5. The constant −7 shifted the function down but contributed nothing to the rate. Constants vanish under differentiation.

---

## ٥. Your Turn

### Da'if (Guided)

**Problem D1.** Early in pre-dawn, brightness is nearly linear: L(t) = 4t.

Find L'(t) from first principles. Write the difference quotient [L(t + h) − L(t)] / h, simplify, take the limit.

What does a constant derivative tell Yusuf about the sky?

*Hint: L(t + h) = 4(t + h) = 4t + 4h. What cancels?*

<!-- diagram: ex-daif-tangent -->

> *A straight line. The tangent to a straight line is the line itself. The derivative of a linear function is constant.*

**Problem D2.** Using the power rule, find f'(x) for:

(a) f(x) = x⁵
(b) f(x) = 6x³
(c) f(x) = x² + 3x + 1

*Hint: For (c), differentiate each term separately (sum rule), then apply the constant rule to the final term.*

**Problem D3.** Yusuf models brightness as L(t) = t². At what time is L'(t) = 6?

Is the sky changing slowly or rapidly at that moment?

*Hint: Set 2t = 6.*

### Hasan (Exam-level)

**Problem H1.** [5 marks]
Show from first principles that if f(t) = t³, then f'(t) = 3t².

You must show:
- The difference quotient [1 mark]
- Expansion of (t + h)³ [1 mark]
- Simplification and cancellation [1 mark]
- Factoring and cancelling h [1 mark]
- The limit as h → 0 [1 mark]

<!-- diagram: ex-hasan-first-principles -->

> *The five steps of differentiation from first principles. Each step earns one mark.*

**Problem H2.** [6 marks]
Yusuf refines his model: L(t) = t³ − 3t² + 4t.

(a) Find L'(t). [2 marks]
(b) Solve L'(t) = 0. [2 marks]
(c) Interpret: if L'(t) = 0 at some time, what is happening to the brightness? Does this suggest a pause between two phases of brightening? [2 marks]

**Problem H3.** [5 marks]
A second light curve: f(t) = 2t³ − 9t² + 12t − 4.

(a) Find f'(t). [2 marks]
(b) Solve f'(t) = 0. [2 marks]
(c) Find the tangent line at t = 1. [1 mark]

### Sahih (Proof and extension)

**Problem S1.** [6 marks]
Prove from first principles that if f(t) = t⁴, then f'(t) = 4t³. [4 marks]

*You may use: (t + h)⁴ = t⁴ + 4t³h + 6t²h² + 4th³ + h⁴*

Why does every term except 4t³ vanish in the limit? Connect to the binomial expansion. [2 marks]

**Problem S2.** [5 marks]
Trace the chain from 1 = 1 to d/dx[x³]:

(a) Identify which island's result is used at each step: writing [f(x+h) − f(x)] / h, expanding (x+h)³, cancelling h, taking the limit. [2 marks]

(b) The power rule at n = 0 gives 0 · x⁻¹. The constant rule gives 0. Explain why these are consistent. [1 mark]

(c) Why does the power rule proof require BOTH the binomial theorem AND limits? What is missing if you have one but not the other? [2 marks]

---

## ٦. Exam Technique

> **FIRST PRINCIPLES — the five-mark template:**
>
> When the exam says "from first principles," you MUST use
> the limit definition. The power rule alone earns 0 marks.
>
> **Step 1:** Write the definition.
>     f'(x) = lim [f(x+h) − f(x)] / h           [1 mark]
>
> **Step 2:** Substitute f(x+h) and f(x). Expand.     [1 mark]
>     Most errors happen here. Expand (x+h)² carefully.
>
> **Step 3:** Simplify. Cancel matching terms.          [1 mark]
>     Every surviving term should contain h.
>
> **Step 4:** Factor h. Cancel with denominator.        [1 mark]
>     State "h ≠ 0" to show awareness.
>
> **Step 5:** Take the limit. Set h = 0.               [1 mark]
>     Write the conclusion: "∴ f'(x) = ..."
>
> **Common errors:**
> - (x+h)² = x² + 2xh + h², NOT x² + h²
> - Write h → 0, not h = 0 (the limit APPROACHES)
> - Do not skip steps. Each step above is worth one mark.
>
> **TANGENT LINES:**
>     y − f(a) = f'(a)(x − a)
> Two marks: one for f'(a), one for the equation.
> Use the point (a, f(a)), NOT (a, f'(a)).

---

## ٧. Log Pose

```
0.1 Equality ──→ 0.2 Counting ──→ 0.3 Multiplication ──→ 0.4 Zero
     │                                     │                   │
     │                          Distributive law          0.5 Fractions
     │                                     │                   │
     │                                     ▼                   ▼
     │                              0.6 Variables ──→ 0.7 Quadratics
     │                                                     │
     │                                                √2 appears
     │                                                     │
     │                                                     ▼
     └──────────────→ 0.8 Irrationals ──→ 0.9 Functions ──→ 0.10 Limits
                           │                   │                │
                           ℝ                  f(x)         lim concept
                                                               │
                                                               ▼
                                                  ╔═══════════════════════╗
                                                  ║  0.11 DERIVATIVES     ║
                                                  ║  The Fajr Call        ║
                                                  ║  f'(x) = nxⁿ⁻¹       ║
                                                  ╚═══════════╤═══════════╝
                                                              │
                                                     ARC 0 COMPLETE
```

**This island unlocks:**
- **Arc 1: Complex Numbers** — x² + 1 = 0 demands a number whose square is negative
- **Arc 1: Chain Rule** — differentiating compositions f(g(x))
- **Arc 2: Coordinate Geometry** — the derivative is the gradient of the tangent line
- **Arc 3: Numerical Methods** — Newton-Raphson uses f'(x) to leap toward roots

**Requires:** Every island. 0.10 (limits), 0.9 (functions), 0.5 (division), 0.4 (subtraction), 0.3 (distributive law), 0.1 (preservation).

---

## ٨. Reflection

Eleven islands.

I began with a dead man's estate. A wife washing courtyard stones because her hands needed work. Two daughters against the far wall, the younger one's head on her sister's shoulder. A father standing in the doorway. A mother already seated. Already waiting.

They came for justice. The Quran gave exact fractions. The fractions summed to 27/24 — more than the whole. I could not solve it. I did not have fractions. I did not have equations. I did not even have a definition of what "equal" means.

I had 1 = 1. A thing is itself.

From that I built. Not because I chose to, but because each link was forced.

A buyer in the souk needed a true scale — equality. A shepherd needed to know none were lost — counting. A farmer needed his total — multiplication, and with it the distributive law that would power every expansion I have done since. A debtor stood before the qadi owing more than he held — subtraction forced zero, zero forced the negatives.

Then the family returned. The fractions summed to 27/24, and 'awl restored the balance. Five islands to answer one family's need.

A merchant with ships at sea needed equations for wealth he could not count — variables. A patron needed a side length — quadratics, completing the square, and a number that emerged from the solution: √2. A builder stretched his cord and found that no fraction could name the diagonal. The reals were born because creation contained quantities the rationals could not hold.

Old Bilal came with forty years of watching the sky and no way to pass his knowledge to a boy. Functions — the rule that makes prediction transmissible. A traveler arrived at the gate, dusty and running low on water. Limits — the art of approaching what cannot be reached in finite steps.

And now Yusuf stands where his teacher stood.

He has the function. He needs what the function cannot give: the rate. How fast is the light changing at this instant? The difference quotient shrinks. The limit resolves it. The derivative is born — and it uses EVERY island. Equality preserves each algebraic step. Counting and induction underlie the binomial theorem. The distributive law expands (x + h)ⁿ. Subtraction forms the numerator. Division forms the quotient. Variables let me work with x and h as symbols. The reals ensure the limit exists. Functions give me the object. Limits give me the mechanism.

```
1 = 1 → equality → counting → multiplication → distributive law
      → subtraction → fractions → division → variables
      → the real numbers → functions → limits
      → the derivative
```

Eleven islands from 1 = 1. One young man on a rooftop at dawn.

He computes L'(t). The rate is small. He waits. The rate climbs. The transition accelerates. The rate crosses the threshold Bilal would have felt in his bones.

The white thread becomes distinct from the black.

Yusuf opens his mouth. Across the sleeping city, his voice carries the call. His first fajr. Exactly on time.

---

The arc is complete. But the mathematics is not.

The quadratic formula solves x² + bx + c = 0 whenever b² − 4c ≥ 0. But when b² − 4c < 0, the formula demands the square root of a negative number. I proved on Island 0.8 that no real number squares to a negative. The equation x² + 1 = 0 is not broken. My number system is incomplete.

I open a book the English will one day call Further Mathematics. But that is another journey.

The fajr call has been made. The silence after is the space where the next journey begins.

---

> أَقِمِ الصَّلَاةَ لِدُلُوكِ الشَّمْسِ إِلَىٰ غَسَقِ اللَّيْلِ وَقُرْآنَ الْفَجْرِ ۖ إِنَّ قُرْآنَ الْفَجْرِ كَانَ مَشْهُودًا
> *"Establish prayer at the decline of the sun from its meridian to the darkness of the night, and the Quran at dawn. Indeed, the recitation of dawn is ever witnessed."*

*1 = 1 has not been lost.*

---
