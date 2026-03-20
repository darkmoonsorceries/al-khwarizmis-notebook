# Island 0.2: Counting — The Shepherd's Gate

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> لَّقَدْ أَحْصَاهُمْ وَعَدَّهُمْ عَدًّا
> "He has encompassed them and has counted them, one by one."
> *— Surah Maryam (19:94)*

**Connection grade: HASAN** — The verse speaks of Allah's omniscience: every being in the heavens and earth is known to Him, counted exhaustively, none missed. The primary purpose is theological, not mathematical. But the structure of the act described — عَدًّا, one by one, exhaustive enumeration that misses nothing and counts nothing twice — maps genuinely to the mathematical operation of counting. The shepherd at the gate does not know this verse. He does the same thing with his sheep.

**The problem this ayah creates:** To count is to assign each thing a unique number, miss none, repeat none. What guarantees this process works? What guarantees that after 47 there IS a 48? The shepherd's livelihood depends on the answer.

---

## ٢. Al-Khwarizmi Thinks

I have equality and nothing else.

I can write `a = b`. I know what makes it true — the souk taught me that. A thing is itself. Comparison has no preferred direction. It chains through a common measure. What holds on one side holds on the other.

But `a` and `b` are empty letters. The inheritance demands specific quantities: one-eighth, two-thirds, one-sixth. Four heirs. 2700 dinars. I cannot write any of these. I have a scale with nothing to weigh.

I need numbers.

I go to the city gate at dusk to think, and I find the shepherd there instead.

He is old. His staff is notched — years of use have worn grooves where his hand grips. A dog trails behind him, limping on three legs. The right foreleg is bound with cloth. It cannot run. It cannot chase.

The flock comes through the gate single file. The opening is narrow — one animal at a time. The shepherd stands to the side and touches each one with the end of his staff as it passes. His lips move with each touch.

> *Margin note: His dog cannot chase a stray. If one has wandered, he will not know until the count is done. Every touch of the staff is a question: are you here? The count is all he has.*

I watch him and I think: what is he doing?

He is not adding. He is not multiplying. He is doing something more basic than any operation I can name. Each animal passes. He marks it — not on paper, not with ink, but with a fact. This one is here. This one is here. This one is here.

And between each touch, something happens that he would not be able to explain if I asked. He moves from one number to the next. From the count of what has passed to the count of what has now passed. After the thirty-first sheep, the thirty-second. After the thirty-second, the thirty-third.

But what guarantees the thirty-third exists?

I stop walking. The question is serious. The shepherd takes for granted that after every number there is a next one. So does every merchant in the souk, every scribe in the court. So have I, until this moment. But the inheritance will require me to count heirs, count shares, count dinars. If counting breaks somewhere — if there is a number with no successor, a place where the chain stops — then every sum I build on top of it is built on sand.

What if the shepherd reaches 47 and there is no 48? What if the counting itself has a gap?

The dusk deepens. He is still counting. His hand has not stopped. The flock is large — I count roughly, and there are at least forty animals still moving through the gate. His face is tight. Not with the effort of counting. With the fear of what the count might say.

Because his dog cannot chase. If the count comes up short, he has no way to recover. He cannot send the dog after the stray. He will have to go himself, in the dark, and a shepherd alone at night with a lame dog does not always come back with the missing animal. One lost sheep. That is all it would take.

> *Margin note: The Arabic عَدَّ (adda) means "to count." From the same root: عَدَد (adad), "number." The number IS the count. The act and the object are the same word.*

He does not know I am watching. He does not care. His lips move. His staff touches.

What IS counting? I force myself to answer.

He began with nothing. No sheep had passed. Then one passed, and he had one. Not the symbol "1" — the fact of a single animal on the other side of the gate. One.

Then another. He did not start over. He did not recount the first. He took what he had — one — and he moved to the next. One became two.

The operation is: take a number, produce the next number. Every time. Without exception.

This is the thing I need. Not a list of numbers. A *rule* that generates them. Given any number `n`, there is a next number. I will call it the successor: `S(n)`. The number you reach when one more sheep passes through the gate.

So 1 exists. `S(1) = 2`. `S(2) = 3`. `S(3) = 4`. And on.

But I have to be precise. Three things must be true, or the shepherd's count is worthless:

The chain never loops back. The forty-first sheep is not the first sheep again. If it were, the shepherd would count forty and think he had one. `S(n)` is always *new* — a number that is not any number that came before.

