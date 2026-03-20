# Island 0.5: Fractions — The Inheritance Fulfilled

بسم الله الرحمن الرحيم

---

## ١. The Ayah

> يُوصِيكُمُ اللَّهُ فِي أَوْلَادِكُمْ ۖ لِلذَّكَرِ مِثْلُ حَظِّ الْأُنثَيَيْنِ ۚ فَإِن كُنَّ نِسَاءً فَوْقَ اثْنَتَيْنِ فَلَهُنَّ ثُلُثَا مَا تَرَكَ ۖ وَإِن كَانَتْ وَاحِدَةً فَلَهَا النِّصْفُ ۚ وَلِأَبَوَيْهِ لِكُلِّ وَاحِدٍ مِّنْهُمَا السُّدُسُ مِمَّا تَرَكَ إِن كَانَ لَهُ وَلَدٌ

> "Allah instructs you concerning your children: for the male, what is equal
> to the share of two females. But if there are only daughters, two or more,
> for them is two-thirds of what he left. And if there is only one, for her
> is half. And for one's parents, to each one of them is a sixth of what he
> left, if he left children..."
> *— Surah An-Nisa (4:11)*

> وَلَهُنَّ الرُّبُعُ مِمَّا تَرَكْتُمْ إِن لَّمْ يَكُن لَّكُمْ وَلَدٌ ۚ فَإِن كَانَ لَكُمْ وَلَدٌ فَلَهُنَّ الثُّمُنُ مِمَّا تَرَكْتُمْ

> "And for the wives is a fourth of what you leave if you have no child. But
> if you have a child, then for them is an eighth of what you leave..."
> *— Surah An-Nisa (4:12)*

**Connection grade: SAHIH** — the verse IS the problem. The Quran prescribes exact fractional shares: one-half, two-thirds, one-fourth, one-sixth, one-eighth. A family fulfilling this command needs fraction arithmetic to obey it. Remove the fractions and the verse cannot be executed. Zero links.

**The problem this ayah creates:** A man has died. His wife, two daughters, father, and mother sit before me with an estate of 2700 dinars. The Quran gives each heir an exact fractional share. But what IS a fraction? How do I add one-sixth to one-eighth? And when the shares demand more than the estate contains — what then?

---

## ٢. Al-Khwarizmi Thinks

The wife enters first. She walks the way a woman walks who held the household together before her husband died and will hold it together after. The two daughters are behind her, close enough that their sleeves touch. The father comes last. He is burying his son. Every step costs him something. The mother is already seated when I look up. She was here before them. She is waiting.

The qadi has sent them. The estate is 2700 dinars. The Quran prescribes their shares.

I write them:

| Heir | Prescribed share | Source |
|------|-----------------|--------|
| Wife | 1/8 of the estate | 4:12 — husband had children |
| Two daughters | 2/3 of the estate | 4:11 — two or more daughters |
| Father | 1/6 of the estate | 4:11 — deceased had children |
| Mother | 1/6 of the estate | 4:11 — deceased had children |

I stare at what I have written.

One-eighth. Two-thirds. One-sixth.

These are not integers. They are not any number I have built in four islands of work. I have the natural numbers — 1, 2, 3, counting upward without end. I have zero, the empty position. I have negatives, the debtor's honest record. I have addition, multiplication, their inverses and laws. Every tool I own operates on whole numbers.

Not one of them can say "one-eighth."

I try anyway. The wife's share is 1/8 of 2700. I know what that means — divide 2700 into 8 equal parts, take one. But I have no operation for "divide into equal parts." Multiplication gives me 8 × 337 = 2696. Close, but not 2700. 8 × 338 = 2704. Too much. The answer is between 337 and 338. Between two integers. In a place where no integer lives.

I try another way. The daughters' share is 2/3 of 2700. I need 2700 split into 3 parts, then take 2 of them. 2700 = 3 × 900. So two-thirds is 1800. That works — but only because 3 divides 2700 evenly. What if the estate were 2500? 2500 divided by 3 is... not a whole number. My method breaks again.

