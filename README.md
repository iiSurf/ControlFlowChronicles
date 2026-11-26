# Will It Assemble?

Check out [ControlFlowChronicles](https://iisurf.github.io/ControlFlowChronicles/) to play the game and learn at the same time.

A learning game for a computer systems class: x86 assembly (AT&T syntax), the memory hierarchy, caches, virtual memory and the Y86-64 processor, in nineteen parts.

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

**Caches and virtual memory** (L07 parts 1–3, L08 parts 1–4, In-Class Practice 10–15)

- **Part 10 · Cache Memory**: blocks, hits and misses, the three kinds of miss, S, E and B, splitting an address into tag, set and offset, and looking a byte up in a 2-way cache.
- **Part 11 · Cache Misses**: run the slides' caches from empty (you call each hit or miss), 2-way sets and LRU, colliding arrays and padding, write policies, and how fast a cache is.
- **Part 12 · Virtual Memory**: physical vs virtual addressing, the MMU, and counting address spaces with N = 2ⁿ and K, M, G, T, P.
- **Part 13 · Page Tables**: the three jobs of virtual memory, permission bits, pages and the DRAM cache, reading a page table, counting PTEs, and why page tables have levels.
- **Part 14 · Address Translation**: VPN and VPO, translating an address with a page table, page hits and page faults, working sets and thrashing.
- **Part 15 · The TLB**: what the TLB is for, TLBI and TLBT, and following one address all the way through the TLB, the page table and the cache.
- **Part 16 · Y86-64 ISA** (L09 part 1, In-Class Practice 16): CISC vs RISC, the Y86-64 registers and flags, encoding instructions as bytes (first the two opcode and register bytes, then little-endian constants), laying out a program with .pos and labels, decoding, and tracing a loop. Every encoding question shows the encoding table, function codes and register numbers beside it. Practice 16's Q2 and Q3 trace sum() one pass at a time, with each line's meaning, the registers, the array in memory and a pass-by-pass table that fills in as you answer.
- **Part 17 · SEQ Processor** (L09 part 2, In-Class Practice 17): built up one step at a time. First the six stages in plain words (read the instruction, read registers, do the math, use memory, save to registers, go to the next one), one small question per stage. Then the same instruction with the book's names (valA, valE, R[rA]…), which turn out to be the rows of the stage table. Then the stack, the pushq %rsp and popq %rsp puzzles, and jumps, call and ret. Class Practice 17 shows what the class page shows: the object code with line numbers and bytes, the register numbers, function codes and encoding table, the Stage | Generic | Specific table, and the pushq/popq figure.
- **Part 18 · Pipelining** (L09 part 3, In-Class Practice 18): a car wash first (throughput and latency), then real pipelines: clock cycle (slowest stage + register), GIPS (1000 ÷ cycle), latency (stages × cycle). A place-the-registers game for uneven stages, and a how-many-nops game for data hazards. Practice 18 shows each question's figure.
- **Part 19 · Pipeline Performance** (L09 part 4, In-Class Practice 19): CPI from bubbles, the three penalties (lp, mp, rp) with the lecture's typical values, a what-if CPI game, branch prediction (always taken, never taken, BTFNT, and the Yes!/No! predictor), exceptions and modern processors. Practice 19 shows the typical values it builds on.

**Review**: eight shuffled mixes (including a Parts 16–19 processor mix) that pick new questions every replay, plus a Lab that works out any instruction, operand or flag result step by step.

Every part ends with a **Class Practice** level that works through that part's in-class worksheet, and has a one-page **cheat sheet** for exam review. Bigger problems are broken into **guided steps** that fill in as you answer, and every level ends with a one-line **Remember** card.

Most lessons are things to do rather than read. Many are short step-by-step walkthroughs where each step asks you to tap or predict something: the best DRAM shape, disk capacity, disk access time, whole-file reads and SSD lifetime (each with a calculator for your own numbers), a 4-slot cache you fill block by block, a build-a-cache walkthrough for S, E and B, the memory map for tag, set and offset, colliding arrays, write policies, counting 100 reads, and counting address bits. Others are small games and toys: sort-the-facts games that build each comparison table one tap at a time (operand kinds, real or fake registers, caller- vs callee-save, SRAM vs DRAM, volatile or not, SSD vs disk, temporal vs spatial), a byte dial, a live stack, a DRAM chip, loop-order explorers for 2D and 3D arrays, two be-the-cache games (a tiny cache, then Practice 11's), a hands-on run of the slides' caches, a be-the-MMU game, and four tap-through games for virtual memory: find a page in the page table, translate an address, look up the TLB, and take a physical address to the cache. Part 16 adds a be-the-assembler bench (tap the table row, the function code and the registers, then place the constant's bytes), a byte ruler for laying out programs, a byte cutter for decoding, and a step-through run of sum(). Part 17 adds six-stage cards: one stage open at a time, with a small box showing only the registers and memory the instruction touches.html`, with no build step and no dependencies beyond Google Fonts.

## Run it locally

Open `index.html` in a browser. That's it.