# Will It Assemble?

A learning game for x86 assembly (AT&T syntax), built around five in-class practice sets:

- **Part 1 · Moving Data** — operand kinds, suffix sizes, register names, and the rules that make a `mov` legal.
- **Part 2 · Memory Addressing** — `D(Rb,Ri,S)` built up one piece at a time, with register and memory tables.
- **Part 3 · Control Flow** — `cmp` order, the four flags one at a time, `set`, conditional jumps, if and loops.
- **Part 4 · Procedures** — the stack, `call` and `ret`, argument registers, and stack frames.
- **Part 5 · Arrays** — type sizes, declarations, element addresses, pointer math, and `lea` vs `mov`.
- **Review** — four shuffled mixes that pick new questions every replay, plus a Lab that works out any instruction, operand or flag result step by step.

The whole game is a single file, `index.html`, with no build step and no dependencies beyond Google Fonts.

## Run it locally

Open `index.html` in a browser. That's it.

Progress (XP and level blocks) is saved in each visitor's own browser with `localStorage`, so nothing is stored on the server and every classmate gets their own progress.

## Editing questions

Questions live in the `LEVELS` array inside `index.html`, one object per level. Each level has a `lesson` (HTML) and a list of `qs`. The answer checkers (`analyze` for mov instructions, `solveOperand` for addressing, `solveFlags` for the Lab's condition codes) generate worked explanations automatically.