> *Margin note: The integers handle "how many" and "how far below zero." They cannot handle "what part of." The Quran demands parts. My tools do not have parts.*

The family is sitting in front of me. The wife has placed her hands flat on the table, palms down. The daughters are still. The father has lowered himself onto the bench by the wall. The mother watches.

I cannot tell them to wait while I invent mathematics. But I cannot give them an answer with tools that do not reach their problem.

I need a new kind of number. A number that lives between the integers. A number that can say "one-eighth" the way 5 says "five."

### What is a fraction?

I go back to 1 = 1. Everything I have built grew from here. Addition grew from succession. Multiplication grew from repeated addition. Negatives grew from the impossibility of subtracting a larger number from a smaller. Each time, a problem forced the numbers to extend.

This time the problem is division. Multiplication says: 8 × something = 1. What is that something?

I already know 8 × 0 = 0. Too small. 8 × 1 = 8. Too large. The answer is between 0 and 1. I name it.

```
1/8 means: the number which, multiplied by 8, gives 1.

8 × (1/8) = 1
```

This is the multiplicative inverse of 8. Just as −5 was the additive inverse of 5 (the number that, added to 5, gives 0), 1/8 is the multiplicative inverse of 8 (the number that, multiplied by 8, gives 1).

> *Margin note: "And of everything We have created pairs" (51:49). Addition and subtraction. Multiplication and division. Each operation exists with its inverse.*

More generally, a fraction a/b is defined:

```
a/b = a × (1/b)
```

It means: take the multiplicative inverse of b (the number that gives 1 when multiplied by b), then multiply by a. Three-eighths: take the inverse of 8, multiply by 3. Two-thirds: take the inverse of 3, multiply by 2.

The definition requires one thing: b cannot be zero. If b = 0, I need a number that, multiplied by 0, gives 1. But I proved in Island 0.4 that 0 × anything = 0. No number multiplied by 0 gives 1. Division by zero is not forbidden by convention. It is impossible by logic. The inverse of 0 does not exist.

### The rational numbers

With fractions, I extend once more:

```
N ⊂ Z ⊂ Q

Natural numbers: {1, 2, 3, ...}
Integers:        {..., -2, -1, 0, 1, 2, ...}
Rationals:       {a/b : a, b ∈ Z, b ≠ 0}
```

Every integer is rational: 5 = 5/1. The rationals do not replace the integers — they extend them. Subtraction forced Z into existence. Division forces Q.

### When are two fractions equal?

I write 1/2 and 2/4. These should be the same quantity. One loaf split between 2 people, each getting 1 piece. Two loaves split between 4 people, each getting 2 pieces. Same amount of bread. But the symbols are different. I need a rule.

Two fractions a/b and c/d represent the same quantity when:

```
a/b = c/d   if and only if   a × d = b × c
```

Check: 1/2 = 2/4 because 1 × 4 = 4 = 2 × 2. Yes.

Check: 2/3 = 8/12 because 2 × 12 = 24 = 3 × 8. Yes.

This is the cross-multiplication test. It follows from the definition: if a/b = c/d, multiply both sides by b × d, and the equality laws from Island 0.1 give a × d = b × c.

### Arithmetic

I need to add, multiply, and divide fractions before I can touch the family's problem. I build each operation.

**Addition.** To add a/b + c/d, I need the pieces to be the same size. Eighths and thirds are different-sized pieces. I cannot add them any more than the shepherd could mix sheep and camels in a single count.

I convert both fractions to pieces of the same size — a common denominator:

```
a/b + c/d = (a × d + b × c) / (b × d)
```

This works because multiplying numerator and denominator by the same number is multiplying by 1. The value does not change. This is preservation of equality — Island 0.1.

When b × d is larger than necessary, I use the least common multiple (LCM) of the denominators instead. Same result, smaller numbers.

