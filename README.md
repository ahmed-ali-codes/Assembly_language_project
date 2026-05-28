# 🖥️ Assembly Language Projects

A collection of x86 Assembly Language programs written during university coursework and self-study. Each project directly interacts with system hardware through CPU registers, memory addressing, and DOS/BIOS interrupts — demonstrating low-level control that higher-level languages abstract away.

---

## About Assembly Language

Assembly is a low-level programming language with a near 1-to-1 correspondence between its instructions and the CPU's machine code. Writing in Assembly teaches you how programs actually execute: how registers hold values, how the stack manages function calls, how memory is laid out, and how the operating system is invoked through interrupts. It is foundational knowledge for computer architecture, embedded systems, OS development, and reverse engineering.

---

## Projects

| # | Project | Description | Concepts |
|---|---|---|---|
| 1 | [Clock](./Clock/) | A 12-hour countdown clock with user-set start time | Interrupts, carry logic, loops, ASCII conversion |

> More projects coming soon — see the [Roadmap](#roadmap) below.

---

## Tools & Environment

All programs are written for the **x86 (8086/80286) architecture** and use **MASM/TASM** directives with **DOS INT 21h** system calls.

Recommended environments:

- **[emu8086](https://emu8086-microprocessor-emulator.en.softonic.com/)** — beginner-friendly emulator with a built-in editor and debugger
- **[DOSBox](https://www.dosbox.com/)** + MASM or TASM — for a closer-to-real DOS experience
- **NASM** on Linux — for projects targeting flat binary or ELF output

---

## Getting Started

### Clone the repository

```bash
git clone https://github.com/ahmed-ali-codes/Assembly_language_project.git
cd Assembly_language_project
```

### Run any project

Navigate into a project folder and follow its own `README.md` for assembler-specific build steps. For example:

```
cd Clock
```

Then follow the instructions in [Clock/README.md](./Clock/README.md).

---

## Repository Structure

```
Assembly_language_project/
│
├── Clock/
│   ├── clock.asm         ← Source code
│   └── README.md         ← Project-specific instructions
│
└── README.md             ← This file
```

Each project folder contains:
- The `.asm` source file(s), fully commented
- A `README.md` explaining what the program does, how to build it, and sample output

---

## Concepts Covered Across Projects

- CPU registers (`AX`, `BX`, `CX`, `DX`, `SI`, `DI`, `SP`, `BP`)
- Memory segmentation (`.CODE`, `.DATA`, `.STACK`)
- DOS interrupts (`INT 21h`) for I/O, string display, and program termination
- BIOS interrupts for hardware-level operations
- Stack operations (`PUSH`, `POP`, `CALL`, `RET`)
- Conditional and unconditional jumps (`JMP`, `JE`, `JNE`, `JG`, etc.)
- Loops (`LOOP`, `CX`-based counting)
- ASCII ↔ integer conversion
- Carry propagation and BCD-style digit arithmetic

---

## Roadmap

Planned projects to be added:

- [ ] **Simple Calculator** — addition, subtraction, multiplication, division via keyboard input
- [ ] **String Reversal** — reverse a user-entered string using stack push/pop
- [ ] **Number to ASCII Converter** — convert a binary number to its ASCII decimal representation
- [ ] **Even/Odd Checker** — use bitwise AND to determine parity
- [ ] **Interrupt-driven I/O** — custom interrupt handlers using INT vectors
- [ ] **Bubble Sort** — sort an array of integers in memory
- [ ] **Fibonacci Sequence** — recursive or iterative generation using registers

---

## Author

**Ahmed Ali** — Computer Science student exploring low-level systems programming.

Feel free to open an issue or pull request if you spot a bug or want to contribute a project!

---

## License

This repository is open-source under the [MIT License](./LICENSE).