The chain never collapses. If two different numbers had the same successor — if `S(5)` and `S(8)` were both 9 — then counting would conflate different quantities. Two distinct sheep could produce the same count. The shepherd would lose an animal and never know.

The chain never stops. After every number, the successor exists. There is no last number. If someone told me "the numbers end at one thousand," I would count one more sheep and break the claim.

These are not choices. They are requirements. If any of them fails, the shepherd cannot trust his count. If any of them fails, I cannot trust my arithmetic with the inheritance.

One thing more. The deepest one.

The shepherd touches each sheep. One, then the next, then the next. He reaches the end of the flock and knows: every sheep passed. But how does he *know*? He checked the first. He checked that each sheep was followed by the next. And the flock is finite. So every sheep was checked.

This is the principle I need for proofs, not just for sheep. If something is true for 1, and being true for any number means it is true for the next number, then it is true for *all* numbers. The shepherd's method IS this principle. Check the first. Check that each follows from the last. Conclude: all are checked.

I look up. He is almost done. The last animals are passing through. His staff touches each one.

He finishes. He is still for a moment. Then his shoulders drop. He breathes.

Forty-seven. He had forty-seven this morning. He has forty-seven now.

None lost. None miscounted.

Now I can build. The numbers exist — `1, 2, 3, 4, ...` — each one the successor of the last, each one new, the chain never stopping. But counting alone will not solve the inheritance. I need to *combine* counts. How many heirs? Four. How many shares? Four. What is the total? I need addition.

The shepherd's neighbour arrives at the gate with his own flock. Twenty-eight animals. The guard asks: how many total?

I could line up all seventy-one and count from scratch. But that wastes the counting already done. The first shepherd counted to 47. I do not need to undo his work. I start at 47 and count the successor 28 times.

That is what addition is. Not a new operation. Repeated succession.

```
a + 1 = S(a)              (adding one means taking the successor)
a + S(b) = S(a + b)       (adding the next number means the successor of the sum)
```

These two rules and the existence of 1 define every sum. I will never need another definition of addition.

Does the order matter? The first shepherd has 47. The second has 28. Is `47 + 28` the same as `28 + 47`?

I draw it in the dust by the gate. Forty-seven pebbles in a row, then twenty-eight placed end to end. I count: 75. Swap the rows. Count again. 75. The pebbles do not care which row came first.

> *Margin note: When I add the inheritance shares — 1/8 + 2/3 + 1/6 + 1/6 — the order will not matter. I will get 27/24 regardless. The crisis is in the values, not the arrangement.*

One more test. Three shepherds arrive with `a`, `b`, `c` sheep. Combine the first two flocks, then add the third: `(a + b) + c`. Or combine the last two first: `a + (b + c)`. The sheep are the same sheep. The total cannot change because I grouped them differently.

The gate is closed now. The shepherd is walking home, staff across his shoulders, his dog limping beside him. He does not know that what he did — touching each animal, one by one, trusting that the next number exists — is the foundation under every calculation I will ever make.

I know what counting is. I know what addition is. I can prove they work.

Now I need to write it down.

---

## ٣. The Derivation

### Axioms of the Natural Numbers

Five facts. Everything else follows.

**Axiom 1.** 1 is a natural number.
*(1 = 1. Something exists.)*

**Axiom 2.** Every natural number `n` has a unique successor `S(n)` that is also a natural number.
*(After every sheep, there can be another.)*

**Axiom 3.** There is no natural number whose successor is 1.
*(1 is the beginning. Nothing comes before it in N.)*

**Axiom 4.** If `S(m) = S(n)`, then `m = n`.
*(Different sheep produce different counts. The successor never collapses two distinct numbers into one.)*

**Axiom 5 (Induction).** If a property holds for 1, and whenever it holds for `k` it also holds for `S(k)`, then it holds for every natural number.

This is the axiom that lets finite work guarantee infinite truth. I cannot check every natural number — the chain has no end. But if I show the first case holds, and that the step from any number to its successor preserves truth, then ALL cases hold. The base case plants the seed. The inductive step carries it forward without limit.

The shepherd cannot inspect every sheep that will ever be born. But he knows: if the first passes through the gate, and each sheep follows the one before it, then every sheep passes through.

From these five axioms, the natural numbers unfold:

```
1, S(1) = 2, S(2) = 3, S(3) = 4, ...
```

No gaps. No repetitions. No end.

### Definition of Addition

For any natural number `a`:

