## Table of Contents
- Example 8.1
- Example 8.2
- Example 8.3
- Example 8.4 - Picking Students
- Example 8.5
- Example 8.6
- Example 8.7
- Example 8.8
- Example 8.9
- Example 8.10
- Example 8.11
- Example 8.12
- Example 8.13
***
# Example 8.1
Personal Identification Numbers or PINs are entered on a numeric keypad and, hence made up entirely of digits. The PINs on our office locks are required to be exactly 4 digits. How many different PINs are possible? <br />
<u>The set of digits, D = 0, 1, 2, 3, 4, 5, 6, 7, 8, 9 has cardinality 10.</u> Each PIN corresponds to an element of **D × D × D × D**. There are **10<sup>4</sup> = 10,000** different PINs.
## A. How many different 7 digit PINs are there?
- **10<sup>7</sup> = 10,000,000.**
## B. How many different 4 to 7 digit PINs are there?
- A single PIN has either 4 or 5 or 6 or 7 digits. We use the product rule to separately count the sets of 4-digit, 5-digit, 6-digit, and 7-digit passwords then use the sum rule to count the union of these sets. The number of 4 to 7 digit pins is **10<sup>4</sup> + 10<sup>5</sup> +10<sup>6</sup> + 10<sup>7</sup> = 11,110,000.**
***
# Example 8.2
Passwords are often composed of alpha-numeric characters, a, b, ..., z, 0, 1, 2, ..., 9 on systems that are not case-sensitive or A, B, ..., Z, a, b, ..., z, 0, 1, 2, ..., 9 on systems that are case-sensitive.
## A. How many <u>4-character alpha-numeric passwords</u> are there if you can use <u>upper- and lower- case letters and digits </u>(i.e. case-sensitive)?
- There are 26 upper-case letters, 26 lower-case letters, and 10 digits for a character.
- Set C of size 62 = (26+26+10). The total number of possible passwords is: **|C × C × C × C| = (62)4 = 14,776,336.**
## B. If a hacker has code that can try out passwords on a system at a rate of <u>1 per second</u>, how long would it take her to break into a system that
### a) Uses 4-digit passwords? (numeric: 0-9)
- 10<sup>4</sup> = 10,000 seconds = 2 hours 46 minutes 40 seconds.
### b) Uses 4-character case-sensitive, alpha-numeric passwords?
- 14,776,336 seconds = 171 days 32 minutes 16 seconds
***
# Example 8.3  
**Bit strings** are strings composed of **0s and 1s**.  
## A. How many <u>bit strings</u> are there with <u>8 bits</u>?  
- 2<sup>8</sup> = 256.  
## B. How many <u>bit strings</u> are there with <u>16 bits</u>?  
- 2<sup>16</sup> = 65,536.  
## C. What is <u>the largest integer</u> that can be represented in <u>16-bit two’s complement</u>?  
Since **positive integers in two’s complement must have a 0 in the leftmost position**, we have only **15 places to represent the magnitude of the integer.** The largest integer we can represent  
is **0111 1111 1111 1111 = 2<sup>15</sup> − 1 = 32767**
***
# Read About the [Product Rule](Chapter%208%20(Part%201)%20Notes.md#Product-Rule) and the [Sum Rule](Chapter%208%20(Part%201)%20Notes.md#Sum-Rule) in the Notes Before Going to the Next Examples
***
# Example 8.4 - Picking Students
Suppose that there are three sections of a discrete structures class containing 73, 64, and 41 students, respectively.  
## a) How many distinct ways are there of choosing one discrete structures student to write up a sheet of notes for everyone to use at the final?  
- The **[Sum Rule](Chapter%208%20(Part%201)%20Notes.md#Sum-Rule)** applies, yielding **73 + 64 + 41 = 178 possibilities**.  
## b) How many distinct ways are there of <u>choosing one discrete structures student</u> from each class to form an advisory committee?  
- The **[Product Rule](Chapter%208%20(Part%201)%20Notes.md#Product-Rule)** applies, yielding **73 · 64 · 41 = 191,552**.  
## c) How many distinct ways are there of <u>listing six different discrete structures students from a 41 person section</u> to go to the board <u>one after the other to present problem</u> solutions?  
- Consider the choices that must be made in generating such a section. There are **41 students to choose from as the first presenter**, but then there are only **40 students to choose from as the second presenter**, 39 as the third presenter and so on. Note that multiple choices must be made (so the product rule applies) and the size of the sets of alternatives (from which these choices must be made) shrinks with each successive choice. The result is **41 · 40 · 39 · 38 · 37 · 36 = 3,237,399,360**.  <br />
	- This is an example of **permutations**, which is discussed in more detail in Section 8.4.
## d) How many distinct ways are there of choosing <u>six discrete structures students to form the course volleyball team</u>?
- Now we have to **choose a set of six students out of the 178 discrete structures students**. If we count the ways to make a list of 6 students, as in c, we get **178 · 177 · 176 · 175 · 174 · 173 possible ordered lists of 6 students**.  
- **Each set of 6 students appears** in this list **6! = 6 · 5 · 4 · 3 · 2 · 1** times so the number of sets is of six students out of the 178 is  
	- This is an example of **combinations**, which is discussed in more detail in Section 8.5.
***
# Read About the [Inclusion-Exclusion Principle](Chapter%208%20(Part%201)%20Notes.md#Inclusion-Exclusion-Principle) in the Notes Before Going to the Next Examples
***
# Example 8.5
More Passwords Suppose passwords are restricted to **6 case-sensitive alpha-numeric characters** and **must contain at least 1 digit and at least 1 letter**. How many are there?
- There are **(62)<sup>6</sup> passwords** composed of **6 case-sensitive alpha-numeric characters** with no other restrictions. Of these, **(52)<sup>6</sup> are composed of letters only and (10)<sup>6</sup> are composed of digits only. All the others have at least one digit and at least one letter.** So the answer is: 
	- \[(62)<sup>6</sup> − (52)<sup>6</sup> − (10)<sup>6</sup>\].
Suppose passwords may have **6 to 10 case-sensitive alpha-numeric characters and must contain at least 1 digit and at least 1 letter**. How many are there?
- Since a password may have **6, 7, 8, 9, or 10 letters**, we can **count each of these possibilities separately and apply the [Sum Rule](Chapter%208%20(Part%201)%20Notes.md#Sum-Rule)** to get the result:
	- \[(62)<sup>6</sup>−(52)<sup>6</sup>−(10)<sup>6</sup>\]+\[(62)7<sup>7</sup>−(52)<sup>7</sup>−(10)<sup>7</sup>\]+\[(62)<sup>8</sup>−(52)<sup>8</sup>−(10)<sup>8</sup>\]+\[(62)<sup>9</sup>−(52)<sup>9</sup>−(10)<sup>9</sup>\]+\[(62)<sup>10</sup>−(52)<sup>10</sup>−(10)<sup>10</sup>]
***
# Example 8.6
How many strings of **6 upper-case letters start with A or end with Z**?  
- **26<sup>5</sup> start with A.**  
- **26<sup>5</sup> end with Z.**  
- **26<sup>4</sup> start with A and end with Z and they were counted twice.** 
	- The answer is:
		- **26<sup>5</sup> + 26<sup>5</sup> − 26<sup>4</sup>**
***
# Example 8.7
How many **positive integers between 1000 and 9999 inclusive** (There are 9000 consecutive integers = (9999-1000)+1)  
## a) Are divisible by 9?  
- Every **9th integer is divisible by 9 and 9 divides 9000 evenly so there are 1000**.  
## b) Are even?  
- Half the integers are even and **2 divides 9000 evenly so 4500 are even**.  
## c) Have distinct digits?  
- Integers between 1000 and 9999 all have 4 digits and the **leftmost digit cannot be 0 so there are 9 choices**. The **second digit can be any digit but the first so there are 9 choices**. There are **8 choices for the third digit and 7 for the fourth**. 
- By the **[Product Rule](Chapter%208%20(Part%201)%20Notes.md#Product-Rule)**, **9 × 9 × 8 × 7 = 4536** have distinct digits.  
## d) Are not divisible by 3?  
- **Every 3rd integer is divisible by 3 and 3 divides 9000 evenly so there are 3000 that are divisible by 3** and **9000 − 3000 = 6000 that are not divisible by 3**.  
## e) Are divisible by 5 or 7? Use the [Inclusion-Exclusion Principle](Chapter%208%20(Part%201)%20Notes.md#Inclusion-Exclusion-Principle) here.
- We compute **the number divisible by 5 plus the number divisible by 7 minus the number divisible by both** (i.e. divisible **by 35**).  
	- **Divisible by 5: 9000/5 = 1800**  
	- **Divisible by 7: 9000/7 = 1285.71429 . . . so there are either 1285 or 1286.**
- This take some extra checking, e.g. there are 3 integers from 4 to 12 that are
	- Divisible by **4 (4, 8, 12) but only 2 integers from 3 to 11 (4, 8) that are divisible by 4**. The range in each case includes 9 integers and **9/4 = 2.25**.  
	- The first integer starting at **1000 that is divisible by 7 is 1001** and **1001 + 7 · 1285 = 1001 + 8995 = 9996** so the answer is 1286.  
	- Divisible by 35: **9000/35 = 257.142857**
		- The first integer starting at **1000** that is divisible by 35 is 1015 and **1015 + 35 · 257 = 10010 > 9999** so the answer is **257** (not 258).
- Now we apply the **[Inclusion-Exclusion Principle](Chapter%208%20(Part%201)%20Notes.md#Inclusion-Exclusion-Principle)**. The number divisible by 5 plus the number divisible by 7 minus the number divisible by both is **1800 + 1286 − 257 = 2829.**  
	- ### f) Are not divisible by either 5 or 7?  
		- This is **9000 minus the number that are divisible by 5 or 7, 9000 − 2829 = 6171.**  
	- ### g) Are divisible by 5 but not by 7?  
		- This is the number divisible by **5 but not divisible by 35, 1800 − 257 = 1543**.  
	- ### h) Are divisible by 5 and 7? 
		- This is the same as the number divisible by **35 which is 257**
***
# Read About the [Pigeonhole Principle](Chapter%208%20(Part%201)%20Notes.md#The-Pigeonhole-Principle) in the Notes Before Going to the Next Examples
***
# Example 8.8
Suppose that there are **102 students in two sections of discrete structures**. If they all take the final, will **at least two of them get the same grade**?  
- There are **101 possible grades 0, 1, . . . , 100** so the result follows from the pigeonhole principle
***
# Example 8.9
If I use the last **two digits of their social security numbers as a code to post grades in anonymity**, will **at least two students get the same code**?  
- There are 1**00 2-digit codes, 00 through 99** so by the time I **list the first 101 students there will be two with the same code**.
***
# Example 8.10
If a drawer contains **12 red socks and 12 blue socks** and I pull some socks out in the dark,  
## a) How many must I pull out to be sure of having a pair?  
- **3** because there are only **2 colors**.
## b) How many must I pull out to be sure of having a pair of red socks?  
- **14** because I might pull out **all the blue ones and just 2 red ones**.  
## c) How many must I pull out to be sure of having at least one of each color?  
- **13** because I might pull out all **12 of one color and just one of the other color**.
***
# Example 8.11
**Every integer n** has a multiple that has only 0s and 1s in its decimal expansion.
## Proof
Consider the n + 1 numbers 1, 11, . . . , 11111...11 where the last number has (n + 1) ones. If we evaluate each of these numbers <u>mod n</u>, two of them must give the same value as there are only n possible results, 0, . . . , n − 1. If then a − b is divisible by n. So take the two numbers that result in the same value and subtract the smaller from the larger. The result is a multiple of n and has only 0s and 1s in its decimal expansion.
### Example
Take n = 6. <br />
1 mod 6 = 1  <br />
11 mod 6 = 5  <br />
111 mod 6 = 3  <br />
1111 mod 6 = 1  <br />
so 1111 − 1 = 1110 is a multiple of 6. <br />
***
# Example 8.12
In any set of **n + 1 positive integers not exceeding 2n**, there must be one integer that divides another.  <br />
Write each of the n + 1 integers as a power of 2 times an odd integer, a<sub>j</sub> = 2e<sub>j</sub> q<sub>j</sub>. <br />  
Then q<sub>1</sub> . . . q<sub>n+1</sub> are **n+ 1 odd integers less than 2n**. Two of them must be the same.  <br />
One of the corresponding a<sub>j</sub>s divides the other. <br />
***
***
