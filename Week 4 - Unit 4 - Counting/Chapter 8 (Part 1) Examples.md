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
# Example 8.4 - Picking Students
Suppose that there are three sections of a discrete structures class containing 73, 64, and 41 students, respectively.  
## a) How many distinct ways are there of choosing one discrete structures student to write up a sheet of notes for everyone to use at the final?  
- The **[Sum Rule](Chapter%208%20(Part%201)%20Notes.md#Sum-Rule)** applies, yielding **73 + 64 + 41 = 178 possibilities**.  
## b) How many distinct ways are there of <u>choosing one discrete structures student</u> from each class to form an advisory committee?  
- The [Product Rule](Chapter%208%20(Part%201)%20Notes.md#Product-Rule) applies, yielding **73 · 64 · 41 = 191,552**.  
## c) How many distinct ways are there of <u>listing six different discrete structures students from a 41 person section</u> to go to the board <u>one after the other to present problem</u> solutions?  
- Consider the choices that must be made in generating such a section. There are **41 students to choose from as the first presenter**, but then there are only **40 students to choose from as the second presenter**, 39 as the third presenter and so on. Note that multiple choices must be made (so the product rule applies) and the size of the sets of alternatives (from which these choices must be made) shrinks with each successive choice. The result is **41 · 40 · 39 · 38 · 37 · 36 = 3,237,399,360**.  <br />
	- This is an example of **permutations**, which is discussed in more detail in Section 8.4.
## d) How many distinct ways are there of choosing <u>six discrete structures students to form the course volleyball team</u>?
- Now we have to **choose a set of six students out of the 178 discrete structures students**. If we count the ways to make a list of 6 students, as in c, we get **178 · 177 · 176 · 175 · 174 · 173 possible ordered lists of 6 students**.  
- **Each set of 6 students appears** in this list **6! = 6 · 5 · 4 · 3 · 2 · 1** times so the number of sets is of six students out of the 178 is  
	- This is an example of **combinations**, which is discussed in more detail in Section 8.5.
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