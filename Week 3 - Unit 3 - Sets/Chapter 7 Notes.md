## Table of Contents

***
# Chapter 7: Sets - Notes Simplified
**Sets** - An unordered collection of objects or **elements** <br />
There are different kinds of sets that could include elements like:
- Rational Numbers
- Both Negative and Positive Integers
- Rational Numbers
- Real Numbers
- Letters <br />
### Some Sets and Their Corresponding Symbols
![](Photos/Some%20Sets%20of%20Numbers.png) <br />
We use **braces (curly brackets, aka these -> `{ }`)** to show the elements of a set.

# Set Basics
**x ∈ S** - if x is an element of S (x is in S) <br />
**x ∉ S** - if x is NOT in S <br />

Two sets are only **equal** if they both  **have the same elements**: 
`{a, b, c} = {b, c, a} = {c, b, a}` <br />

 **Finite Set** - A set that has a **finite number of elements**. The **cardinality or size** of the set is the **number of elements it contains**.  <br />
- To denote the cardinality of S, we use **| S |** - If `S = {1, 2, 5, 7}` then | S | = 4 <br />

**Cardinality** is also defined for **infinite sets** which are just sets with **infinitely many elements**.
- Even though both R and Z have infinitely many elements, they do not have the same cardinality. In fact, there are an infinite number of different infinities, based on **Theory of Computation**. <br />

**Empty Set** - a set with no elements at all. Denoted with: ∅ or `{ }` <br />

When you declare a set variable in computing, it is an empty set until you put something in it. <br />
![](Photos/Set%20Example%201.png) <br />

## Set Builder Notation
When we need to **describe which elements are in the set** instead of just leaving it to the reader to figure out how to continue a list, we use **set-builder notation.** <br />
![](Photos/set%20builder%20notation.png) <br />
Where v is a variable and S is a set. The braces { and } tell us to say “the set of" and the vertical bar '|' is read as “such that." We sometimes use a colon “:" in place of the vertical bar. <br />
`{v| condition on v}` is read as “the set of v such that" the condition on v holds. <br />
`{v ∈ S| condition on v}` is read as “the set of v in S such that" the condition on v holds. <br />


## Set Operations
### Union ∪
![](Photos/Union%20venn%20diagram.png) <br />
![](Photos/Union%20example.png)

### Intersection ⋂
![](Photos/intersection%20venn%20diagram.png) <br />
![](Photos/Intersection%20example.png)

### Complement ∁
![](Photos/Compliment%20venn%20diagram.png)
![](Photos/Complement%20example.png) <br />
So for example. if set A already has elements that exists in set U, you just get rid of the same elements in A within set U.

### Difference
![](Difference%20venn%20diagram.png) <br />
![](Photos/Difference%20example.png) <br />
I feel like this is self explanatory. But pretty much, if set A has elements that already exist or don't exist on set B, you get rid of the same elements within the set, then the remaining elements will remain.