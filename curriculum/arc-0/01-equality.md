# Island 0.1: Equality — The Scales

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> وَنَضَعُ الْمَوَازِينَ الْقِسْطَ لِيَوْمِ الْقِيَامَةِ فَلَا تُظْلَمُ نَفْسٌ شَيْئًا
> "And We place the scales of justice for the Day of Resurrection,
> so no soul will be treated unjustly at all."
> *— Surah Al-Anbiya (21:47)*

**Connection grade: Hasan** — The verse is about divine justice on
the Day of Judgement. Its primary meaning is theological, not
mathematical. But the STRUCTURE of a just scale — what makes it
true, what makes it false — genuinely maps to the axioms of
equality. The verse is not about mathematics. The mathematics
is in the verse's structure.

**The problem this ayah creates:** If God promises scales of
justice, then a scale must be either true or false. What makes
a scale TRUE? What properties must it have so that no soul is
wronged? Answer that, and you have defined equality.

---

## ٢. Al-Khwarizmi Discovers

I have written it.

"Wife's share = 1/8."

I stop. The ink is still wet on the paper. I stare at the mark
between "share" and "1/8." The two small lines, one on top of
the other.

What does that mark mean?

I have used it. I have always used it. Every scribe uses it.
But I cannot tell you what it IS. If a man asked me — "what
does it mean for two things to be equal?" — I would point at
a scale. Everyone would point at a scale.

Fine. I will go to the souk and look at one.

---

The saffron merchant has the best scale in the souk. Polished
brass pans, a beam of dark wood, a fulcrum filed to a point
so fine you could prick your finger on it. He is proud of this
scale. He should be. His customers trust it more than they
trust him.

But today there is a problem. A buyer stands with his arms
crossed. He has purchased saffron — three dirhams' worth — and
he does not believe the weight is honest.

"Your weights are false," the buyer says.

"My weights are certified by the muhtasib," the merchant says.

They both stare at the scale.

I stare at the scale.

<!-- diagram: empty-scale -->

> *An empty scale. The beam is level. Nothing is being weighed.
> But the argument is already here: what makes this scale TRUE?*

Neither man can answer the question. The buyer says the weights
are wrong. The merchant says they are right. They are arguing
about the ANSWER. I am staring at the INSTRUMENT.

What must be true about this scale — about ANY scale — for it
to deserve the trust these men place in it?

---

I take a brass weight from the merchant's set. It is cold and
heavy in my palm. I place it on the left pan. The beam tilts.
Obviously. One side is loaded, the other empty.

Now I take an identical weight — same brass, same stamp, same
muhtasib's mark — and place it on the right pan.

The beam levels.

<!-- diagram: reflexive -->

> *The same weight on both sides. The beam is level.*

This is not a discovery. A child knows this. But I write it
down because I am trying to build from nothing, and even
obvious things must be said once.

> `a = a`
>
> A thing is equal to itself.

This is reflexive. The weight is what it is. The number 3 is 3.
The wife's share is the wife's share. I cannot build anything
if this is not solid ground.

> *Margin note: 1 = 1. This is where the ground was laid.
> Everything I build will stand on this.*

---

Now I try something. I reach across the scale and swap the
pans — I lift the left weight and set it on the right, lift
the right weight and set it on the left.

The beam tilts during the swap. For a moment, everything is
wrong. Then I place the second weight, and—

The beam levels again.

<!-- diagram: symmetric -->

> *The weights swapped sides. The beam returns to level.
> The NAMES changed. The TRUTH did not.*

Why should this work? Because the scale does not know which
side is "left" and which is "right." The scale knows only
weight. If the left pan holds the same weight as the right,
then the right holds the same weight as the left.

> `if a = b, then b = a`
>
> Equality is symmetric.

This is the property the buyer is relying on. He says: "if
your weight equals my saffron, then my saffron equals your
weight." He wants to put the saffron on the OTHER pan and
check. The merchant cannot refuse — symmetry is not a
courtesy. It is a law.

---

The buyer's neighbor has been watching. He leans in. "I bought
from the same merchant yesterday. My saffron weighed the same
as yours."

