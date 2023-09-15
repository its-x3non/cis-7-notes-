# Chapter 8 (Part 1): Counting - Notes Simplified
## Table of Contents
***
**Combinatorics** - A branch of mathematics largely concerned with counting discrete objects <br />
Many problems in comp sci involve **counting** possible solutions, **enumerating** those solutions, or **finding** the optimal solution among a candidate set.

## Example 1 (Sum Rule):
Alice order soup or sandwich: **6 types of soups, 12 different sandwiches.** <br />
Alice must choose **either one of six soups or one of 12 sandwiches** for a total of **6 + 12 = 18 different meals** <br />
### **Sum Rule:** If A and B are **disjoint finite sets** then the number of ways of choosing a **single element** from **A or B is |A ∪ B| = |A| + |B|.**
- The sum rule is applicable when one must make one choice from the union of two (or more) sets of alternatives; sum rule can be generalized to more than two sets of alternatives in an obvious way.
- **General Sum Rule:** If A<sub>1</sub>, A<sub>2</sub>, . . . , A<sub>n</sub> are mutually disjoint finite sets then the number of ways of choosing a single element from A<sub>1</sub>, A<sub>2</sub>, . . . , or An is **|A<sub>1</sub> ∪ A<sub>2</sub> ∪ · · · ∪ A<sub>n</sub>| =|A<sub>1</sub>| + |A<sub>2</sub>| + · · · + |A<sub>n</sub>|.**

## Example 2 (Product Rule):
Bob orders **both soup and sandwich: 6 types of soups, 12 different sandwiches.**
Bob must choose **one soup** and one sandwich. He has **6 ways to choose a soup and 12 ways to choose a sandwich.** <br />
Since any soup can be paired with any sandwich, there are **6 · 12 = 72 total different meals that he can order.** <br />
If in addition Bob were to choose a drink and there were eight possible drinks, Bob would
then have **6 × 12 × 8 = 576** possible meal choices. The product rule can clearly be extended
to this more general case. <br />
### **Product Rule:** If A and B are **finite sets** then the number of ways of choosing an element from **A and an element from B is |A × B| = |A| × |B|.**
- The product rule is applicable when **one must make two (or more) consecutive choices from sets of alternatives.**
- **General Product Rule:** If A<sub>1</sub>, A<sub>2</sub>, . . . , A<sub>n</sub> are finite sets, then the number of ways of choosing an element from A<sub>1</sub>, A<sub>2</sub>, . . . , and an element from A<sub>n</sub> is **|A<sub>1</sub> × A<sub>2</sub> ×· · · × A<sub>n</sub>| = |A<sub>1</sub>| × |A<sub>2</sub>| ×  · · · × |A<sub>n</sub>|.**

## Example 8.1
Personal Identification Numbers or PINs are entered on a numeric keypad and, hence made up entirely of digits. The PINs on our office locks are required to be exactly 4 digits. How many different PINs are possible? <br />
<u>The set of digits, D = 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 has cardinality 10.</u> Each PIN corresponds to an element of **D × D × D × D**. There are **104 = 10,000** different PINs.
### A. How many different 7 digit PINs are there?
- 10<sup>7</sup> = 10,000,000.
### B. How many different 4 to 7 digit PINs are there?
- A single PIN has either 4 or 5 or 6 or 7 digits. We use the product rule to separately count the sets of 4-digit, 5-digit, 6-digit, and 7-digit passwords then use the sum rule to count the union of these sets. The number of 4 to 7 digit pins is 10<sup>4</sup> + 10<sup>5</sup> +10<sup>6</sup> + 10<sup>7</sup> = 11,110,000.

## Example 8.2
Passwords are often composed of alpha-numeric characters, a, b, ..., z, 0, 1, 2, ..., 9 on systems that are not case-sensitive or A, B, ..., Z, a, b, ..., z, 0, 1, 2, ..., 9 on systems that are case-sensitive.
### A. How many **4-character alpha-numeric passwords** are there if you can use **upper- and lower- case letters and digits** (i.e. case-sensitive)?
- There are 26 upper-case letters, 26 lower-case letters, and 10 digits for a character.
- Set C of size 62 = (26+26+10). The total number of possible passwords is: **|C × C × C × C| = (62)4 = 14,776,336.**
### B. If a hacker has code that can try out passwords on a system at a rate of **1 per second**, how long would it take her to break into a system that
#### a) Uses 4-digit passwords? (numeric: 0-9)
- 10<sup>4</sup> = 10,000 seconds = 2 hours 46 minutes 40 seconds.
#### b) Uses 4-character case-sensitive, alpha-numeric passwords?
- 14,776,336 seconds = 171 days 32 minutes 16 seconds