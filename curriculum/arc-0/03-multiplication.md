# Island 0.3: Multiplication — The Farmer's Grain

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> مَّثَلُ الَّذِينَ يُنفِقُونَ أَمْوَالَهُمْ فِي سَبِيلِ اللَّهِ كَمَثَلِ حَبَّةٍ أَنبَتَتْ سَبْعَ سَنَابِلَ فِي كُلِّ سُنبُلَةٍ مِّائَةُ حَبَّةٍ ۗ وَاللَّهُ يُضَاعِفُ لِمَن يَشَاءُ ۗ وَاللَّهُ وَاسِعٌ عَلِيمٌ
> "The example of those who spend their wealth in the way of Allah
> is like a seed of grain that grows seven ears; in each ear is a
> hundred grains. And Allah multiplies for whom He wills. And Allah
> is all-Encompassing and Knowing."
> *— Surah Al-Baqarah (2:261)*

**Connection grade: Hasan** — The verse is about spiritual reward for charity. Its primary purpose is to encourage spending in the way of Allah. But the STRUCTURE is explicitly multiplicative: one seed, seven ears, a hundred grains per ear. The Arabic *yuda'ifu* — "He multiplies" — names the operation. The number IS in the verse: 1 × 7 × 100 = 700. Stronger than typical Hasan — borderline Sahih — but the verse's point is generosity, not arithmetic.

**The problem this ayah creates:** A farmer has fields of grain. Zakat is due at the harvest. He must know his total. Seven fields, roughly a hundred measures each — he could add. But his neighbor has twenty-three fields at forty-seven measures each. Adding forty-seven twenty-three times is not a method. It is punishment. Two of the farmer's fields were damaged by locusts. The harvest is not uniform. He needs a tool that addition alone cannot provide.

---

## ٢. Al-Khwarizmi Discovers

A farmer is waiting for me at the masjid after Dhuhr.

He has come early. His hands are cracked at the knuckles. His robe carries dust from the threshing floor and he has not changed it — he came straight from the fields. Beside him on the stone bench sit two cloth bags, heavy with grain. Samples from his harvest. The zakat collector comes in six days.

He needs a number.

"Each field gave roughly a hundred measures," he says. "Seven fields. I need the total."

I write it:

```
100 + 100 + 100 + 100 + 100 + 100 + 100
```

Seven terms. I add. Seven hundred measures. The farmer nods. He knew that already — he could feel seven hundred in the weight of the season. But he needed it written.

Then he leans forward. "My neighbor Ibrahim — he has twenty-three fields. Each one gave forty-seven measures. He asked me to help him count."

Twenty-three fields. Forty-seven measures each.

I would need to write:

```
47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47 + 47
```

Twenty-three terms. Each addition is a place where I can make an error. One slip and the total is wrong, and Ibrahim pays the wrong zakat — either cheating himself or cheating the poor.

I stare at the line. Addition works. Addition is correct. But addition does not SCALE. The tool is honest and slow, like counting sheep one by one through a gate. For seven fields it is tolerable. For twenty-three it is miserable. For a merchant with a hundred transactions it is impossible.

> *Margin note: The tool is not wrong. It is insufficient. This is different from the souk, where I needed a new concept (equality). Here I have the right concept (addition) but the wrong speed. The problem is not WHAT I compute — it is how long the computation takes.*

---

I sit with this. The structure of the problem is: *the same quantity, repeated many times*. That is what "seven fields at a hundred measures" means. It is not seven different numbers being added. It is the same number, added to itself, again and again.

The imam recited the grain verse at Jumu'ah last week. One seed. Seven ears. A hundred grains per ear. The Quran does not say "a hundred grains, and a hundred grains, and a hundred grains, and a hundred grains, and a hundred grains, and a hundred grains, and a hundred grains." It says: seven ears. A hundred each. The repetition is named, not performed.

I need a way to write: "`a` added to itself `b` times" — without writing it `b` times.

I will call it **multiplication**. I write it with this mark: ×.

```
a × b = a + a + a + ... + a     (b times)
```

The farmer's harvest: `100 × 7 = 700`. Ibrahim's harvest: `47 × 23`. One line instead of twenty-three.