```
(i)   a + 1 = S(a)
(ii)  a + S(b) = S(a + b)    for any natural number b
```

Rule (i): adding 1 means taking the successor. Rule (ii): adding the successor of `b` is the successor of adding `b`. Together, they reduce any sum to a chain of successor operations.

**Example.** Compute `3 + 2`:

```
3 + 2 = 3 + S(1)          (since 2 = S(1))
      = S(3 + 1)           (by rule ii)
      = S(S(3))            (by rule i)
      = S(4)               (since S(3) = 4)
      = 5                  (since S(4) = 5)
```

Three plus two is five. Not by memorisation — by the successor operation applied twice.

### Theorem 1: Commutativity of Addition

**Claim.** For all natural numbers `a` and `b`: `a + b = b + a`.

**Proof.** Two stages, both by induction.

*Stage 1: Show `a + 1 = 1 + a` for all `a`.*

Base case: `1 + 1 = 1 + 1`. True by reflexivity.

Inductive step: Assume `a + 1 = 1 + a`. Show `S(a) + 1 = 1 + S(a)`.

```
S(a) + 1 = S(S(a))                    (rule i)
1 + S(a) = S(1 + a)                   (rule ii)
         = S(a + 1)                    (by hypothesis: 1 + a = a + 1)
         = S(S(a))                     (rule i)                    ✓
```

*Stage 2: Show `a + b = b + a` for all `a`, `b`.* Fix `a`, induct on `b`.

Base case: `a + 1 = 1 + a`. This is Stage 1.

Inductive step: Assume `a + b = b + a`. Show `a + S(b) = S(b) + a`.

```
a + S(b) = S(a + b)                   (rule ii)
         = S(b + a)                    (by hypothesis)
```

That `S(b + a) = S(b) + a` follows by a subsidiary induction on `a` using rule (ii) and Stage 1. Each step reduces to successor operations.

Therefore `a + b = b + a` for all natural numbers.                    ∎

### Theorem 2: Associativity of Addition

**Claim.** For all natural numbers `a`, `b`, `c`: `(a + b) + c = a + (b + c)`.

**Proof.** By induction on `c`.

Base case (`c = 1`):

```
(a + b) + 1 = S(a + b)                (rule i)
a + (b + 1) = a + S(b)                (rule i)
            = S(a + b)                 (rule ii)
```

Both sides equal `S(a + b)`.                                          ✓

Inductive step: Assume `(a + b) + c = a + (b + c)`. Show `(a + b) + S(c) = a + (b + S(c))`.

```
(a + b) + S(c) = S((a + b) + c)       (rule ii)
               = S(a + (b + c))        (by hypothesis)

a + (b + S(c)) = a + S(b + c)         (rule ii on b + S(c))
               = S(a + (b + c))        (rule ii)
```

Both sides equal `S(a + (b + c))`.                                    ∎

### Summary

| Property | Statement | Meaning |
|----------|-----------|---------|
| Closure | `a + b` is in N | Sum of naturals is natural |
| Commutativity | `a + b = b + a` | Order does not matter |
| Associativity | `(a + b) + c = a + (b + c)` | Grouping does not matter |

### The Chain from 1 = 1

```
1 = 1                     Axiom (from Island 0.1)
  │
  ├──→ 1 is in N           Axiom 1
  │
  ├──→ S(n) exists          Axiom 2 (successor)
  │
  ├──→ S(n) is new          Axioms 3, 4 (no loops)
  │
  ├──→ Induction            Axiom 5 (finite proves infinite)
  │
  ├──→ a + b defined        From successor (rules i, ii)
  │
  ├──→ a + b = b + a        Commutativity (proved by induction)
  │
  └──→ (a+b)+c = a+(b+c)   Associativity (proved by induction)
```

---

## ٤. Al-Khwarizmi Solves

### Example 1: Computing a Sum from Successor Rules

**Problem.** Compute `4 + 3` using only the successor definition.

```
4 + 3 = 4 + S(2)         (since 3 = S(2))
      = S(4 + 2)          (rule ii)
      = S(4 + S(1))       (since 2 = S(1))
      = S(S(4 + 1))       (rule ii)
      = S(S(S(4)))        (rule i)
      = S(S(5))
      = S(6)
      = 7
```

Three applications of the successor — one for each unit in the second number. The definition does not ask me to "just know" that 4 + 3 = 7. It builds the answer one step at a time.

### Example 2: The Shepherd's Full Count

