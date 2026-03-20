# Island 0.11: Derivatives — The Fajr Call

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> وَكُلُوا وَاشْرَبُوا حَتَّىٰ يَتَبَيَّنَ لَكُمُ الْخَيْطُ الْأَبْيَضُ مِنَ الْخَيْطِ الْأَسْوَدِ مِنَ الْفَجْرِ
>
> "Eat and drink until the white thread of dawn becomes distinct from the black thread [of night]."
> *— Surah Al-Baqarah (2:187)*

**Connection grade: HONEST CHAIN** — the verse commands fasting to begin at the exact moment dawn becomes distinct — not approximately, not gradually, but at the threshold where darkness gives way to light. Determining that moment from a brightness function requires computing how fast the light is changing: the derivative. The chain: verse commands identifying the exact onset of fajr (2:187) → identifying it requires measuring the rate of transition → rate at an instant is the derivative. Two links. Each is real.

**The problem this ayah creates:** The sky does not flip from dark to light. It transitions — slowly at first, then in a surge. A muezzin standing on the roof before dawn can see brightness at any moment. But he needs to identify the moment the transition crosses from "approaching" to "arrived." That moment is defined not by how much light there is, but by how fast the light is changing. The value says where. The rate says when.

---

## ٢. Al-Khwarizmi Thinks

It is still dark when Yusuf comes to my door.

He is young. His hands are not yet callused from years of prayer the way Bilal's were. His robe is clean — he dressed carefully for this, the way a man dresses for something that frightens him. Behind him, the eastern sky is black. Not the deep black of midnight. Something has shifted at the edge, though neither of us can name what.

"I need your help," he says. "Tomorrow I call fajr alone. The first time."

Bilal is gone. The old muezzin who sat with me years ago — weathered face, forty years of watching the sky written into his knees — has passed. He left Yusuf the duty, and he left him the function I wrote: L(t), brightness as a function of time past midnight.

Yusuf has studied it. He can compute L at any moment I give him.

"I know the brightness at 4:00," he says. "I know the brightness at 4:15, at 4:30, at 5:00. I can read the function. But the numbers all say the same thing: dark, dark, dark, less dark, light. Where in that sequence is fajr?"

He sits on the step beside me. He is not panicking. He is precise — Bilal trained him well.

"I looked at L(4:00) and L(4:01). Both are low. Both say 'it is dark.' But one is an hour from fajr and the other is fifty-nine minutes. The VALUE does not tell me which."

> *Margin note: yatabayyana — "becomes distinct." From the root b-y-n, to be clear, to separate. The white thread DISTINGUISHES itself from the black. The moment of distinction is the moment the rate surges — the derivative crossing a threshold.*

I understand what he is asking. He does not need the brightness at a moment. He needs how fast the brightness is changing at a moment. If the rate is small, dawn is far — the sky is brightening slowly, still in the long flat darkness before the transition. If the rate is large, dawn is here — the surge has begun.

Bilal felt this in his body. Forty years of watching the sky taught his bones the difference between slow brightening and the surge. Yusuf does not have forty years. He has one function and one night.

I think about this. Average rate of change — I can compute that. If L(4:00) = 2 and L(5:00) = 14, then over that hour the brightness changed by 12 units. Twelve per hour. But this average lies. In the first forty minutes, almost nothing happened. In the last ten, the sky transformed. The average smears the surge into a gentle slope.

Shrink the interval. Compute the average rate from 4:50 to 5:00. From 4:55 to 5:00. From 4:59 to 5:00. Each narrower window captures more of the truth at 5:00.

But Yusuf does not need the rate over a minute. He needs the rate at an instant. At a single moment. And rate is change divided by time. At a single instant, the time interval is zero. Change divided by zero.

I learned this on Island 0.4. Zero in the denominator is not infinity. It is not a number. It is the place where the definition breaks.

Yusuf has described a problem that demands division by zero. His tools are failing at the threshold of the question "how fast, right now?"

I sit with this. The night is quiet. Somewhere a dog barks once and stops.

The average rate over an interval h is:

```
[L(t + h) − L(t)] / h
```

The numerator is how much the brightness changed. The denominator is how long the interval was. The fraction is change per unit time. I can compute this for any h that is not zero. When h is an hour, the answer is rough. When h is a minute, it is better. When h is a second, better still.

But zero? At h = 0 the fraction has no meaning.