But I have only named the shortcut. I have not understood what it DOES.

---

I pick up a handful of pebbles from the masjid courtyard. I lay them out. Four rows. Three in each row.

<!-- diagram: grid -->

```
● ● ●
● ● ●
● ● ●
● ● ●
```

> *Twelve pebbles. Four rows of three.*

Twelve pebbles. Four groups of three: `3 × 4 = 12`.

I stand. I walk to the other side of the arrangement and look again. From here, I see three rows of four.

<!-- diagram: rows-vs-columns -->

```
● ● ● ●
● ● ● ●
● ● ● ●
```

> *The same twelve pebbles. Three rows of four.*

`4 × 3 = 12`.

The pebbles did not move. I moved. The count is the same from both sides. Whether I say "four groups of three" or "three groups of four," the total is twelve.

> *Margin note: The rectangle. Walk around it and the rows become columns. The pebbles do not care which direction I count. This is why `a × b = b × a`.*

So `7 × 100 = 100 × 7`. The farmer could count seven groups of a hundred, or a hundred groups of seven. Same total. The field does not care which way he walks through it.

This matters for Ibrahim. `47 × 23 = 23 × 47`. If adding forty-seven twenty-three times is miserable, he could instead add twenty-three forty-seven times. Still miserable — but the CHOICE exists. The operation does not depend on which number comes first.

I write: **`a × b = b × a`**. The commutative law of multiplication.

---

Now the ayah. One seed, seven ears, a hundred grains per ear. That is `1 × 7 × 100`. Three numbers chained. Does it matter how I group them?

`(1 × 7) × 100 = 7 × 100 = 700`.

`1 × (7 × 100) = 1 × 700 = 700`.

Same answer. The grouping does not matter. I think of the pebble rectangle extended into depth — a box of pebbles, layers stacked. However I slice the box, I count the same objects.

**`(a × b) × c = a × (b × c)`**. The associative law.

And one thing more. `a × 1`. One group of `a`. That is just `a`. The number 1 — the same 1 from which everything began — passes through multiplication unchanged. `a × 1 = a`. The multiplicative identity.

---

The farmer is not finished. "Two of my fields had damage," he says. "Locusts. Those two gave only eighty measures, not a hundred."

So his real harvest is: five fields at a hundred measures, and two fields at eighty.

```
100 + 100 + 100 + 100 + 100 + 80 + 80
```

I add. Five hundreds is five hundred. Eighty and eighty is a hundred and sixty. Five hundred and a hundred and sixty. Six hundred and sixty. Seven terms is manageable.

But what about Ibrahim's version? Eight of his twenty-three fields damaged. I would need to add forty-seven fifteen times, then some smaller number eight times, then combine. The line of additions would sprawl across the page.

I think about the farmer's five good fields. `100 × 5`. His two damaged fields. `80 × 2`. The total: `100 × 5 + 80 × 2`.

But suppose all seven fields had been the same yield — say all seven gave `a` measures. Then:

```
a × 5 + a × 2 = a × 7
```

> *Margin note: Five groups of `a` combined with two groups of `a` gives seven groups of `a`. This is not new arithmetic — it is the meaning of "five plus two equals seven" applied to groups.*

This means: `a × 5 + a × 2 = a × (5 + 2)`. I can split or combine groups freely.

I test it with small numbers. Is `(4 + 3) × 2` the same as `4 × 2 + 3 × 2`?

`(4 + 3) × 2 = 7 × 2 = 14`.

`4 × 2 + 3 × 2 = 8 + 6 = 14`.

Yes.

---

I go back to the pebbles. I lay out `(4 + 3) × 2` as a rectangle: two columns, seven rows. But I draw a line between the fourth and fifth rows.

<!-- diagram: distributive -->

```
● ●  ┐
● ●  │ 4 × 2
● ●  │
● ●  ┘
-----
● ●  ┐
● ●  │ 3 × 2
● ●  ┘
```

> *The rectangle split. Four-by-two above the line. Three-by-two below. Total area unchanged.*

The rectangle is one shape. The line divides it into two sub-rectangles. The total pebbles — fourteen — are the same whether I count the whole rectangle or add the two parts.

The multiplication reaches inside the addition and touches each part separately.

