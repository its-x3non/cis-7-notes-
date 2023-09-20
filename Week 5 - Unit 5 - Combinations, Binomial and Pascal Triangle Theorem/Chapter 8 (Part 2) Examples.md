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