**Multiplication.** Two fractions multiply cleanly:

```
(a/b) × (c/d) = (a × c) / (b × d)
```

Numerators multiply. Denominators multiply.

**Division.** Dividing by a fraction means multiplying by its reciprocal:

```
(a/b) ÷ (c/d) = (a/b) × (d/c) = (a × d) / (b × c)     [c ≠ 0]
```

Division undoes multiplication. The reciprocal flips the fraction. I will prove each of these in Section 3.

### Back to the family

Now I can name the wife's share. One-eighth. I can name the daughters'. Two-thirds. The father's and mother's. One-sixth each.

But naming is not distributing. I must add these shares to find the total. They have four different denominators: 8, 3, 6, 6. I need a common denominator — a single piece-size that measures all four.

The multiples of 8: 8, 16, 24, 32...
The multiples of 3: 3, 6, 9, 12, 15, 18, 21, 24...
The multiples of 6: 6, 12, 18, 24...

LCM(8, 3, 6) = 24. Twenty-four is divisible by 8, by 3, and by 6. I convert every share to twenty-fourths:

```
Wife:       1/8 = 3/24     (× 3)
Daughters:  2/3 = 16/24    (× 8)
Father:     1/6 = 4/24     (× 4)
Mother:     1/6 = 4/24     (× 4)
```

I add the numerators.

```
3 + 16 + 4 + 4 = 27
```

I stop.

27/24.

That is greater than 1.

Twenty-seven parts out of twenty-four. The Quran prescribes four shares, each just in isolation, and together they demand more than the estate. There is not enough.

I check the arithmetic. 3 + 16 = 19. 19 + 4 = 23. 23 + 4 = 27. Correct. I check the conversions. 1/8 = 3/24 because 1 × 24 = 24 = 8 × 3. Correct. 2/3 = 16/24 because 2 × 24 = 48 = 3 × 16. Correct. I check the verse references. Wife with children: 1/8. Two or more daughters: 2/3. Each parent when deceased had children: 1/6. Every share is correct.

The overflow is not my error. It is the situation.

> *Margin note: Each share is prescribed for a relationship — wife, daughter, parent — considered on its own. When all four relationships exist in one estate, the total can exceed the whole. The verse prescribes just ratios. The mathematics must reconcile them with a finite estate.*

The wife is watching me. She has seen the number I wrote. She does not read mathematics, but she reads faces, and she has read mine.

"Is there a problem?"

"The shares add to more than the estate." I do not soften it. She is not a woman who needs softening. "Each share is correct. Together they exceed what he left."

She does not look away. "Then what do we do?"

### The method of 'awl

The Caliph Umar ibn al-Khattab, may Allah be pleased with him, was the first to face this. He gathered the Companions. They reasoned: when a man dies owing debts greater than his estate, each creditor does not receive the full amount — each receives a fair proportion of what exists. The debts are real. The estate is finite. Justice is proportional.

The same principle applies here. The Quranic shares are real. The estate is finite. Each heir's share is reduced by the same proportion. No heir bears more of the shortfall than any other.

> *Margin note: The scholar Ibn Abbas, may Allah be pleased with him, held a different view — that certain heirs (the daughters, in cases like this) should bear the reduction, while others (the spouse, the parents) receive their full prescribed share. The Shi'a school follows this position. What I describe here, 'awl (proportional reduction applied to all), is the majority Sunni method established by Umar's consultation. The mathematics of both approaches is sound. The legal question of which to apply belongs to the jurists, not the mathematician. I teach the technique. See 42:10 — "And in anything over which you disagree, its ruling is with Allah."*

The procedure. The original denominator is 24. The numerators sum to 27. I raise the denominator to match the sum:

```
Original shares:   3/24 + 16/24 + 4/24 + 4/24 = 27/24
Adjusted shares:   3/27 + 16/27 + 4/27 + 4/27 = 27/27 = 1
```