**`a × (b + c) = a × b + a × c`**

The distributive law.

Now I can compute Ibrahim's harvest without adding forty-seven twenty-three times:

```
47 × 23 = 47 × (20 + 3)
        = 47 × 20 + 47 × 3
        = (40 + 7) × 20 + (40 + 7) × 3
        = 40 × 20 + 7 × 20 + 40 × 3 + 7 × 3
        = 800 + 140 + 120 + 21
        = 1081
```

Five lines. Not twenty-three additions. The distributive law did this — broke the problem into pieces I could handle, then let me combine the results.

---

The farmer watches me write. "That is what Ibrahim needs?"

"One thousand and eighty-one measures," I say.

"And my total? Six hundred and sixty?"

"Six hundred and sixty."

"Then the zakat is one-fortieth of six hundred and sixty." He pauses. "What is one-fortieth of six hundred and sixty?"

I try. `16 × 40 = 640`. Not enough. `17 × 40 = 680`. Too much. The answer is between sixteen and seventeen. It is not a whole number.

I do not have a tool for this. I can multiply. I can add. But I cannot split a whole number into forty equal parts when the split does not come out even.

"I will have your answer," I tell him. "Not today."

He picks up his grain bags. He will come back.

---

## ٣. The Derivation

I build from what I have. Equality from Island 0.1. Addition from Island 0.2.

### Definition

For natural numbers `a` and `b`:

```
a × b = a + a + a + ... + a     (b times)
```

This is a definition, not an assumption. I name a process I already understand: repeated addition.

### Property 1: Multiplicative Identity

**Claim:** `a × 1 = a`

**Proof:** By definition, `a × 1` means one copy of `a`. One copy of `a` is `a`. ∎

By commutativity: `1 × a = 1 + 1 + ... + 1` (`a` times) `= a`.

The number 1 is the **multiplicative identity**. It passes through multiplication unchanged — the same 1 from which counting began.

### Property 2: Commutative Law

**Claim:** `a × b = b × a`

<!-- diagram: formal-commutative -->

**Proof (rectangle argument):**

Arrange `a × b` objects in a grid: `b` rows of `a` objects. The total is `a × b`.

Read the same grid by columns: `a` columns of `b` objects. The total is `b × a`.

No object was added or removed. The grid is unchanged. By the reflexive property of equality (Island 0.1):

```
a × b = b × a    ∎
```

**Geometry spec:** A grid of `a` columns and `b` rows. First, gold brackets group rows (count by rows = `a × b`). Then brackets shift to teal, grouping columns (count by columns = `b × a`). The grid does not move. Only the grouping changes.

### Property 3: Associative Law

**Claim:** `(a × b) × c = a × (b × c)`

**Proof (box argument):**

Arrange `a × b × c` objects in a three-dimensional grid: `c` layers, each a rectangle of `a × b`.

- Left grouping: compute `a × b` per layer, then multiply by `c` layers. Total: `(a × b) × c`.
- Right grouping: compute `b × c` (a column through all layers), then multiply by `a` such columns. Total: `a × (b × c)`.

Both groupings count every object exactly once. The box is unchanged.

```
(a × b) × c = a × (b × c)    ∎
```

This is why the grain verse resolves regardless of grouping:

```
(1 × 7) × 100 = 1 × (7 × 100) = 700
```

### Property 4: Distributive Law

**Claim:** `a × (b + c) = a × b + a × c`

<!-- diagram: formal-distributive -->

**Proof:**

By definition:

```
a × (b + c) = a + a + ... + a     ((b + c) times)
```

This is `a` written `(b + c)` times. By the associative property of addition (Island 0.2), group the first `b` copies and the remaining `c` copies:

```
= [a + a + ... + a] + [a + a + ... + a]
       (b times)           (c times)
```

By definition, the first group is `a × b` and the second is `a × c`:

```
= a × b + a × c    ∎
```

By commutativity: `(b + c) × a = b × a + c × a`.

The reverse direction — `a × b + a × c = a × (b + c)` — is **factoring**. Same law, read backward.

