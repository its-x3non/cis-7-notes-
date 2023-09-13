# Chapter 3: Logic - Notes Simplified
## Table of Contents
- [Truth Table](#Truth-Table)
	- [AND Rules](#AND-Rules)
	- [OR Rules](#OR-Rules)
	- [NOT Rules](#NOT-Rules)
	- [NAND (NOT AND) Rules](#NAND-(NOT-AND)-Rules)
	- [NOR (NOT OR) Rules](#NOR-(NOT-OR)-Rules)
- [Logical Equivalent](#Logical-Equivalent)
	- [Laws of Boolean Algebra](#Laws-of-Boolean-Algebra)
- [Normal Form](#Normal-Form)
	- [Conjunctive Normal Form](#Conjunctive-Normal-Form)
		- [Formulae in CNF](#Formulae-in-CNF)
		- [Formulae NOT in CNF](#Formulae-NOT-in-CNF)
	- [Disjunctive Normal Form](#Disjunctive-Normal-Form)
***
The basic operators of Boolean algebra correspond to the Basic Logic Gates. <br />
![](Photos/Chapter%203/Basic%20Operators%20-%20Basic%20Logic%20Gates.png) <br />

# Truth Table
In logic, variables may take on one of **two truth values (T or F)**. These values are manipulated and combined by various logical operators. The actions of these logical operators are typically defined using **truth tables**, in a manner identical to the use of these truth tables in defining the actions of logic gates. <br />
![](Photos/Chapter%203/Truth%20Table%20for%20BASIC%20LOGIC%20GATES.png) <br />
From LEFT to RIGHT: [AND](Chapter%202%20Notes#AND-Gate), [OR](Chapter%202%20Notes#OR-Gate), [NOT](Chapter%202%20Notes#NOT-Gate). <br />

## AND Rules
| Input 1 | Input 2 | AND   | Output |
| ------- | ------- | ----- | ------ |
| P       | Q       | P ∧ Q | Output |
| 0       | 0       | 0 ∧ 0 | 0      |
| 0       | 1       | 0 ∧ 1 | 0      |
| 1       | 0       | 1 ∧ 0 | 0      |
| 1       | 1       | 1 ∧ 1 | 1       |

## OR Rules
| Input 1 | Input 2 | OR   | Output |
| ------- | ------- | ----- | ------ |
| P       | Q       | P V Q | Output |
| 0       | 0       | 0 V 0 | 0      |
| 0       | 1       | 0 V 1 | 1      |
| 1       | 0       | 1 V 0 | 1      |
| 1       | 1       | 1 V 1 | 1      |

## NOT Rules
| Input | NOT | Output |
| ----- | --- | ------ |
| P     | ¬P  | Output |
| 0     | ¬0  | 1      |
| 1     | ¬1  | 0       |

## NAND (NOT AND) Rules
| Input 1 | Input 2 | Output   |
| ------- | ------- | -------- |
| P       | Q       | P NAND Q |
| 0       | 0       | 1        |
| 0       | 0       | 1        |
| 1       | 0       | 1        |
| 1       | 1       | 0        |

## NOR (NOT OR) Rules
| Input 1 | Input 2 | NOR    |
| ------- | ------- | ------ |
| P       | Q       | Output |
| 0       | 0       | 1      |
| 0       | 1       | 0      |
| 1       | 0       | 0      |
| 1       | 1       | 0       |
<br />

Other logical operators exist, including exclusive-OR (XOR) represented by the ⊕ symbol. And its equivalence (XNOR) represented by the ≡ symbol.
- Truth Tables can be used to represent much more than just actions of primitive logical operators.
- Truth tables can represent the arbitrary input/output behavior or Boolean (logical) formulae or circuits. One goal of logic design is to find efficient implementations of truth tables and their corresponding Boolean formulae using logic gates.
**XOR**: Exclusive OR or exclusive disjunction is a logical operator that outputs true only when inputs differ. (One is true, the other is false).
# Logical Equivalent
Two Boolean formulae are said to be logically equivalent if they have the same truth table; they perform the same actions on their inputs. For example, ⌐(⌐p) is logically equivalent to p and this is typically written ⌐(⌐p) ≡ p.

### Table 3.3 - Truth table for the Boolean Formula ¬p ∧ (q V ¬r)
| p   | ¬p  | ¬¬p |
| --- | --- | --- |
| 0   | 1   | 0   |
| 1   | 0   | 1   |

| p   | q   | ¬(p V q) | ¬p ∧ ¬q |
| --- | --- | -------- | ------- |
| F   | F   | T        | T       |
| F   | T   | F        | F       |
| T   | F   | F        | F       |
| T   | T   | F        | F        |

### Laws of Boolean Algebra
![](Photos/Chapter%203/Laws%20of%20Boolean%20Algrebra.png) <br />
#### Example of the [Laws of Boolean Algebra](#Table-3.4---Laws-of-Boolean-Algebra) in Use
![](Photos/Chapter%203/Example%20of%20the%20Laws%20of%20Boolean%20Algebra%20in%20Use.png)

# Normal Form
## Conjunctive Normal Form
A Boolean formula is in **Conjunctive Normal Form (CNF)** if it is a conjunction (∧) of clauses, where each clause is a disjunction of (V) of variables. <br />
A **CNF** is an approach to Boolean logic that expresses formulas as conjunctions of classes with an AND or OR. Each clauses connected by a conjunction, or AND, must be either a literal or contain a disjunction, or OR operator. <br />
For Example:
- (A OR B) AND (C OR D)
- (A OR B) AND (NOT C OR B)

### Formulae in CNF
| Formula                                | Clauses |
| -------------------------------------- | ------- |
| A ∧ ¬B ∧ (B V C)                       | A, ¬B, B V C        |
| (A V B V ¬C) ∧ (¬B V A V D) ∧ (F V ¬E) | A V B V ¬C, ¬B V A V D, F V ¬E        |
| A ∧ B                                  | A, B        |
| A V B                                       | A V B        |
### Formulae NOT in CNF
| Formula           | Causes            |
| ----------------- | ----------------- |
| A ∧ ¬B ∧ ¬(B V C) | ¬ outside (B V C) |
| (A ∧ B) V ¬C                  | Both a disjunction and one clause, *A ∧ B* is a conjunction                  |

#### Double Negation:  
1. P↔¬(¬P)P↔¬(¬P)  
##### De Morgan's Laws  
2. ¬(P⋁Q)↔(¬P)⋀(¬Q)¬(P⋁Q)↔(¬P)⋀(¬Q)  
3. ¬(P⋀Q)↔(¬P)⋁(¬Q)¬(P⋀Q)↔(¬P)⋁(¬Q)  
##### Distributive Laws  
4. (P⋁(Q⋀R))↔(P⋁Q)⋀(P⋁R)(P⋁(Q⋀R))↔(P⋁Q)⋀(P⋁R)  
5. (P⋀(Q⋁R))↔(P⋀Q)⋁(P⋀R)(P⋀(Q⋁R))↔(P⋀Q)⋁(P⋀R)  

So let’s expand the following: (equivalent to the expression in question)
1. (((A⋀B)⋁(C⋀D))⋁E)(((A⋀B)⋁(C⋀D))⋁E) Now using 4.  
We get:  
2. ((A⋀B)⋁C)⋀((A⋀B)⋁D))⋁E((A⋀B)⋁C)⋀((A⋀B)⋁D))⋁E And using 4. again  
3. ((((A⋁C)⋀(B⋁C))⋀((A⋁D)⋀B⋁D)))⋁E)((((A⋁C)⋀(B⋁C))⋀((A⋁D)⋀B⋁D)))⋁E) which gives:  
4. (((A⋁C)⋀(B⋁C))⋁E)⋀((A⋁D)⋀B⋁D))⋁E)(((A⋁C)⋀(B⋁C))⋁E)⋀((A⋁D)⋀B⋁D))⋁E)  
5. (A⋁C⋁E)⋀(B⋁C⋁E)⋀(A⋁D⋁E)⋀(B⋁D⋁E)

*I will color code this once I have a complete understanding of this part*

## Disjunctive Normal Form
A Boolean formula is in **Disjunctive Normal Form (DNF)** if its a disjunction (V) of clauses, where each clauses is a conjunction (⋀) of variables.