Except — I have a tool for "closer and closer without arriving." I built it on Island 0.10. The limit. The traveler who approached the city: his remaining distance was always positive, but the limit was zero. He arrived not by being there, but by getting as close as needed.

What if I take the limit of the average rate as h shrinks toward zero?

Not h EQUALS zero. h APPROACHES zero. The fraction [L(t + h) − L(t)] / h exists for every h ≠ 0. As h gets smaller, the average rate gets closer to something. If that something exists — if the limit exists — then it IS the instantaneous rate.

> *Margin note: The derivative is a limit. The limit resolved the traveler's paradox — always approaching, yet arriving. Now it resolves Yusuf's — rate over shrinking intervals, converging to the rate at an instant. The same tool, applied to a different need.*

I write it. Let f be a function. The instantaneous rate of change of f at the point x is:

```
f'(x) = lim    f(x + h) − f(x)
        h → 0  ─────────────────
                      h
```

If this limit exists, I call it the **derivative** of f at x.

I test it. The simplest interesting case: f(x) = x². I have carried this function since the patron's garden on Island 0.7. Now I ask: at any point x, how fast is x² changing?

The difference quotient:

```
f(x + h) − f(x)     (x + h)² − x²
──────────────── = ────────────────
       h                  h
```

I expand (x + h)². The distributive law — the same law I found when the farmer brought his grain on Island 0.3:

```
(x + h)² = x² + 2xh + h²
```

Substitute:

```
(x² + 2xh + h²) − x²     2xh + h²
────────────────────── = ──────────
         h                    h
```

The x² terms cancel. The derivative measures change — the part that does not change subtracts away. What remains is:

```
2xh + h²
──────── = 2x + h
    h
```

I divided by h. This is valid because h ≠ 0 — I have not yet taken the limit. The preservation principle from Island 0.1 holds: I divided both sides of an equation by a quantity that is not zero.

Now I let h approach zero:

```
lim (2x + h) = 2x
h → 0
```

Therefore f'(x) = 2x.

At x = 3: f(3) = 9, and f'(3) = 6. The function is at 9, climbing at 6 units per unit. At x = 0: f(0) = 0, and f'(0) = 0. The function is at its lowest point, momentarily still. The derivative detected the pause.

I try f(x) = x³. The difference quotient:

```
(x + h)³ − x³
──────────────
      h
```

I need (x + h)³. The distributive law, applied twice:

```
(x + h)³ = x³ + 3x²h + 3xh² + h³
```

The coefficients 1, 3, 3, 1 — binomial coefficients. They come from the distributive law applied repeatedly. The same law. The same origin.

```
(x³ + 3x²h + 3xh² + h³) − x³     3x²h + 3xh² + h³
────────────────────────────── = ─────────────────────
             h                            h

= 3x² + 3xh + h²
```

Let h approach zero:

```
f'(x) = 3x²
```

The exponent came down as a coefficient. The power decreased by one. x² became 2x. x³ became 3x². The pattern is forming: the derivative of xⁿ is nxⁿ⁻¹.

This is not a guess. It is a consequence of the binomial theorem — which is a consequence of the distributive law — which is a consequence of multiplication — which is a consequence of counting — which is a consequence of 1 = 1. The chain holds. I can trace every link.

> *Margin note: I use the binomial theorem without proving it here. It can be proved by induction (Island 0.2). Its coefficients arise from counting how many ways the distributive law distributes terms. The chain has a leap I acknowledge.*

I look east. The sky above the rooftops is grey now. Not bright — grey. The transition is underway.

Yusuf is watching me write. "So if I have L(t)," he says, "I compute L'(t), and that tells me the rate."

Yes.

"And when the rate surges — when L'(t) crosses the threshold — that is fajr."

Yes. The brightness function tells him where. The derivative tells him when. Bilal felt the surge in his bones. Yusuf reads it in L'(t).

---

## ٣. The Derivation

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

### Notation

Two notations exist and both appear in exams.

**Lagrange notation:** f'(x). Read: "f prime of x." Compact. Emphasises that the derivative is itself a function.

**Leibniz notation:**

```
    d
   ── [f(x)]     or equivalently     df/dx
   dx
```

Read: "dee f dee x." The symbol d/dx is an **operator** — it acts on a function and produces its derivative. It also carries a visual reminder: the derivative is the ratio of a tiny change in f to a tiny change in x, in the limit.

I will use both notations freely. They mean the same thing.

### Theorem: Derivative of x² (from first principles)