The total is now exactly 1. The estate is fully distributed. And the ratios — the proportional relationships the Quran established — are preserved. Before 'awl, the daughters had 16 parts to the wife's 3. After 'awl, still 16 to 3. The relationship holds. Only the scale changes.

Now I compute the dinars. The estate is 2700.

```
Wife:       2700 × 3/27  = 2700/9  = 300 dinars
Daughters:  2700 × 16/27 = 1600 dinars  (800 each)
Father:     2700 × 4/27  = 400 dinars
Mother:     2700 × 4/27  = 400 dinars
```

300 + 1600 + 400 + 400 = 2700. Every dinar accounted for.

I write the amounts on the paper and turn it so the wife can see. She reads the numbers — these she understands. She nods once, the way someone nods when a weight shifts from their chest to the ground. She stands. She gathers her daughters.

The father pushes himself from the bench. He does not look at the paper. He looks at his son's wife, steady and upright, and for the first time since he entered the room, something in his face eases.

The mother folds the cloth she has been holding. She places it on the table. She does not need to grip it anymore.

---

## ٣. The Derivation

**From 1 = 1 to fraction arithmetic.**

Every result below derives from the definition of the multiplicative inverse combined with the laws established in Islands 0.1–0.4.

### Definition: multiplicative inverse

For any integer a ≠ 0, the multiplicative inverse of a is the number 1/a such that:

```
a × (1/a) = 1
```

This extends the multiplicative identity (a × 1 = a) by asking: what number plays the role of "undoing" multiplication, the way −a undoes addition?

### Definition: fraction

```
a/b = a × (1/b)          [b ≠ 0]
```

A fraction is a product: the integer a multiplied by the inverse of the integer b.

### Why division by zero is impossible

Suppose 1/0 exists. Then 0 × (1/0) = 1 by definition. But 0 × (1/0) = 0 (proved in Island 0.4: 0 × n = 0 for all n). So 0 = 1. This contradicts 0 ≠ 1.

For a/0 with a ≠ 0: I need 0 × ? = a. But 0 × anything = 0 ≠ a. No solution exists.

For 0/0: I need 0 × ? = 0. Every number satisfies this. The answer is not unique.

In all cases, division by zero fails — either by contradiction, by nonexistence, or by non-uniqueness. ∎

### The rational numbers Q

```
Q = {a/b : a, b ∈ Z, b ≠ 0}
```

**Q extends Z:** Every integer n equals n/1, so Z ⊂ Q. The extension is strict — 1/2 ∈ Q but 1/2 ∉ Z.

**Q inherits all laws:** Addition (commutative, associative), multiplication (commutative, associative, distributive over addition), additive identity (0), multiplicative identity (1), additive inverses (negatives). These carry forward from Z because Z ⊂ Q.

**Q adds:** multiplicative inverses for every nonzero element. This is the new capability.

### Equivalence of fractions

**Theorem.** a/b = c/d if and only if a × d = b × c.

*Proof.* (⇒) Suppose a/b = c/d. Multiply both sides by b × d (which is nonzero since b ≠ 0 and d ≠ 0):

```
(b × d) × (a/b) = (b × d) × (c/d)
```

Left side: (b × d) × (a/b) = d × (b × a/b) = d × a = a × d. [Associative, then definition: b × (a/b) = a, then commutative.]

Right side: (b × d) × (c/d) = b × (d × c/d) = b × c. [Same reasoning.]

So a × d = b × c. ∎

(⇐) follows by reversing the steps: if a × d = b × c, divide both sides by b × d.

*Example:* 2/3 = 8/12 because 2 × 12 = 24 = 3 × 8.

### Addition of fractions

**Theorem.**

```
a/b + c/d = (a × d + b × c) / (b × d)
```

*Proof.* Let S = a/b + c/d. Multiply both sides by b × d:

```
(b × d) × S = (b × d) × (a/b) + (b × d) × (c/d)   [distributive law, Island 0.3]
             = d × a + b × c
             = a × d + b × c                          [commutative law]
```

