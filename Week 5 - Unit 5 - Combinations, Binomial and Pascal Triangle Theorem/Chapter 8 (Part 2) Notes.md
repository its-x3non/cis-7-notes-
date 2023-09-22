## Table of Contents

***
> **Examples are provided within another page, click the corresponding link below each section**
# Chapter 8 (Part 2): Combinations in Counting - Notes Simplified
## Combinations
An **r-permutation** is an **ordered arrangement or r out of n elements**, while an **r-combination** is an unordered subset of r out of n elements.
## Combinations vs Permutations
### Permutations
- When the **order doesn't mater**, it's a **combination**
- When the **order DOES matter**, it's a **permutation**
	- There are 2 types of permutation: **Repetition** and **non-repetition**
### Counting r-combinations
- The number of r-combinations of n distinct elements is
$$C(n,r) = (\substack{n\\r}) = \frac{n!}{r!\times(n-r)!}$$
#### Proof
$$P(n,r) = C(n,r)\times P(r,r)$$That is, to create an **ordered list of r elements from a set of n elements**
1) First, **choose r elements from the set (there are C(n,r) )** ways to do this
2) Then, choose **an ordering of the r elements** (there are **P(r,r)** ways to do this). Since we already know that $$\frac{n!}{r!\times (n-r)!} \space and \space P(r,r) = r!$$The result follows.
Choosing **r out of n elements to be included in a subset is <u>equivalent</u> to choosing the n − r elements** which should be left out of the subset. Therefore, <u>every r-combination has a unique associated (n − r)-combination</u>, and thus the number of **r-combinations is equivalent to the number of (n − r)-combinations**:
$$C(n,r) = (\substack{n\\r}) = \frac{n!}{r!\times(n-r)!} = \frac{n!}{(n-r)!\times r!} = (\substack{n\\n-r}) = C(n,n-r) $$
### Combinations: Order does not matter
- There are 2 types of combinations: **Repetition and No-Repetition**
- **Repetition is Allowed**: such as coins in your pocket (5,5,5,10,10)
In **permutation**, choosing balls 1, 2, and 3. These are the possibilities:
# REMEMBER TO GO BACK TO INSERT THE TABLE
So the permutations have 6 times as many possibilities in comparison to combinations.
## Balls in Bins
i'll do this later lol <br />
just remind me to do this if you see this message if i never got to it.

# Binomial Theorem
- Binomial Theorem which allows one to expand expressions of the form **(x+y)<sup>n</sup>** for any **non-negative integer n**.
- 
# Pascal Triangle
Pascal's Triangle arises as a consequence of the following fact concerning binomial coefficient.