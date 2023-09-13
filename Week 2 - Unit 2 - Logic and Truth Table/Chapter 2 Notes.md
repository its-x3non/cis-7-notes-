# Chapter 2: Circuits - Notes Simplified
## Table of Contents
- [Transistors and Switches](#Transistors-and-Switches)
- [Basic Logic Gates: AND, OR, NOT](#Basic-Logic-Gates:-AND,-OR,-NOT)
	- [AND Gate](#AND-Gate)
	- [OR Gate](#OR-Gate)
	- [NOT Gate](#NOT-Gate)
	- [NAND Gate](#NAND-Gate)
	- [NOR Gate](#NOR-Gate)
	- [XOR Gate](#XOR-Gate)
***
# Transistors and Switches
**Transistor** - A digital switch that's used to either establish or break an electrical connection. <br />

# Basic Logic Gates: AND, OR, NOT
## AND Gate
The **AND Gate** takes 2 inputs (switches). If both switches have been pushed, then the output is "ON". <br />
![](Photos/Chapter%202/AND%20Gates/AND%20Gate%201.png) <br />

In a computer, there are four possible input pairs to the AND Gate. When given A or B is either 0 or 1. <br />
![](Photos/Chapter%202/AND%20Gates/AND%20Gate%202.png) <br />

### Truth Table
| A   | B   | A (AND) B |
| --- | --- | --------- |
| 0   | 0   | 0         |
| 0   | 1   | 0         |
| 1   | 0   | 0         |
| 1   | 1   | 1          |
 <br />

## OR Gate
The **OR Gate** also take 2 inputs, but is "ON" if at least 1 of the inputs is switched "ON". <br />
![](Photos/Chapter%202/OR%20Gates/OR%20Gate%20Diagram.png) <br />

## NOT Gate
The **NOT Gate** only has 1 input, and is basically the opposite of it's input.
![](Photos/Chapter%202/NOT%20Gates/NOT%20Gate%20Diagram.png) <br />

## NAND Gate
The **NAND Gate** is pretty much the opposite of the [AND Gate](#AND-Gate). A **NAND Gate** is constructed using an [AND Gate](#AND-Gate) whose output is attached to a [NOT Gate](#NOT-Gate). <br />
- A NAND Gate is the simplest logic gate to construct from common electrical components.
- The NAND gate is "logically complete" in that every conceivable truth table, logic gate, or circuit can be constructed solely from NAND Gates. <br />
![](Photos/Chapter%202/NAND%20Gates/NAND%20Gates%201.png) <br />
### Truth Table
| A   | B   | A (NAND) B |
| --- | --- | --------- |
| 0   | 0   | 1         |
| 0   | 1   | 1         |
| 1   | 0   | 1         |
| 1   | 1   | 0          |
 <br />

## NOR Gate
The **NOR Gate** is pretty much the opposite of the [OR Gate](#OR-Gate). A **NOR Gate** is constructed using an [OR Gate](#OR-Gate) whose output is attached to a [NOT Gate](#NOT-Gate). <br />
![](Photos/Chapter%202/NOR%20Gates/NOR%20Gate%20Diagrams.png) <br />
## XOR Gate
The **XOR Gate** is the **"exclusive OR"** gate. It's only 1 (on) if only ONE of the inputs is 1, not both. <br />
The **XOR gate** gives the proper output of the *least* significant bit in adding two bits, and
further note that an **[AND Gate](#AND-Gate)** gives the proper output of the *most* significant bit (or carry) in adding two bits. <br />
![](Photos/Chapter%202/XOR%20Gates/XOR%20Gate%20diagram.png)