**Problem.** The shepherd counts 47 sheep out in the morning. At dusk he counts them back through the gate. He gets 47. Are they the same 47?

Counting establishes a one-to-one correspondence between sheep and the numbers 1 through 47. In the morning: sheep₁ ↔ 1, sheep₂ ↔ 2, ..., sheep₄₇ ↔ 47. At dusk, the same process yields 47 again.

By Axiom 4, different sheep produce different counts (the successor is injective). By the construction of natural numbers, every number from 1 to 47 is reached exactly once. So 47 out and 47 back means no count was skipped and no count was repeated.

The dog did not need to chase. The count was enough.

### Example 3: Two Flocks, Two Orders

**Problem.** The shepherd has 47 sheep. His neighbour has 28. Compute the total both ways.

```
47 + 28:  start at 47, apply the successor 28 times → 75
28 + 47:  start at 28, apply the successor 47 times → 75
```

By commutativity, these must agree. The total is 75 regardless of which flock is counted first.

In practice, `47 + 28` is faster — fewer successor steps. Commutativity gives me the freedom to choose the more efficient order.

### Example 4: Three Flocks (Associativity in Action)

Three shepherds arrive with 15, 8, and 12 sheep. The gate guard needs the total.

```
Method 1:  (15 + 8) + 12 = 23 + 12 = 35
Method 2:  15 + (8 + 12) = 15 + 20 = 35
Method 3:  (15 + 12) + 8 = 27 + 8 = 35    (commutativity + associativity)
```

Method 2 happens to be easier — `8 + 12 = 20` is a clean number. Associativity guarantees all three methods give the same answer. I am free to choose the grouping that makes the arithmetic simplest.

---

## ٥. Your Turn

### Da'if (Guided)

**Problem D1.** Compute `3 + 4` using only the successor definition. Write out every step.

*Hint: `4 = S(3)`, `3 = S(2)`, `2 = S(1)`. Apply rule (ii) repeatedly, then rule (i).*

**Problem D2.** The shepherd counted 47 sheep this morning. At dusk he counts only 45. He recounts. Still 45.

(a) By which axiom can he be certain that 45 ≠ 47?

(b) How many sheep are missing? Express the answer using the successor function: find the number `m` such that `45 + m = 47`.

*Hint: `45 + S(1) = S(45 + 1) = S(S(45)) = S(46) = 47`. So `m = S(1) = 2`.*

**Problem D3.** Compute `1 + 5` and `5 + 1` separately using successor rules. Verify they give the same result.

*Hint: `5 + 1 = S(5) = 6` by rule (i). For `1 + 5`, you need four applications of rule (ii).*

### Hasan (Exam-level)

**Problem H1.** [4 marks]

Compute `(1 + 2) + 3` and `1 + (2 + 3)` using successor rules. Verify associativity holds. [2 marks per computation]

**Problem H2.** [3 marks]

A shepherd counts his flock every morning and evening. State precisely:

(a) Which axiom guarantees that no two sheep can share the same count? [1 mark]

(b) A second shepherd claims 1 is not a natural number. Which axiom contradicts him? [1 mark]

(c) A third shepherd claims there is a largest natural number. Which axiom contradicts him, and why? [1 mark]

**Problem H3.** [4 marks]

The shepherd's master dies and leaves four heirs. The shepherd must count them to divide the flock. Express "four" as a successor chain starting from 1:

```
1 → S(1) → S(S(1)) → S(S(S(1)))
```

Each heir receives a share. The shares must be counted. Explain why the one-to-one correspondence between heirs and the numbers {1, 2, 3, 4} guarantees that no heir is missed and no heir is counted twice. Reference specific axioms. [4 marks]

### Sahih (Proof and extension)

**Problem S1.** [5 marks]

The shepherd notices a pattern: when he counts sheep into two equal pens, the total is always the count times half the next count. Prove by induction that for all natural numbers `n`:

```
1 + 2 + 3 + ... + n = n × (n + 1) / 2
```

You may use the fact that multiplication and division by 2 are defined (they will be formalised in Island 0.3). State the base case, inductive hypothesis, and inductive step explicitly. [5 marks]

**Problem S2.** [6 marks]

Al-Khwarizmi challenges the shepherd: "What if counting worked differently?" He defines a new operation `⊕` on the natural numbers by:

```
a ⊕ 1 = S(S(a))
a ⊕ S(b) = S(a ⊕ b)
```