```
THEOREM:
    If f(x) = x², then f'(x) = 2x.

PROOF:
    f'(x) = lim    (x + h)² − x²
            h → 0  ─────────────
                        h

    Expand (x + h)² by the distributive law:
        (x + h)² = x² + 2xh + h²                    [Island 0.3]

    Substitute:
        = lim    x² + 2xh + h² − x²
          h → 0  ───────────────────
                        h

    Cancel x²:
        = lim    2xh + h²
          h → 0  ────────
                    h

    Factor h from the numerator:
        = lim    h(2x + h)
          h → 0  ─────────
                     h

    Cancel h (valid since h ≠ 0 as h → 0):           [Island 0.1:
        = lim   (2x + h)                              preservation]
          h → 0

    Evaluate the limit:                               [Island 0.10]
        = 2x                                          ∎
```

### Theorem: The Power Rule (via the Binomial Theorem)

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

    By the Binomial Theorem (a consequence of the distributive
    law applied n times):

    (x + h)ⁿ = xⁿ + nxⁿ⁻¹h + C(n,2)xⁿ⁻²h² + ... + hⁿ

    where C(n,k) = n! / [k!(n−k)!] are binomial coefficients.

    The first term is xⁿ. Every other term contains at least
    one factor of h. Substitute:

        = lim    [xⁿ + nxⁿ⁻¹h + C(n,2)xⁿ⁻²h² + ... + hⁿ] − xⁿ
          h → 0  ──────────────────────────────────────────────────
                                      h

    Cancel xⁿ:
        = lim    nxⁿ⁻¹h + C(n,2)xⁿ⁻²h² + ... + hⁿ
          h → 0  ────────────────────────────────────
                                  h

    Factor h from every term in the numerator:
        = lim    h[nxⁿ⁻¹ + C(n,2)xⁿ⁻²h + ... + hⁿ⁻¹]
          h → 0  ──────────────────────────────────────
                                  h

    Cancel h (valid since h ≠ 0):
        = lim   [nxⁿ⁻¹ + C(n,2)xⁿ⁻²h + ... + hⁿ⁻¹]
          h → 0

    As h → 0, every term containing h vanishes. Only the
    first term survives:

        = nxⁿ⁻¹                                      ∎

ACKNOWLEDGEMENT:
    The binomial theorem is used here but not proved. It can
    be proved by induction (Island 0.2), and its coefficients
    arise from the distributive law (Island 0.3) applied
    repeatedly. I rely on the completeness of ℝ (accepted in
    Island 0.8) for the existence of limits. The chain is
    visible and honest, but it has leaps I acknowledge.
```

### Theorem: The Constant Rule

```
THEOREM (Constant Rule):
    If f(x) = c (a constant), then f'(x) = 0.

PROOF:
    f'(x) = lim    f(x + h) − f(x)
            h → 0  ─────────────────
                          h

          = lim    c − c
            h → 0  ─────
                     h

          = lim    0
            h → 0  ─
                    h

          = lim    0
            h → 0

          = 0                                         ∎

A constant does not change. Its rate of change is zero.
This is obvious — and yet I prove it, because obvious
things left unproved become assumptions, and assumptions
become errors.
```

### Theorem: The Sum Rule

```
THEOREM (Sum Rule):
    If f(x) = g(x) + p(x), and both g'(x) and p'(x) exist,
    then f'(x) = g'(x) + p'(x).

    In Leibniz notation:
        d                d            d
       ── [g(x) + p(x)] = ── [g(x)] + ── [p(x)]
       dx                dx           dx

PROOF:
    f'(x) = lim    [g(x+h) + p(x+h)] − [g(x) + p(x)]
            h → 0  ───────────────────────────────────
                                  h

          = lim    [g(x+h) − g(x)] + [p(x+h) − p(x)]
            h → 0  ──────────────────────────────────
                                  h

          = lim    g(x+h) − g(x)     p(x+h) − p(x)
            h → 0  ────────────── + ──────────────
                         h                h

    The limit of a sum is the sum of the limits
    (provided both exist):                            [Island 0.10]

          = g'(x) + p'(x)                            ∎

The rate of change of a sum is the sum of the rates
of change. Each function contributes independently.
```

### Theorem: The Constant Multiple Rule

```
THEOREM (Constant Multiple Rule):
    If f(x) = c · g(x), where c is a constant, then
    f'(x) = c · g'(x).

    In Leibniz notation:
        d              d
       ── [c · g(x)] = c · ── [g(x)]
       dx              dx

