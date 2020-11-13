﻿# NumNinja: Numeric Dictionary Generator

## Description & Usage
A super-high speed numeric dictionary generator (2M+ lines per second), that generates a file with all the integers within a user-specified range, either by the Leading Zeros method; ideal in aiding dictionary attacks performed against a number-based pin system, or if the candidates to be tried are within—say—a specific range of contact numbers (example: if a specific network vendor's numbers start with either the digit 7 or 8, a list consisting of all integers 7000000000 → 8999999999 would be both more efficient and ideal in finding the correct possible candidate, than a list of the 0000000000 → 9999999999 range).

## Methods
### Leading Zeros Generation
This method generates integers within the user-defined constraints, **at a *constant* length**, for example:

0000
0001
0002
...
0068
0069
...
999
1000
...
9998
9999
10000

### Straightforward Generation
This method generates integers within the user-defined constraints, **at *incremental* lengths**, for example:

0 
1 
2 
... 
68
69
... 
999 
1000
... 
9998
9999
10000

<div align="center">
<img src="https://github.com/SHUR1K-N/NumNinja-Number-Dictionary-Generator/blob/master/Images/CUI%20Example.png" >
<p>NumNinja.py CUI</p>
</div>

<div align="center">
<img src="https://github.com/SHUR1K-N/NumNinja-Number-Dictionary-Generator/blob/master/Images/GUI%20Example.png" >
<p>NumNinja.py GUI</p>
</div>

This project was created in Python, and has both versions — graphical UI and console UI.

## Optimization
The extremely high integer-generation speeds are owed to the implementation of multiprocessing in this program (the regular version of the program is completely functional, but the much faster multiprocessing version is still an active work in progress).

## Dependencies to PIP-Install
- **tqdm** (for progress bars)
- **tkinter** (for GUI elements)
- **colorama** (for colors)
- **termcolor** (for colors)

------------

My website: http://bit.do/SHUR1KN