(a) Compute `3 ⊕ 2`. [2 marks]

(b) Compute `2 ⊕ 3`. [2 marks]

(c) Is `⊕` commutative? Justify by comparing your answers to (a) and (b). [2 marks]

---

## ٦. Exam Technique

```
┌─────────────────────────────────────────────────────────────────┐
│                   PROOF BY INDUCTION                            │
│                                                                 │
│  Induction follows the shape of the natural numbers.            │
│  A base case and an inductive step together cover               │
│  every natural number. This is Axiom 5 turned into a            │
│  proof technique.                                               │
│                                                                 │
│  THE FOUR-STEP FORMAT (what mark schemes want):                 │
│                                                                 │
│  1. BASE CASE. Show the statement holds for n = 1.              │
│     State both sides. Show they are equal.                      │
│                                                                 │
│  2. ASSUMPTION. Write: "Assume true for n = k."                 │
│     State what you are assuming, explicitly.                     │
│                                                                 │
│  3. INDUCTIVE STEP. Show the statement holds for n = k + 1.     │
│     Use the assumption. Show the algebra.                        │
│                                                                 │
│  4. CONCLUSION. Write: "Therefore, by mathematical induction,   │
│     the statement holds for all n in Z+." Name the method.      │
│     Close the proof.                                            │
│                                                                 │
│  COMMON MISTAKES:                                               │
│  - Forgetting to state the base case (costs 1 mark)             │
│  - Writing the conclusion without naming induction               │
│  - Assuming the result for n = k + 1 (circular reasoning)       │
│  - Skipping algebra in the inductive step                        │
│                                                                 │
│  NOTATION WARNING: Some texts write N = {0,1,2,...},             │
│  others N = {1,2,3,...}. Edexcel uses Z+ for {1,2,3,...}.       │
│  In this notebook, N starts at 1. Zero arrives in Island 0.4.   │
└─────────────────────────────────────────────────────────────────┘
```

---

## ٧. Log Pose

```
 0.1 Equality ──► 0.2 COUNTING ──► 0.3 Multiplication
   (scales)          (gate)            (grain)
    a = a            N, S(n)           repeated
    a = b → b = a   a + b = b + a     addition → a × b

 ┌─────────────────────────────────────┐
 │  This island unlocks:               │
 │  0.3 Multiplication                 │
 │                                     │
 │  "Counting one by one is honest     │
 │   but slow. The farmer has seven    │
 │   fields. Adding one by one will    │
 │   take forever."                    │
 └─────────────────────────────────────┘

 Chain: 1 = 1 ─► Equality ─► Counting ─► ???

 Forward to FP1:
   × Proof by induction (Axiom 5) is a core FP1 technique
   × Summation formulae are proved by induction
   × Recurrence relations use the successor structure
```

---

## ٨. Reflection

Forty-seven went out. Forty-seven came back. The shepherd is home.

He does not know what he gave me. Each touch of his staff was an axiom in motion — the successor exists, the successor is new, the chain never stops. His dog limped beside him and could not chase a single stray. All he had was the count. The count was enough.

I walked from the gate with numbers in my hands. Before tonight, I had equality — a scale with nothing on it. Now the scale has weight. I can place 3 on one side and 3 on the other and know they balance — not because I defined 3 to be 3, but because I built 3 from the ground. 1 exists. `S(1) = 2`. `S(2) = 3`. Each number earned its place through the successor.

The inheritance needs these numbers. How many heirs? Four. How many shares? Four. When I add the shares — 1/8 + 2/3 + 1/6 + 1/6 — commutativity and associativity guarantee the order and grouping do not matter. I will get 27/24 regardless. The problem is in the values, not the arrangement.

But counting one by one is slow. The shepherd counted 47 sheep. It took time, and 47 is a small number. At the masjid tomorrow, a farmer will stand before me with dusty hands and grain in cloth bags. Seven fields, each yielding roughly 100 measures. Zakat is due. He needs the total. Adding 100 seven times is tedious but possible. His neighbour has 23 fields each yielding 47 measures. Adding 47 twenty-three times — the successor applied over five hundred times — is not a count. It is a punishment. He needs a faster tool.

Counting cannot be the end. There must be a shortcut that keeps counting's honesty but not its slowness.

---

> لَّقَدْ أَحْصَاهُمْ وَعَدَّهُمْ عَدًّا
> *He has encompassed them and counted them, one by one.*

*1 = 1 has not been lost.*