**Geometry spec:** A rectangle of width `a` and height `(b + c)`. A horizontal line splits it into two sub-rectangles: width `a`, heights `b` and `c`. The top sub-rectangle glows gold (area `a × b`). The bottom glows teal (area `a × c`). Total area: `a × b + a × c = a × (b + c)`.

### Summary of Laws

| Law | Statement | Proof method |
|-----|-----------|--------------|
| Identity | `a × 1 = a` | Definition |
| Commutativity | `a × b = b × a` | Rectangle argument |
| Associativity | `(a × b) × c = a × (b × c)` | Box argument |
| Distributivity | `a × (b + c) = a × b + a × c` | Grouping repeated addition |

**The chain from 1 = 1:**

```
1 = 1                                    (axiom)
├── Equality: reflexive, symmetric,
│   transitive, preservation             (Island 0.1)
├── Counting: successor, addition,
│   commutative, associative             (Island 0.2)
└── Multiplication: repeated addition,
    identity, commutative, associative,
    distributive                          (Island 0.3)
```

The distributive law is the only law that mentions both operations. Without it, addition and multiplication are strangers. With it, they are one system.

---

## ٤. Al-Khwarizmi Solves

### Example 1: The Farmer's Harvest

<!-- diagram: example-zakat -->

The farmer has five good fields at 100 measures and two damaged fields at 80 measures. Total harvest?

**Solution:**

```
100 × 5 + 80 × 2
```

Compute each term:

```
100 × 5 = 500
80 × 2 = 80 + 80 = 160
```

Total:

```
500 + 160 = 660
```

The farmer's harvest: **660 measures**.

### Example 2: Ibrahim's Harvest (Distributive Computation)

<!-- diagram: example-damaged -->

Ibrahim has 23 fields, each yielding 47 measures. Total harvest?

**Solution:**

```
47 × 23
```

By the distributive law, break 23 into parts I can handle:

```
47 × 23 = 47 × (20 + 3)
        = 47 × 20 + 47 × 3
```

Compute `47 × 20`. By associativity: `47 × 20 = 47 × (2 × 10) = (47 × 2) × 10`.

```
47 × 2 = 47 + 47 = 94
94 × 10 = 940
```

Compute `47 × 3`:

```
47 × 3 = 47 + 47 + 47 = 141
```

Total:

```
940 + 141 = 1081
```

Ibrahim's harvest: **1081 measures**.

### Example 3: The Grain Verse

One seed grows seven ears. Each ear holds a hundred grains. How many grains from twelve seeds?

**Solution:**

```
12 × 7 × 100
```

By associativity, group as I wish:

```
12 × (7 × 100) = 12 × 700
```

By the distributive law:

```
12 × 700 = (10 + 2) × 700
          = 10 × 700 + 2 × 700
          = 7000 + 1400
          = 8400
```

Twelve seeds yield **8400 grains**.

---

## ٥. Your Turn

### Da'if (Guided)

<!-- diagram: ex-daif-grid -->

**1.** Compute using the definition (repeated addition):
(a) `6 × 4`
(b) `9 × 3`
(c) `1 × 15`
*Hint: write each as a sum, then add.*

**2.** Draw a rectangle of pebbles to show that `5 × 3 = 3 × 5`. How many pebbles in total? Which property guarantees they are equal?

**3.** The farmer's neighbor Ibrahim sets aside grain for three families. Each family receives 47 measures. Write this as a multiplication, then compute `47 × 3` by adding.

### Hasan (Exam-level)

<!-- diagram: ex-hasan-distributive -->

**4.** Use the distributive law to compute: [3 marks]
(a) `8 × 34`
(b) `6 × 203`
(c) `14 × 15`
Show your working for each.

**5.** The farmer has 9 fields. Seven fields produced 100 measures each. Two fields (damaged by locusts) produced 80 measures each. [4 marks]
(a) Write the total harvest as a sum of two multiplications.
(b) Compute the total.
(c) The farmer later discovers a tenth field he forgot — it produced 100 measures. What is his new total? Use your answer from (b).

**6.** Expand: [3 marks]
(a) `3 × (x + 5)`
(b) `(a + b) × 7`
(c) `4 × (2a + 3b)`

### Sahih (Proof and extension)

**7.** Prove that `a × (b + c + d) = a × b + a × c + a × d` using only the two-term distributive law. [4 marks]
*Hint: let `e = c + d` and apply the law twice.*