Now there are three quantities. The buyer's saffron. The
neighbor's saffron. And the merchant's weight.

The merchant's weight balanced the buyer's saffron. The
neighbor says his saffron balanced the buyer's. So the
merchant's weight should balance the neighbor's saffron too.

Should it?

I try. I place the merchant's weight on the left. The
neighbor's saffron on the right.

<!-- diagram: transitive -->

> *If A equals B, and B equals C, does A equal C?*

The beam levels.

> `if a = b and b = c, then a = c`
>
> Equality is transitive.

This is the property that lets chains of reasoning WORK. If I
know my weight equals the standard, and the standard equals
yours, then my weight equals yours — without us ever
comparing them directly. The chain carries the truth.

If this property failed, every transaction in the souk would
require starting from scratch. No standard could be trusted
past one use. Commerce would be impossible. Justice would be
impossible.

---

One more. The buyer says: "Add one dirham to each side."

He places a small coin on the left pan. I place an identical
coin on the right.

<!-- diagram: preservation -->

> *Equal weight added to both sides. The beam does not move.*

> `if a = b, then a + c = b + c`
>
> Equality is preserved under equal operations.

This is the most powerful of the four. It means I can DO things
to both sides of an equation — add, subtract, multiply, divide
— and if I do the SAME thing to both sides, the equality holds.

This is how equations will be solved. Not today. But soon. The
merchant with ships at sea will need this. The patron with his
garden will need this. Every equation I will ever write depends
on this property.

The buyer nods. The merchant nods. They have not resolved their
dispute about the saffron. But they have agreed on something
deeper: the scale itself is true.

---

## ٣. The Derivation

Four properties define equality. I state them now without
story, for the student who wants them clean.

**Definition.** A relation `=` on a set S is an *equality*
if and only if it satisfies:

**Property 1 — Reflexive**

```
For all a in S:  a = a
```

A thing is itself.

<!-- diagram: formal-reflexive -->

**Property 2 — Symmetric**

```
For all a, b in S:  if a = b then b = a
```

Direction does not matter.

<!-- diagram: formal-symmetric -->

**Property 3 — Transitive**

```
For all a, b, c in S:  if a = b and b = c then a = c
```

Chains carry truth.

<!-- diagram: formal-transitive -->

**Property 4 — Preservation (Substitution)**

```
For all a, b, c in S:  if a = b then a + c = b + c
```

Equal operations on equal quantities yield equal results.

<!-- diagram: formal-preservation -->

