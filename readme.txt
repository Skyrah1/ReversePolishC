----------------------------
What is reverse-polish.zip?
----------------------------

This zip file contains 6 files:
- stacks.c
- stacks.h
- trees.c
- trees.h
- reverse-polish.c (main function)
- A Makefile to compile reverse-polish.c with stacks.c and trees.c
  (written to save you time)

stacks.c and trees.c act as modules for reverse-polish.c, which uses stacks
and trees to solve equations in Reverse Polish notation (postfix), as well
as infix equations.

----------------------------
How do we use it?
----------------------------

Open up the zip file, make the program and type one of the following into the
console:

    > ./reverse-polish
    (runs automated tests);

    > ./reverse-polish rp
    (solves an equation in reverse polish notation, with each integer/operator
    entered one at a time)

    > ./reverse-polish infix
    (solves an equation in infix notation, taking in the entire equation at
    once)

----------------------------
Limitations
----------------------------
- The infix solver can only solve equations with one operator outside each set
  of brackets.
  e.g. 1 * 2 is solvable
       (3 / 1) + 100 is solvable
       (2 * 3) / (5 MOD (10 - 8)) is solvable
       3 + 3 + 3 is NOT solvable
       (10 + 4 - 2) MOD 5 is NOT solvable
