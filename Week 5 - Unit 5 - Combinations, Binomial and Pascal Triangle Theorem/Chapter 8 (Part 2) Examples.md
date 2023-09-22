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
#### Permutations (Non-Repetitive) Formula
$$\frac{16!}{3!(16-3)!} = \frac{16!}{3! \times13!} = 16 \times 15 \times 14 = 3,360$$
### Errands Example
From the ["errands" example from the previous section](../Week%204%20-%20Unit%204%20-%20Counting/Chapter%208%20(Part%201)%20Examples.md#Permutation-Example---Errands)
