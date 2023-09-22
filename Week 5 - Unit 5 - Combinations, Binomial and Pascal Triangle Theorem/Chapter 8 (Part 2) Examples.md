## Table of Contents
***
## Combinations vs Permutations
### Permutations - Safe Number (Repetition)
- A lock combination "222" - **Repetition**
- **For example:** choosing **3** of those things, the permutations are: $$n\times n\times n$$
- More generally: choosing **r** of something that has **n** different types, the permutations are: $$n \times n \times \ldots (r \space times) $$
	- In other words, there are **n** possibilities for the first choice, THEN there are **n** possibilities for the second choice, and so on, multiplying each time.
- Which is easier to write down using an exponent of r: $$n \times n \times \ldots (r \space times) = n^{r}$$
	- **For example:** For a lock number selection, there are 10 numbers to choose from (0, 1, 2, 3, 4, 5, 6, 7, 8 ,9) and we choose 3 of them:
		- 10 x 10 x ... (3 times) = 103 = 1,000 permutations
### Permutations - Olympic Race (Non-Repetition)
- We have to reduce the number of available choices each time
- What order could 16 pool balls be in?
	- After choosing, for example, number "14" we can't choose it again. So our first choice has 16 possibilities, and our next choice has 15 possibilities, then 14, 13, 12, 11, ... etc. And the total permutations are: **16 x 15 x 14 x 13 x ... = 20,922,789,888,000**
	- But maybe we don't want to choose them all, just 3 of them, then that will become: 16 x 15 x 14 = 3,360
#### Permutations (Non-Repetitive) Equation
$$\frac{16!}{3!(16-3)!} = \frac{16!}{3! \times13!} = 16 \times 15 \times 14 = 3,360$$
### Errands Example
- From the ["errands" example from the previous section](../Week%204%20-%20Unit%204%20-%20Counting/Chapter%208%20(Part%201)%20Examples.md#Permutation-Example---Errands), if ***one had to choose 2 out of the 4 possible errands***, there are **P(4,2) = 4 * 2 = 12** such **ordered arrangements (r-permutations)**.
- Note that ***such permutations distinguish between identical subsets of errands if they appear in a different order***:
	- e.g., **(grocery store, post office)** is different from **(post office, grocery store)**
		- This is because the errands are processed in a different order. If the order didn't matter, then these two "arrangements" would be identical and ***denoted with set notation {grocery store, post office}***
	- Such a subset is a 2-combination. More generally, an unordered subset of r elements out of n is an r-combination, and the number of such combination is denoted: $$C(n,r) = (\substack{n\\r})$$
	- Calculators often use the notation nCr analogous to nPr for r-permutations.
	- $$ (\substack{n\\r}) $$ This part is often referred to as a binomial coefficient.

### Combinations Example - Ice Cream Flavors
- There are 5 flavors of ice cream: **banana, chocolate, lemon, strawberry, and vanilla**
- We can have 3 scoops. How many variations will there be?
- We can use the letters for the flavors: {b, c, l, s, v}. Example selections include:
	- {c, c, c} - 3 scoops of chocolate
	- {v, v, v} - 3 scoops of vanilla
	- {b, l, v} - One each of banana, lemon, and vanilla
	- {b, v, v} - One of banana, 2 of vanilla
	- etc...
		- There are **n=5** things to choose from, and we choose **r=3** of them.
		- **ORDER DOESN'T MATTER** and we **CAN** repeat.
- How many different ways can we select ice cream flavors?
Formula: $$\frac{(r+n-1)!}{r!(n-1)!}$$
- Where **n** is the number of things to choose from, and we can choose **r** of them. Repetition is allowed, order doesn't matter.
- Choosing 3 of 5 flavors of ice-cream:
$$=\frac{(3+5-1)!}{3!(5-1)!}=\frac{7!}{3!\times 4!} = 35$$
## Balls in Bin
### Halloween Example
remind me to do this too