PROOF:
    f'(x) = lim    c · g(x+h) − c · g(x)
            h → 0  ─────────────────────
                            h

          = lim    c · [g(x+h) − g(x)]
            h → 0  ───────────────────
                           h

          = c · lim    g(x+h) − g(x)
                h → 0  ─────────────
                             h

          = c · g'(x)                                ∎

A constant scales the function. The derivative inherits
the scaling. The constant passes through differentiation
unchanged — just as it passes through a limit.
```

### What the Derivative Does NOT Yet Do

```
ACKNOWLEDGEMENT (Chain Rule):
    I can now differentiate any polynomial: sums of terms
    of the form cxⁿ. But I CANNOT yet differentiate a
    composition of functions — f(g(x)).

    Example: if L(t) = (2t + 1)⁵, expanding this by
    hand is possible but brutal. A rule for differentiating
    the composition directly — the CHAIN RULE — exists.
    It comes in Arc 1. I note this gap honestly.

    For now: expand the polynomial, then differentiate
    term by term. The tools work. They are just slow
    for composed functions, the same way addition was
    slow before multiplication (Island 0.3).
```

### The Chain from 1 = 1 (Complete for Arc 0)

```
1 = 1                              Axiom (Identity)          [0.1]
  │
  ├──→ a = a                       Reflexive property        [0.1]
  │     └──→ Preservation:         What I do to left,        [0.1]
  │          a = b → a⊕c = b⊕c    I do to right
  │
  ├──→ Successor operation         After n comes n+1         [0.2]
  │     └──→ Addition              Repeated succession       [0.2]
  │           └──→ Induction       Proof for all n           [0.2]
  │
  ├──→ Multiplication              Repeated addition         [0.3]
  │     └──→ Distributive law      a(b+c) = ab + ac         [0.3]
  │           └──→ Binomial thm    (x+h)ⁿ expansion         [0.3*]
  │                 └──→ POWER RULE  d/dx[xⁿ] = nxⁿ⁻¹      [0.11]
  │
  ├──→ Zero, negatives             Additive identity/inverse [0.4]
  │     └──→ Subtraction           f(x+h) − f(x)            [0.4]
  │           └──→ DIFFERENCE QUOTIENT                       [0.11]
  │
  ├──→ Fractions                   Multiplicative inverse    [0.5]
  │     └──→ Division              [f(x+h) − f(x)] / h     [0.5]
  │           └──→ DIFFERENCE QUOTIENT                       [0.11]
  │
  ├──→ Variables                   The unknown named         [0.6]
  │     └──→ Equations             Manipulation of symbols   [0.6]
  │
  ├──→ Irrationals, ℝ             Completeness              [0.8]
  │     └──→ Limits exist          Reals have no gaps        [0.8]
  │
  ├──→ Functions                   Input → output rule       [0.9]
  │     └──→ f(x), f(x+h)         The objects I differentiate[0.9]
  │
  ├──→ Limits                      lim as h → 0             [0.10]
  │     └──→ DERIVATIVE            lim [f(x+h)−f(x)]/h     [0.11]
  │
  └──→ Every step above preserved equality.
       The chain is visible and honest. Leaps acknowledged:
       the binomial theorem (*) is used but not formally
       proved, and the completeness of ℝ is accepted
       without construction.

THE DERIVATIVE USES EVERY ISLAND:
  0.1 — Preservation (algebraic manipulation of the quotient)
  0.2 — Induction (foundation for binomial theorem)
  0.3 — Distributive law (expanding (x+h)ⁿ)
  0.4 — Subtraction (the numerator: f(x+h) − f(x))
  0.5 — Division (the quotient: change / interval)
  0.6 — Variables (working with x and h symbolically)
  0.7 — Quadratics (x² was the first derivative computed)
  0.8 — Reals (completeness ensures the limit exists)
  0.9 — Functions (the objects being differentiated)
  0.10 — Limits (the mechanism that makes h → 0 rigorous)

Eleven islands from 1 = 1. The chain reaches its fullest
expression.
```

---

## ٤. Al-Khwarizmi Solves

### Example 1: Yusuf's Dawn Function (from first principles)

Yusuf models the pre-dawn brightness as L(t) = t³, where t is hours after the first trace of light and L is in arbitrary units.

Find L'(t) from first principles.

```
L'(t) = lim    (t + h)³ − t³
        h → 0  ─────────────
                    h