Therefore S = (a × d + b × c) / (b × d). ∎

**Common denominators via LCM.** When b × d is larger than necessary, use L = LCM(b, d) instead. Write a/b = (a × L/b) / L and c/d = (c × L/d) / L. Then add numerators over L. The result is the same fraction, with smaller numbers.

*Finding the LCM:* For two numbers, LCM(b, d) = (b × d) / GCD(b, d). For three or more, compute pairwise: LCM(b, d, e) = LCM(LCM(b, d), e).

### Multiplication of fractions

**Theorem.**

```
(a/b) × (c/d) = (a × c) / (b × d)
```

*Proof.* Let P = (a/b) × (c/d). Multiply both sides by b × d:

```
(b × d) × P = (b × d) × (a/b) × (c/d)
             = [b × (a/b)] × [d × (c/d)]    [associative + commutative, Islands 0.2–0.3]
             = a × c                          [definition of inverse]
```

Therefore P = (a × c) / (b × d). ∎

### Division of fractions

**Theorem.**

```
(a/b) ÷ (c/d) = (a/b) × (d/c) = (a × d) / (b × c)     [c ≠ 0]
```

*Proof.* Dividing by c/d means finding the number Q such that (c/d) × Q = a/b. Multiply both sides by d/c (the reciprocal of c/d):

```
Q = (a/b) × (d/c)
  = (a × d) / (b × c)    [by multiplication theorem]  ∎
```

### The 'awl procedure — formalized

Given prescribed fractional shares s₁, s₂, ..., sₙ:

1. Find a common denominator D.
2. Express each share as kᵢ / D.
3. Sum the numerators: T = k₁ + k₂ + ... + kₙ.
4. If T = D: shares balance. Distribute each share as (kᵢ / D) × E, where E is the estate.
5. If T < D: a remainder of (D − T)/D exists, distributed by ta'sib (residual rules).
6. If T > D: apply 'awl. Replace D with T. Each heir receives (kᵢ / T) × E.

### Proof that 'awl preserves ratios

**Theorem.** The ratio between any two heirs' shares is the same before and after 'awl.

*Proof.* Before 'awl, heir i receives kᵢ / D and heir j receives kⱼ / D. Their ratio:

```
(kᵢ / D) ÷ (kⱼ / D) = kᵢ / kⱼ
```

After 'awl, heir i receives kᵢ / T and heir j receives kⱼ / T. Their ratio:

```
(kᵢ / T) ÷ (kⱼ / T) = kᵢ / kⱼ
```

The ratios are identical. The denominators cancel. Every proportional relationship the Quran established between heirs is preserved exactly. ∎

**The chain from 1 = 1:**

```
1 = 1
  → equality (reflexive, symmetric, transitive)           [Island 0.1]
  → preservation: equals applied to equals yield equals   [Island 0.1]
  → multiplication: a × b defined, commutative,
    associative, distributive                              [Islands 0.2–0.3]
  → multiplicative identity: a × 1 = a                    [Island 0.3]
  → multiplicative inverse: a × (1/a) = 1, a ≠ 0
  → fractions defined: a/b = a × (1/b)
  → equivalence: a/b = c/d iff a × d = b × c              [cross-multiplication]
  → addition: common denominator, from distributive law    [Island 0.3]
  → multiplication: (a/b)(c/d) = (ac)/(bd)
  → division: multiply by reciprocal
  → 'awl: proportional scaling preserves ratios            [from equivalence]
```

Every operation traces back to 1 = 1 through laws already derived. No new axioms.

---

## ٤. Al-Khwarizmi Solves

### Worked Example 1: The family's inheritance — full computation

*The estate is 2700 dinars. Heirs: wife, two daughters, father, mother.*

**Step 1.** Prescribed shares with common denominator.

Denominators: 8, 3, 6, 6. I need LCM(8, 3, 6).

