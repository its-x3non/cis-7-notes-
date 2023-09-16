## Table of Contents
- [Example 1 (Sum Rule)](#Example-1-Sum-Rule)
- [Example 2 (Product Rule)](#Example-2-Product-Rule)
- [Inclusion-Exclusion Principle](#Inclusion-Exclusion-Principle)
- [The Pigeonhole Principle](#The-Pigeonhole-Principle)
	- [Generalized Pigeonhole Principle](#Generalized-Pigeonhole-Principle)
- [Permutation](#Permutation)
- [External Resources](#External-Resources)
***
> **Examples are provided within another page, click the corresponding link below each section**
# Chapter 8 (Part 1): Counting - Notes Simplified
**Combinatorics** - A branch of mathematics largely concerned with counting discrete objects <br />
Many problems in comp sci involve **counting** possible solutions, **enumerating** those solutions, or **finding** the optimal solution among a candidate set.
## [Examples from the beginning of the Notes](Chapter%208%20(Part%201)%20Examples.md)
***
## Example 1 (Sum Rule)
Alice order soup or sandwich: **6 types of soups, 12 different sandwiches.** <br />
Alice must choose **either one of six soups or one of 12 sandwiches** for a total of **6 + 12 = 18 different meals** <br />
### Sum Rule
If A and B are **disjoint finite sets** then the number of ways of choosing a **single element** from **A or B is |A ∪ B| = |A| + |B|.**
- The sum rule is applicable when one must make one choice from the union of two (or more) sets of alternatives; sum rule can be generalized to more than two sets of alternatives in an obvious way.
	- **General Sum Rule:** If A<sub>1</sub>, A<sub>2</sub>, . . . , A<sub>n</sub> are mutually disjoint finite sets then the number of ways of choosing a single element from A<sub>1</sub>, A<sub>2</sub>, . . . , or An is **|A<sub>1</sub> ∪ A<sub>2</sub> ∪ · · · ∪ A<sub>n</sub>| =|A<sub>1</sub>| + |A<sub>2</sub>| + · · · + |A<sub>n</sub>|.**

## Example 2 (Product Rule)
Bob orders **both soup and sandwich: 6 types of soups, 12 different sandwiches.** <br />
Bob must choose **one soup** and one sandwich. He has **6 ways to choose a soup and 12 ways to choose a sandwich.** <br />
Since any soup can be paired with any sandwich, there are **6 · 12 = 72 total different meals that he can order.** <br />
If in addition Bob were to choose a drink and there were eight possible drinks, Bob would then have **6 × 12 × 8 = 576** possible meal choices. The product rule can clearly be extended to this more general case. <br />
### Product Rule
If A and B are **finite sets** then the number of ways of choosing an element from **A and an element from B is |A × B| = |A| × |B|.**
- The product rule is applicable when **one must make two (or more) consecutive choices from sets of alternatives.**
	- **General Product Rule:** If A<sub>1</sub>, A<sub>2</sub>, . . . , A<sub>n</sub> are finite sets, then the number of ways of choosing an element from A<sub>1</sub>, A<sub>2</sub>, . . . , and an element from A<sub>n</sub> is **|A<sub>1</sub> × A<sub>2</sub> ×· · · × A<sub>n</sub>| = |A<sub>1</sub>| × |A<sub>2</sub>| ×  · · · × |A<sub>n</sub>|.**
## [Examples for these Rules](Chapter%208%20(Part%201)%20Examples.md#Example-84---Picking-Students)
***
# The Inclusion-Exclusion Principle
In the description of the [Sum Rule](#Sum-Rule), we assumed that the **sets of alternatives from which one must make a single choice were <u>mutually disjoint</u>**, i.e., that ***they did not share any common elements***. <br />
In situations when a **single choice must be made from sets of alternatives which are not disjoint**.
## Inclusion-Exclusion Principle
- If A and B are finite sets then **|A∪B| = |A|+|B| −|A∩B|**.
## [Examples for this Principle](Chapter%208%20(Part%201)%20Examples.md#Example-85)
***
# The Pigeonhole Principle
If **`k + 1` or more objects are placed in k boxes**, then there must exist a box that **contains two or more objects**. <br />
### For example:
- If **13 or more people gather in a room**, then it is guaranteed that **at least two of them share the same birth month**. While this may happen in a gathering of 12 or fewer people, it is not guaranteed.
## [Examples for this Principle](Chapter%208%20(Part%201)%20Examples.md#Example-88)
## Generalized Pigeonhole Principle
Suppose that {x<sub>1</sub>, x<sub>2</sub>, . . . , x<sub>n</sub>} is a collection of n numbers, and let x be the average of these numbers, i.e., <br />
![](Photos/Generalized%20Pigeonhole%20Principle%20Equation.png) <br />
Then it clearly cannot be the case that every number is less than the average; in other words, **there must exist at least one number that is at least as large as the average**.
- **Generalized Pigeonhole:** Principle If N objects are placed in k boxes, then there must exist a box that contains \[N/k\] or more objects.
## [Examples for this Generalized Principle](Chapter%208%20(Part%201)%20Examples.md#Example-813)
***
# Permutation
**Permutation** - An **ordered arrangement of a set (or subset) of objects**.
## Counting Permutations
![](Photos/Counting%20Permutations%20Equation.png) <br />
### Counting r-permutations
![](Photos/Counting%20r-Permutations%20Equation.png) <br />
Note that **r-permutations** are a generalization of permutations; indeed, and **n-permutation** is an ordered arrangement of all n out of n objects, and the number of such n-permutations is **P(n,n) = n!/0! = n!**.
## [Examples for Permutation](Chapter%208%20(Part%201)%20Examples.md#Permutation-Example---Errands)
***
# External Resources
## Here are a list of outside resources that might help you better understand Chapter 8 (Part 1)
I recommend that you right click and open in new tab for these links (it's better than going back and forth on the same tab)
### Inclusion Exclusion Principle
- #### [Wolfram MathWorld](https://mathworld.wolfram.com/Inclusion-ExclusionPrinciple.html)
- #### [GeeksforGeeks - Includes Programming Applications](https://www.geeksforgeeks.org/inclusion-exclusion-principle-and-programming-applications/)

### The Pigeonhole Principle
- #### [Baeldung - Overview + Generalized](https://www.baeldung.com/cs/pigeonhole-principle)
- #### [GeeksforGeeks](https://www.geeksforgeeks.org/discrete-mathematics-the-pigeonhole-principle/)
	- ##### [Pigeonhole Sort just for fun :3 (GeeksforGeeks)](https://www.geeksforgeeks.org/pigeonhole-sort/)

### Permutation
- #### [Khan Academy - Permutation Formula](https://www.khanacademy.org/math/precalculus/x9e81a4f98389efdf:prob-comb/x9e81a4f98389efdf:combinatorics-precalc/v/permutation-formula)
- #### [BYJU's - Definition, Formula, Types, and Examples](https://byjus.com/maths/permutation/)