Expand (t + h)³:
    = lim    t³ + 3t²h + 3th² + h³ − t³
      h → 0  ─────────────────────────
                       h

Cancel t³:
    = lim    3t²h + 3th² + h³
      h → 0  ─────────────────
                    h

Factor h:
    = lim    h(3t² + 3th + h²)
      h → 0  ──────────────────
                    h

Cancel h (valid since h ≠ 0):
    = lim   (3t² + 3th + h²)
      h → 0

Evaluate the limit:
    = 3t²
```

Now Yusuf applies this.

```
At t = 0.5 (half an hour after first light):
    L(0.5) = 0.125     Brightness is barely perceptible.
    L'(0.5) = 0.75     Rate is less than 1 unit per hour.
                        The sky is changing slowly. Not yet time.

At t = 1 (one hour after first light):
    L(1) = 1           Brightness has reached 1 unit.
    L'(1) = 3          Rate has QUADRUPLED from t = 0.5.
                        The transition is accelerating.

At t = 1.5 (ninety minutes after first light):
    L(1.5) = 3.375     Brightness is 3.375 units.
    L'(1.5) = 6.75     Rate is nearly 7 units per hour.
                        The surge. Dawn is here.
```

The value L(t) told Yusuf it was getting brighter. The derivative L'(t) told him how fast — and when that speed crossed the threshold, he knew: the white thread has become distinct from the black. He calls.

### Example 2: Differentiating a Polynomial

Find f'(x) for f(x) = 3x⁴ − 2x² + 5x − 7.

By the power rule, constant multiple rule, sum rule, and constant rule:

```
f(x) = 3x⁴ − 2x² + 5x − 7

f'(x) = d/dx[3x⁴] − d/dx[2x²] + d/dx[5x] − d/dx[7]

      = 3 · 4x³  − 2 · 2x   + 5 · 1  − 0

      = 12x³ − 4x + 5