```
LCM(8, 3) = 24    [since GCD(8, 3) = 1, so LCM = 8 × 3]
LCM(24, 6) = 24   [since 6 divides 24]
```

Convert:

```
Wife:       1/8 = 3/24
Daughters:  2/3 = 16/24
Father:     1/6 = 4/24
Mother:     1/6 = 4/24
```

**Step 2.** Check the sum: 3 + 16 + 4 + 4 = 27 > 24. Apply 'awl: raise denominator to 27.

```
Wife:       3/27
Daughters:  16/27
Father:     4/27
Mother:     4/27
Sum:        27/27 = 1  ✓
```

**Step 3.** Compute dinars.

```
Wife:       2700 × 3/27  = 8100/27  = 300 dinars
Daughters:  2700 × 16/27 = 43200/27 = 1600 dinars  (800 each)
Father:     2700 × 4/27  = 10800/27 = 400 dinars
Mother:     2700 × 4/27  = 10800/27 = 400 dinars
```

**Verification:** 300 + 1600 + 400 + 400 = 2700 ✓

**Ratio check:** Daughters' share / wife's share = 1600/300 = 16/3. Before 'awl: (16/24) ÷ (3/24) = 16/3. Preserved. ✓

---

### Worked Example 2: An inheritance that balances

*A man dies leaving 1200 dinars. His heirs: one daughter and both parents. No spouse.*

The Quran prescribes:
- One daughter: 1/2 (4:11 — only one daughter)
- Father: 1/6 (4:11 — deceased had children)
- Mother: 1/6 (4:11 — deceased had children)

Common denominator: LCM(2, 6) = 6.

```
Daughter:  1/2 = 3/6
Father:    1/6 = 1/6
Mother:    1/6 = 1/6
Sum:       3 + 1 + 1 = 5/6
```

5/6 < 1. No 'awl. The remainder 1/6 returns to the father as ta'sib (residual share). His total: 1/6 + 1/6 = 2/6 = 1/3.

```
Daughter:  1200 × 1/2 = 600 dinars
Father:    1200 × 1/3 = 400 dinars
Mother:    1200 × 1/6 = 200 dinars
                 Total = 1200 dinars  ✓
```

---

### Worked Example 3: Fraction arithmetic

Simplify:

```
  2     5     1
 --- + --- - ---
  3     6     4
```

Common denominator: LCM(3, 6, 4).

```
LCM(3, 6) = 6
LCM(6, 4) = 12
```

Convert:

```
2/3 = 8/12     (× 4)
5/6 = 10/12    (× 2)
1/4 = 3/12     (× 3)
```

Compute:

```
8/12 + 10/12 - 3/12 = (8 + 10 - 3)/12 = 15/12
```

Simplify: GCD(15, 12) = 3.

```
15/12 = 5/4
```

Check: 5/4 × 12 = 60/4 = 15 = 8 + 10 − 3. ✓

---

## ٥. Your Turn

### Da'if (Guided)

**D1.** A woman dies leaving 3600 dinars. Her heirs: a husband and one daughter.

The Quran prescribes:
- Husband: 1/4 (4:12 — wife had children)
- Daughter: 1/2 (4:11 — only one daughter)

(a) Find the common denominator for 1/4 and 1/2.
*Hint: What is the LCM of 4 and 2?*

(b) Express each share with the common denominator and compute the sum.
*Hint: Convert 1/2 to the common denominator, then add numerators.*

(c) Is the sum less than 1, equal to 1, or greater than 1? Is 'awl needed?

(d) The remainder goes to the nearest male relative as ta'sib. What fraction of the estate is the remainder?

(e) Compute the amount in dinars each heir receives.

---

**D2.** The two daughters from the family's case each received 800 dinars. Suppose their mother (the wife, who received 300 dinars) wants to give each daughter a gift of 1/5 of her own share.

(a) Compute 1/5 of 300.
*Hint: 300 × (1/5) = 300/5.*

