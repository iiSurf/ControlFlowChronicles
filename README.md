# Will It Assemble?

Check out [ControlFlowChronicles](https://iisurf.github.io/ControlFlowChronicles/) to play the game and learn at the same time.

A learning game for a computer systems class: x86 assembly (AT&T syntax), the memory hierarchy, caches and virtual memory, in twelve parts.

**x86 assembly** (In-Class Practice 1–5)

- **Part 1 · Moving Data**: operand kinds, suffix sizes, register names, and the rules that make a `mov` legal.
- **Part 2 · Memory Addressing**: `D(Rb,Ri,S)` built up one piece at a time, with register and memory tables.
- **Part 3 · Control Flow**: `cmp` order, the four flags one at a time with a worked "flag recipe" for every question, `set`, jumps, and a loop you can step through.
- **Part 4 · Procedures**: a push/pop stack to play with, `call` and `ret` step by step, argument registers, stack frames, and caller- vs callee-saved registers.
- **Part 5 · Arrays**: type sizes, element addresses, pointer math, the lea-vs-mov recipe, plus L05's 2D arrays, arrays of pointers, and structs.

**Memory hierarchy** (L06 parts 1–4, In-Class Practice 6–9)

- **Part 6 · Memory & DRAM**: the memory pyramid, SRAM vs DRAM, reading a DRAM supercell with RAS and CAS, memory modules, and picking the rows × columns that give the shortest address.
- **Part 7 · Buses & Disks**: SDRAM/DDR, nonvolatile memory, bus read and write transactions, disk geometry, capacity, access time, and how long a whole file takes to read, best case vs random.
- **Part 8 · I/O & SSDs**: the I/O bus, reading a disk sector with DMA and interrupts, how SSDs read, write and wear out, and how many years until they do.
- **Part 9 · Locality**: the CPU–memory gap, temporal vs spatial locality, stride-k patterns, rows vs columns, and loop order for 3D arrays.

**Caches and virtual memory** (L07 parts 1–3, L08 part 1, In-Class Practice 10–12)

- **Part 10 · Cache Memory**: blocks, hits and misses, the three kinds of miss, S, E and B, splitting an address into tag, set and offset, and looking a byte up in a 2-way cache.
- **Part 11 · Cache Misses**: the slides' direct-mapped and 2-way simulations, conflict misses and padding, write policies, miss rate and average access time.
- **Part 12 · Virtual Memory**: physical vs virtual addressing, the MMU, and counting address spaces with N = 2ⁿ and K, M, G, T, P.

**Review**: six shuffled mixes that pick new questions every replay, plus a Lab that works out any instruction, operand or flag result step by step.

Every part ends with a **Class Practice** level that works through that part's in-class worksheet, and has a one-page **cheat sheet** for exam review. Bigger problems are broken into **guided steps** that fill in as you answer, and many lessons have something to play with: a byte dial, a live stack, a DRAM chip, a rows × columns explorer, disk and file-read calculators, an SSD lifetime calculator, loop-order explorers for 2D and 3D arrays, a 4-slot cache, an address splitter, a step-by-step cache lookup, the slides' cache simulations, and an address-space counter.

The whole game is a single file, `index.html`, with no build step and no dependencies beyond Google Fonts.