> **The chain from 1 = 1:**
> 1 = 1 (axiom) → reflexive (a thing is itself) →
> symmetric (direction doesn't matter) → transitive
> (chains work) → preservation (operations are safe)

**Geometry spec for Layer (Mode A):**
Five frames. Empty tilted beam → reflexive (same weights,
level) → symmetric (swap, still level) → transitive (chain
verified) → preservation (add to both, still level). Final
frame: fulcrum glows gold. The scale is true.

---

## ٤. Al-Khwarizmi Solves

**Example 1: The buyer's saffron**

The buyer purchased 3 dirhams of saffron. He wants to verify
the weight. The merchant's certified weight is on the left.

<!-- diagram: example-saffron -->

**Example 2: The inheritance equation**

From the prologue: wife's share = 1/8 of the estate.

<!-- diagram: example-inheritance -->

> *Margin note: I cannot solve this yet. I need fractions
> (Island 0.5). But I can WRITE it, because equality lets
> me. The tool to write came before the tool to compute.*

**Example 3: Checking your own work**

A student writes:  `7 + 5 = 13`

Test with Property 1 (reflexive):

<!-- diagram: example-check -->

The student's claim fails. The scale tilts. This is how
every "check your answer" works — compute both sides, test
if they are the same number (reflexive).

---

## ٥. Your Turn

### Da'if (Guided)

**1.** The merchant has three sets of weights: A, B, and C.
He knows A = B (they balance on the scale). He knows
B = C (they also balance). Does A = C? Which property
guarantees this?

<!-- diagram: ex-daif-1 -->

*Hint: This is the chain property.*

**2.** If `x = 5`, what is `x + 3`? Which property of
equality lets you compute this?

<!-- diagram: ex-daif-2 -->

*Hint: You are doing the same thing (+3) to both sides
of x = 5.*

**3.** A student writes `a = b`. Another student writes
`b = a`. Are both correct? Why?

### Hasan (Exam-level)

**4.** Prove that if `a = b` and `c = d`, then
`a + c = b + d`. [3 marks]

*Use Property 4 twice.*

**5.** The muhtasib tests scales by placing a 100-dirham
standard weight on both sides. If the beam levels, the
scale is certified. Which property is he testing, and
why is this test necessary but not sufficient? [4 marks]

**6.** Given that `2x + 1 = 9`, find `x` by applying
Property 4 (preservation) at each step. Show each
application explicitly. [3 marks]

<!-- diagram: ex-hasan-6 -->

### Sahih (Proof and extension)

**7.** The four properties of equality are sometimes
called an "equivalence relation" (Properties 1-3) plus
"congruence" (Property 4). Prove that if `=` is an
equivalence relation, then for any `a`: the set
`{x : x = a}` contains at least one element. [3 marks]

*Hint: Which property guarantees `a` is in its own
equivalence class?*

**8.** A broken scale always tilts left by 1 unit. That
is, when you place weight `a` on the left and weight `b`
on the right, the scale reads `a + 1 = b` instead of
`a = b`. Which properties of equality does this broken
scale violate? Prove your answer. [5 marks]

<!-- diagram: ex-sahih-8 -->

---

## ٦. Exam Technique

> **What mark schemes want for "prove" questions:**
>
> 1. State what you assume (1 mark)
> 2. Apply a known property or theorem (1 mark)
> 3. Conclude with what you've shown (1 mark)
>
> **Common mistake:** Assuming what you're trying to prove.
> "Let a = b. Then a = b." This proves nothing — it uses
> reflexive where you needed to DERIVE the result.
>
> **The equality chain trick:** When asked to show that
> `expression₁ = expression₄`, build a chain:
> `expression₁ = expression₂ = expression₃ = expression₄`
> Each step uses one property. Markers award one mark per
> valid step. More steps = more marks, IF each step is correct.

---

## ٧. Log Pose

```
                    ┌──────────┐
                    │ Prologue │
                    │ 1 = 1    │
                    └────┬─────┘
                         │
                    ┌────▼─────┐
              ┌─────┤ 0.1 ═══ ├─────┐
              │     │ Equality │     │
              │     └────┬─────┘     │
              │          │           │
         ┌────▼───┐ ┌───▼────┐ ┌───▼────┐
         │  0.2   │ │  0.6   │ │  FP1   │
         │ Count  │ │ Vars   │ │ Ch.1   │
         └────────┘ │ (uses  │ │ proof  │
                    │  = to  │ │ by =)  │
                    │ solve) │ └────────┘
                    └────────┘
```

**This island unlocks:**
- 0.2 (Counting) — needs equality to define "the same number"
- 0.6 (Variables) — solving equations uses Property 4 repeatedly
- FP1 Chapter 1 (Proof) — proof by equality chains

---

## ٨. Reflection

The buyer paid for his saffron. Three dirhams. He was satisfied
— not because the merchant was honest, but because the scale was
true. A true scale does not take sides.

I sit in my workshop and write the four properties on a clean
sheet. Reflexive. Symmetric. Transitive. Preservation. Four
words. But they carry the weight of every transaction in the
souk, every contract before the qadi, every equation I will
ever write.

And they rest on one line:

`1 = 1`

A thing is itself. This cannot be denied without using it. It
is the ground.

Tomorrow a shepherd will come through the gate with his flock.
He will touch each animal as it passes. One, then another, then
another. He will count.

But what IS counting? I have equality — I know what it means
for two things to be the same. But I have nothing to BE equal.
No numbers. No "one." No "two." I need something to count WITH.

I watch the gate from my window. The shepherd is already there.
His dog limps beside him. The sun is going down.

*1 = 1 has not been lost.*

---