(b) How much does each daughter now hold in total?

---

**D3.** Simplify:

```
  3     1
 --- + ---
  4     6
```

*Hint: LCM(4, 6) = 12. Convert both fractions to twelfths.*

---

### Hasan (Exam-level)

**H1.** A man dies leaving an estate of 4800 dinars. His heirs: a wife, one daughter, and a mother.

The Quran prescribes:
- Wife: 1/8 (4:12 — husband had children)
- Daughter: 1/2 (4:11 — only one daughter)
- Mother: 1/6 (4:11 — deceased had children)

(a) Find the sum of prescribed shares. Express as a single fraction over the LCM. [3 marks]

(b) Determine whether 'awl is needed. Justify your answer. [1 mark]

(c) A remainder exists. Find its value as a fraction of the estate. [2 marks]

(d) The remainder goes to the nearest male relative as ta'sib. Calculate each heir's share in dinars, assuming no ta'sib claimant exists and the remainder is redistributed proportionally. [3 marks]

---

**H2.** Simplify fully: [3 marks]

```
  5     7     2
 --- - --- + ---
  8    12     3
```

---

**H3.** The father from the family's inheritance (who received 400 dinars) later dies. His own heirs are: his wife (the mother from the original case, who already received 400 dinars) and no children.

The wife's share when there are no children: 1/4 (4:12).

(a) Compute the mother's inheritance from the father's 400 dinars. [2 marks]

(b) Find the mother's total wealth after both inheritances. [1 mark]

(c) Express this total as a fraction of the original 2700-dinar estate. [2 marks]

---

### Sahih (Proof and extension)

**S1.** A man dies leaving an unknown estate of E dinars. His heirs: a wife, three daughters, and both parents.

(a) Write down the prescribed shares from 4:11–12 and compute their sum over a common denominator. Show that 'awl is required. [4 marks]

(b) Apply the 'awl procedure. Express each heir's adjusted share as a fraction of E. [4 marks]

(c) The wife receives 225 dinars. Find E. [2 marks]

(d) Verify that the total distribution equals E. [2 marks]

---

**S2.** Prove that between any two distinct rational numbers, there exists another rational number. [4 marks]

*Hint: If a/b < c/d, consider (a/b + c/d) / 2. Show this is rational and lies strictly between the two.*

*Extension: What does this imply about how many rationals lie between any two rationals? Are there any "gaps" in Q? (This question returns in Island 0.8.)*

---

**S3.** The Quran uses these fractional shares across its inheritance verses: 1/2, 1/3, 2/3, 1/4, 1/6, 1/8. [7 marks]

(a) Find the LCM of all the denominators: 2, 3, 4, 6, 8. [2 marks]

(b) Express every Quranic share with this common denominator. [2 marks]

(c) Explain why this LCM serves as the natural "base" for all inheritance calculations, and describe how the 'awl procedure interacts with this base when shares overflow. [3 marks]

---

## ٦. Exam Technique

> **EXAM NOTE: Fraction arithmetic**
>
> The mark scheme awards method marks (M) for showing a common
> denominator and accuracy marks (A) for correct final answers.
>
> **Always show the common denominator step.** Even if you can add
> fractions mentally, write it out:
>
> ```
> 1/3 + 1/6 = 2/6 + 1/6 = 3/6 = 1/2
> ```
>
> Jumping straight to 1/2 may lose M marks — the examiner cannot
> see your method.
>
> **Always simplify your final answer.** 15/12 must be written
> as 5/4. Unsimplified fractions lose the final A mark on most
> mark schemes.
>
> **Common mistake — subtracting denominators:**
>
> ```
> 5/6 - 1/4 ≠ 4/2       ← WRONG (subtracted 6 - 4)
> 5/6 - 1/4 = 10/12 - 3/12 = 7/12   ← CORRECT
> ```
>
> Only NUMERATORS change. The denominator is the common denominator.
>
> **Common mistake — multiplying when you should add:**
>
> ```
> 1/3 + 1/4 ≠ 1/12       ← WRONG (multiplied)
> 1/3 + 1/4 = 4/12 + 3/12 = 7/12    ← CORRECT
> ```
>
> Multiplication of fractions and addition of fractions are
> different operations. Do not confuse them.
>
> **'Awl problems:** When an exam asks about shares summing to
> more than 1, the answer is NOT "impossible." Apply 'awl:
> raise the denominator to match the numerator sum, then
> recompute each share. Always verify the total equals the
> estate.
>
> **LCM shortcut:** LCM(a, b) = (a × b) / GCD(a, b).
> For three or more: LCM(a, b, c) = LCM(LCM(a, b), c).