**8.** Prove that `(a + b) × (c + d) = a × c + a × d + b × c + b × d` using only the distributive and commutative laws. [5 marks]
This is *double distribution*. You will use it in Island 0.7 (quadratics) and beyond.

---

## ٦. Exam Technique

> **The distributive law is the engine of algebra.** Every time you expand a bracket, you are using `a × (b + c) = a × b + a × c`. Every time you factorise, you are reading the same law backward: `a × b + a × c = a × (b + c)`.
>
> **Single bracket expansion:** `a(b + c) = ab + ac`. The term outside must reach every term inside.
>
> **Common error:** `3(x + 4) = 3x + 4`. Wrong. The 3 must multiply BOTH terms: `3(x + 4) = 3x + 12`.
>
> **Double bracket expansion:** `(a + b)(c + d)`. Treat `(a + b)` as a single multiplier, distribute over `(c + d)`, then distribute again. Result: `ac + ad + bc + bd`. The mnemonic "FOIL" is a special case of this — the distributive law applied twice.
>
> **Factoring:** Same law, reversed. `ab + ac = a(b + c)`. When a mark scheme says "factorise fully," it means extract the largest common factor: `6x + 12 = 6(x + 2)`, not `2(3x + 6)`.
>
> **Mental arithmetic:** `17 × 6 = (10 + 7) × 6 = 60 + 42 = 102`. Break the harder number into tens and units. This is the distributive law, whether or not the exam calls it that.
>
> **Signs:** Multiplication with negative numbers arrives in Island 0.4. For now, the distributive law works with addition only.

---

## ٧. Log Pose

```
1 = 1
├── 0.1 Equality (the scale)
│     a = a, a = b → b = a, preservation
├── 0.2 Counting (the shepherd)
│     N, S(n), addition, commutative, associative
└── 0.3 Multiplication (the grain)
       a × b = b × a          (commutative)
       (a × b) × c = a × (b × c)   (associative)
       a × (b + c) = a × b + a × c  (distributive)
       a × 1 = a              (identity)
```

**This island unlocks:**
- **Island 0.4** — Zero and Negatives: a man has 3 dinars and owes 5. His position is not any number I have built.
- **Island 0.5** — Fractions: the farmer's zakat (660 ÷ 40) and the inheritance shares finally computed. Multiplication converts shares to dinars.

**Forward connections to FP1:**
- Distributive law → expanding brackets → polynomial manipulation
- Double distribution → quadratic expansion (Island 0.7)
- Associativity → matrix multiplication (FP1: matrices)
- Factoring → roots of polynomials, factor theorem

---

## ٨. Reflection

The farmer picked up his bags and left. He has his number — six hundred and sixty measures — and he has six days before the collector arrives. He will come back for the rest.

I did not tell him what his grain taught me. He does not need the word *distributive*. He does not need the rectangle argument. His fields already obey these laws. Seven ears per stalk, a hundred grains per ear — he has held the computation in his rough hands every harvest.

But I need the laws. The farmer's problem was seven fields. Ibrahim's was twenty-three. The inheritance — still waiting, still unsolved — will demand multiplication of fractions by whole numbers, shares converted into dinars. When I reach that family again, it will be this operation that turns "one-eighth of the estate" into an amount a widow can hold.

> *Margin note: The distributive law is the only law that connects two operations — multiplication and addition. Every future tool that bridges two structures will echo this pattern. The bridge is always the most important part.*

The overflow persists. `27/24 > 1`. The family waits. But now I can multiply, and when I build fractions I will need multiplication to compute each heir's share in dinars. The tool learned from the farmer will serve the family.

The farmer asked: what is one-fortieth of six hundred and sixty? I could not answer. Between sixteen and seventeen. Not a whole number. Not any number I have.

But a harder problem waits first. A man in the market owes more than he holds. Three dinars in his hand, five dinars on a contract. His honest position is not one, not two, not any counting number the shepherd and I built at the gate. He stands below the lowest number I have. The qadi needs to write his position, and my mathematics has no symbol for it.

My numbers do not go low enough. That is the next wall.

*1 = 1 has not been lost.*

---
