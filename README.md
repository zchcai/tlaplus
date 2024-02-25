# Learning TLA+

This repo records my learning notes for [TLA+](https://lamport.azurewebsites.net/tla/tla.html).

TLA+ is a programming language to model programs or systems to identify fundamental errors in algorithms or designs.
It belongs to the family of [model checking](https://link.springer.com/chapter/10.1007/BFb0058022), along with other tools like [SPIN](https://spinroot.com/spin/whatispin.html), [(C|J|E)BMC](https://www.cprover.org/), etc.
The active community is a direct reason I chose to learn it recently, especially when [Leslie Lamport](https://en.wikipedia.org/wiki/Leslie_Lamport) [shared his new TLA+ book draft](https://groups.google.com/g/tlaplus/c/r-7eP7O_Lf8) on January 3rd, 2024.
Receiving feedback is crucial for me, or at least very beneficial and necessary, to understand new concepts thoroughly and apply them in daily work.

The notes here have no finalized format and may keep changing, and the content only represents my understanding.
If you find any incorrectness, welcome to fill an issue! Very appreciated!

## Getting Started

### Install (win)

Click to download https://github.com/tlaplus/tlaplus/releases/download/v1.7.1/TLAToolbox-1.7.1-win32.win32.x86_64.zip, unzip it and replace the `tla2tools.jar` with the latest version (click [here](https://github.com/tlaplus/tlaplus/releases/download/v1.7.3/tla2tools.jar) to download).

### Download Tutorial Files

Click and download https://lamport.azurewebsites.net/tla/tutorial/original-specs.zip, unzip and save a copy to a folder you will experiment with.

#### Correction to original files

##### Session1.tla:
- add "Sequences" at line 2: EXTENDS Integers, Sequences
  - Otherwise, when following 2.4 Tuples at Session 1, you will see 1 error in Expression: detected Unknown operator: `Len'.

### Follow PlusCal Tutorial

Go to https://lamport.azurewebsites.net/tla/tutorial/session1.html.
The tutorial is very detailed and easy to follow.