---

## ٧. Log Pose

```
                  +--- 0.6 Variables & Equations
                  |    (the merchant's unknown wealth)
                  |
0.5 Fractions ----+
(inheritance)     |
                  |
                  +--- 0.7 Quadratic Equations
                       (al-jabr's garden problem)
```

**This island unlocks:** Variables and Equations (0.6), where the problem shifts from known fractions to unknown quantities — a merchant who knows the rule (1/40 for zakat) but not the number it applies to. Also unlocks Quadratic Equations (0.7), where Al-Khwarizmi's original al-jabr problems require fraction manipulation throughout.

**Connection forward to FP1:** The fraction 27/24 > 1 — a system whose prescribed parts exceed its whole — previews a pattern that recurs throughout mathematics. In Arc 1, the number system itself overflows when the quadratic formula demands √(−1). Just as 'awl restored the inheritance by extending the denominator, complex numbers will restore algebra by extending the number line into a plane. Al-jabr — restoration — is the recurring motion.

---

## ٨. Reflection

The family came in the late afternoon. They left before maghrib.

The wife received 300 dinars. Each daughter received 800. The father and mother each received 400. The sum is 2700. Every dinar accounted for. Every ratio the Quran prescribed — daughters to wife, parents to daughters — preserved through the 'awl reduction. The proportional relationships survived the scaling. That is what justice looks like when the whole is not enough: not abandoning any claim, but bearing the shortfall together.

The four islands before this one were preparation. Equality, to know what "the same" means. Counting, to enumerate. Multiplication, to scale. Zero and negatives, to record what is absent and what is owed. Every tool pointed here — to the moment a grieving family needed exact fractions from a system that only knew whole numbers.

The fractions exist now. Not as abstractions. As the answer to a specific question asked by a specific family. The wife stood first. The father's face eased. The mother set down the cloth she had been gripping.

> تِلْكَ حُدُودُ اللَّهِ ۚ وَمَن يُطِعِ اللَّهَ وَرَسُولَهُ يُدْخِلْهُ جَنَّاتٍ تَجْرِي مِن تَحْتِهَا الْأَنْهَارُ
> "These are the limits of Allah, and whoever obeys Allah and His Messenger
> will be admitted into gardens beneath which rivers flow."
> *— Surah An-Nisa (4:13)*

This verse comes immediately after the inheritance verses. The fractions of 4:11–12 are not suggestions. They are hudud — limits set by Allah. The computation that executes them is not separate from the obedience. It is the obedience.

I set down my pen. The room is quiet. Then the door opens.

A broad-shouldered man enters, smelling of sandalwood and sea salt. His fingers are stained with ink — he keeps his own ledgers. He sits across from me and speaks without greeting.

"I must pay zakat. One part in forty of my wealth. But my warehouses are uncounted and my ships have not returned. I know the rule. I do not know the number."

He knows what fraction to compute. He does not know what to compute it from. Every tool I have built requires a known number — add this to that, multiply this by that, take one-eighth of this. His number is unknown. It might be 10,000 dinars. It might be 50,000. His ships might return full or empty or not at all.

I need a way to write: "one-fortieth of something I do not yet know."

*1 = 1 has not been lost.*

---