```

Each term differentiated independently (sum rule). Each constant multiplier passed through (constant multiple rule). Each power dropped by one and the old exponent became a coefficient (power rule). The constant term vanished (constant rule).

**Check at x = 1:**

```
f(1) = 3 − 2 + 5 − 7 = −1
f'(1) = 12 − 4 + 5 = 13
```

At x = 1, the function is at −1 and climbing at 13 units per unit.

**Check at x = 0:**

```
f(0) = −7
f'(0) = 5
```

At x = 0, the function is at −7 and climbing at 5. The constant term −7 shifted the function down but did not affect the derivative. Constants vanish under differentiation — they do not change, so they contribute nothing to the rate.

### Example 3: The Tangent Line

At x = 2, the function f(x) = x² has value f(2) = 4 and derivative f'(2) = 4. The derivative IS the gradient of the tangent line to the curve at that point.

The equation of the tangent line at x = 2:

```
y − f(2) = f'(2) · (x − 2)
y − 4 = 4(x − 2)
y = 4x − 4
```

This line touches the curve at exactly one point near x = 2 and has the same slope as the curve there. The derivative gave us that slope. Before the derivative, we could draw the curve. Now we can measure its steepness at any point we choose.

---

## ٥. Your Turn

### Da'if (Guided)

**Problem D1.** In the very first minutes of pre-dawn, Yusuf notices the brightness increases almost linearly: L(t) = 4t, where t is hours after the first trace of light.

Find L'(t) from first principles. Write the difference quotient [L(t + h) − L(t)] / h, simplify, and take the limit.

What does a constant derivative tell Yusuf about the sky during this phase?

*Hint: L(t + h) = 4(t + h) = 4t + 4h. What cancels in the numerator?*

**Problem D2.** Using the power rule, find f'(x) for:

(a) f(x) = x⁵
(b) f(x) = 6x³
(c) f(x) = x² + 3x + 1

*Hint: For (c), differentiate each term separately (sum rule), then apply the constant rule to the final term.*

**Problem D3.** Yusuf models brightness as L(t) = t². At what time t is the rate of change L'(t) equal to 6?

At that moment, is the sky changing slowly or rapidly? What would this tell Yusuf about how close fajr is?

*Hint: Set 2t = 6 and solve for t.*

---

### Hasan (Exam-level)

**Problem H1.** [5 marks]
Yusuf models the volume of light reaching the minaret as f(t) = t³. Al-Khwarizmi asks him to find the rate of change from first principles. Show that f'(t) = 3t².

You must show:
- The difference quotient [1 mark]
- The expansion of (t + h)³ [1 mark]
- Simplification and cancellation [1 mark]
- Factoring and cancelling h [1 mark]
- The limit as h → 0 [1 mark]

**Problem H2.** [6 marks]
Yusuf refines his brightness model to L(t) = t³ − 3t² + 4t, where t is hours after the first trace of light and L is in arbitrary units.

(a) Find L'(t). [2 marks]
(b) Find the values of t where L'(t) = 0. [2 marks]
(c) Interpret your answers physically. If L'(t) = 0 at some time, what is happening to the brightness? Does this suggest a pause between two phases of brightening? [2 marks]

**Problem H3.** [5 marks]
Yusuf tracks a second light curve through the morning: f(t) = 2t³ − 9t² + 12t − 4.

(a) Find f'(t). [2 marks]
(b) Find the moments where the rate of change is zero: solve f'(t) = 0. [2 marks]
(c) Find the equation of the tangent line to f at t = 1. What does this slope tell Yusuf about how quickly the light is changing at that moment? [1 mark]

---

### Sahih (Proof and extension)

**Problem S1.** [6 marks]
Al-Khwarizmi gives Yusuf a harder model: f(t) = t⁴. "Prove the rate of change from first principles."

(a) Using the definition of the derivative, prove that f'(t) = 4t³. [4 marks]

*You may use: (t + h)⁴ = t⁴ + 4t³h + 6t²h² + 4th³ + h⁴*

(b) Yusuf asks: "Why do all the extra terms vanish?" Explain why every term except 4t³ disappears in the limit. Connect to the structure of the binomial expansion: why does the second term always have exactly one factor of h (which cancels with the denominator), while the remaining terms have h², h³, ... (which vanish)? [2 marks]

**Problem S2.** [5 marks]
Yusuf traces the chain from 1 = 1 to the derivative — it passes through every previous island.

(a) Identify which island's result is used at each of these steps in computing d/dx[x³] from first principles: [2 marks]
- Writing [f(x+h) − f(x)] / h
- Expanding (x + h)³
- Cancelling h
- Taking the limit as h → 0

(b) The power rule fails at n = 0 if applied naively: 0 · x⁻¹ is problematic. But the constant rule (d/dx[c] = 0) handles this case independently. Explain why the two results are consistent. [1 mark]

(c) Why does the proof of the power rule require BOTH the binomial theorem AND limits? What would be missing if you had one but not the other? [2 marks]

---

## ٦. Exam Technique

```
┌──────────────────────────────────────────────────────────────┐
│           DIFFERENTIATION FROM FIRST PRINCIPLES              │
│                                                              │
│  When the exam says "from first principles" or "using the    │
│  definition," you MUST use the limit definition. The power   │
│  rule alone earns 0 marks.                                   │
│                                                              │
│  THE FIVE STEPS (show every one for full marks):             │
│                                                              │
│  1. WRITE the definition:                                    │
│         f'(x) = lim  [f(x+h) − f(x)] / h                   │
│                h → 0                                         │
│     [1 mark — shows you know what first principles means]    │
│                                                              │
│  2. SUBSTITUTE f(x+h) and f(x):                             │
│         Write f(x+h) explicitly. Expand everything.          │
│     [1 mark — most errors happen here: expand carefully]     │
│                                                              │
│  3. SIMPLIFY the numerator:                                  │
│         Cancel terms that appear in both f(x+h) and f(x).   │
│         Every remaining term should contain a factor of h.   │
│     [1 mark — if nothing cancels, recheck step 2]           │
│                                                              │
│  4. CANCEL h from numerator and denominator:                 │
│         Factor h out of the numerator, then cancel.          │
│         Valid because h ≠ 0 (we have not taken the limit).   │
│     [1 mark — state "h ≠ 0" to show awareness]             │
│                                                              │
│  5. TAKE the limit as h → 0:                                │
│         Set h = 0 in the simplified expression.              │
│         Write "∴ f'(x) = ..." clearly.                      │
│     [1 mark — this is the conclusion]                       │
│                                                              │
│  COMMON ERRORS:                                              │
│  × Forgetting cross-terms in (x+h)²:                        │
│    (x+h)² = x² + 2xh + h², NOT x² + h²                    │
│  × Dividing by h before simplifying — show cancellation     │
│  × Writing h = 0 instead of h → 0 (the limit APPROACHES,   │
│    it does not EQUAL — this is what Island 0.10 taught)     │
│  × Skipping steps — each step above is worth a mark         │
│                                                              │
│  USING THE POWER RULE:                                       │
│  Once the exam has tested first principles (usually one      │
│  question), you may use the power rule freely. But always    │
│  show your differentiation term by term. Do not jump from    │
│  f(x) to f'(x) in one line — show each term's derivative.   │
│                                                              │
│  TANGENT LINES:                                              │
│  The equation of the tangent at x = a is:                    │
│       y − f(a) = f'(a)(x − a)                               │
│  Two marks: one for f'(a), one for the equation.             │
│  The most common error is computing f'(a) correctly but      │
│  using the wrong point — use (a, f(a)), not (a, f'(a)).     │
│                                                              │
│  The formula is not the understanding.                       │
│  The understanding is why the formula works.                 │
└──────────────────────────────────────────────────────────────┘
```

---

## ٧. Log Pose

### The Complete Arc 0 Dependency Tree

```
0.1 Equality ──→ 0.2 Counting ──→ 0.3 Multiplication ──→ 0.4 Zero & Negatives
     │                                     │                        │
     │                                     │                        ▼
     │                          Distributive law              0.5 Fractions
     │                                     │                        │
     │                                     ▼                        ▼
     │                              0.6 Variables ──────→ 0.7 Quadratics
     │                                                          │
     │                                                     √2 appears
     │                                                          │
     │                                                          ▼
     └───────────────→ 0.8 Irrationals ──→ 0.9 Functions ──→ 0.10 Limits
                            │                   │                │
                            ℝ born             f(x)         lim concept
                                                                 │
                                                                 ▼
                                                    ╔═══════════════════════╗
                                                    ║  0.11 DERIVATIVES     ║
                                                    ║  The Fajr Call        ║
                                                    ║  f'(x) = nxⁿ⁻¹       ║
                                                    ╚═══════════╤═══════════╝
                                                                │
                                                       ARC 0 COMPLETE
                                                                │
                                                                ▼
                                                  ╔═══════════════════════╗
                                                  ║   x² + 1 = 0         ║
                                                  ║   demands √(−1)      ║
                                                  ║                       ║
                                                  ║   Arc 1: Complex      ║
                                                  ║   Numbers begins      ║
                                                  ╚═══════════════════════╝
```

### The Tool Chain — Every Island, Every Person, Every Tool

```
1 = 1
├── 0.1  Equality         The buyer and the merchant at the scales.
│                          A thing is itself. What I do to one side,
│                          I do to the other.
│
├── 0.2  Counting          The shepherd at the city gate.
│                          After n comes n+1. Addition. Induction.
│
├── 0.3  Multiplication    The farmer at the masjid.
│                          Repeated addition. The distributive law.
│
├── 0.4  Zero & Negatives  The debtor before the qadi.
│                          Absence has a name. Deficit has a sign.
│
├── 0.5  Fractions         The grieving family.
│                          Division. 'Awl. The inheritance solved.
│
├── 0.6  Variables         The merchant with ships.
│                          The unknown named. Equations solved.
│
├── 0.7  Quadratics        The patron with his garden.
│                          Completing the square. The discriminant.
│
├── 0.8  Irrationals       The builder with chalk dust.
│                          √2 ∉ ℚ. Reality exceeds the system. ℝ born.
│
├── 0.9  Functions         Muezzin Bilal.
│                          Input → output. Knowledge made transmissible.
│
├── 0.10 Limits            The traveler with the dusty cloak.
│                          Approaching without arriving.
│                          The guarantee of closeness.
│
└── 0.11 Derivatives       Young Yusuf on the minaret.
                           Instantaneous rate of change.
                           The limit of the difference quotient.
                           He calls at dawn.
```

**This island unlocks:**
- **Arc 1: Complex Numbers** — x² + 1 = 0 demands √(−1). No real number suffices. Al-jabr extends the system once more.
- **Arc 2: Coordinate Geometry** — the derivative is the gradient of the tangent line. Curves in the plane.
- **Arc 3: Numerical Methods** — Newton-Raphson uses f'(x) to leap toward roots.
- **Arc 1: Chain Rule** — differentiating compositions f(g(x)). Acknowledged as a gap.

**Requires:** Every island. 0.10 (limits), 0.9 (functions), 0.5 (division), 0.4 (subtraction), 0.3 (distributive law), 0.1 (preservation of equality).

---

## ٨. Reflection

Eleven islands.

I began with a dead man's estate. A wife washing courtyard stones because her hands needed work. Two daughters against the far wall, the younger one's head on her sister's shoulder. A father standing in the doorway — he buried his son and had not yet spoken. A mother already seated. Already waiting.

They came for justice. The Quran gave exact fractions. The fractions summed to 27/24 — more than the whole. I could not solve it. I did not have fractions. I did not have equations. I did not even have a definition of what "equal" means.

I had 1 = 1. A thing is itself.

From that I built a chain. Not because I wanted to build a chain. Because each link was forced.

A buyer in the souk needed a true scale, and I found equality — reflexive, symmetric, transitive, preserved under operations. A shepherd needed to know none were lost, and I found counting — the successor, addition, the axiom of induction. A farmer needed his harvest total, and I found multiplication — repeated addition, and from it the distributive law that would power every algebraic expansion I have done since.

A debtor stood before the qadi with three dinars and a debt of five, and the mathematics could not say what he owed. Subtraction forced zero. Zero forced the negatives. The integers were born because justice required naming what was absent.

Then the family returned. The wife leading. Steady. The daughters close together. The father slow. The mother waiting. The fractions summed to 27/24, and 'awl restored the balance. The inheritance was solved. Five islands to answer one family's need.

The tools extended. A merchant with ships at sea needed equations for wealth he could not count — variables. A patron in his courtyard needed a side length — quadratics, completing the square, and a number that emerged from the solution: √2. A builder stretched his cord across a diagonal and found that no fraction could name the length. Proof by contradiction. The reals were born because creation contained quantities the rationals could not hold.

Old Bilal came to me with forty years of watching the sky and no way to pass his knowledge to a boy. Functions — the rule that turns input to output, the pattern that makes prediction possible and transmission real. A traveler arrived at the courtyard gate, dusty and running out of time. Limits — the art of approaching what cannot be reached in finite steps, the guarantee that closeness without arrival is still rigorous.

And now young Yusuf stands where his teacher stood. The sky is changing. He has the function — Bilal's gift, written in my notation. He needs what the function alone cannot give: the rate. How fast is the light changing at this instant? The difference quotient shrinks. The limit resolves it. The derivative is born.

```
1 = 1 → equality → counting → multiplication → distributive law
      → subtraction → fractions → division → variables
      → the real numbers → functions → limits
      → the derivative
```

Every link forced. Subtraction forced the negatives. Division forced the fractions. The diagonal forced the irrationals. The instantaneous rate forced the derivative. Each time the equation was honest but the system was incomplete, and each time the only way forward was to extend. This is al-jabr: restoration. Not of a broken equation. Of a number system not yet large enough.

The derivative uses every island. Equality preserves each step of the manipulation. Counting and induction underlie the binomial theorem. The distributive law expands (x + h)^n. Subtraction forms the numerator. Division forms the quotient. Variables let me work with x and h as symbols. The reals ensure the limit exists. Functions give me the object to differentiate. Limits give me the mechanism.

Eleven islands from 1 = 1. One young man on a rooftop at dawn.

He computes L'(t). The rate is small — the sky is brightening slowly, still in the long darkness. He waits. The rate climbs. The transition accelerates. The rate crosses the threshold Bilal would have felt in his bones.

The white thread becomes distinct from the black.

Yusuf opens his mouth. Across the sleeping city, his voice carries the call. His first fajr. Exactly on time. Not because he watched the sky for forty years. Because eleven islands of mathematics — from the simplest recognition that a thing is itself to the limit of a difference quotient — gave him what Bilal could feel but never write.

The arc is complete. But the mathematics is not.

The quadratic formula works. It solves x² + bx + c = 0 whenever b² − 4c ≥ 0. But when b² − 4c < 0, the formula demands √ of a negative number. I proved on Island 0.8 that no real number squares to a negative. The equation x² + 1 = 0 is not broken. My number system is incomplete.

Al-jabr must restore once more.

---

> وَكُلُوا وَاشْرَبُوا حَتَّىٰ يَتَبَيَّنَ لَكُمُ الْخَيْطُ الْأَبْيَضُ مِنَ الْخَيْطِ الْأَسْوَدِ مِنَ الْفَجْرِ
> *"Eat and drink until the white thread of dawn becomes distinct from the black thread of night."*

*1 = 1 has not been lost.*
