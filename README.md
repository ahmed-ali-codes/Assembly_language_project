# Assembly Language Projects Collection

This repository showcases a collection of projects written in **Assembly Language**, developed during university courses and personal learning. These low-level programs directly interact with the system hardware and are designed to demonstrate fine control over memory and CPU instructions.

### 💡 About Assembly Language
Assembly is a low-level programming language that is closely tied to a computer's architecture. It allows precise control of hardware resources and is commonly used in embedded systems, performance-critical tasks, and learning how computers execute instructions at the machine level.

### 📁 Project Structure

Each folder contains an individual assembly project with:
- `.asm` source file(s)
- A short `README.md` file explaining the code
- Test outputs or screenshots (optional)
- Instructions for assembling and running the program

### 🛠 Sample Projects
- Simple Calculator in Assembly
- String Reversal Program
- Number to ASCII Converter
- Even/Odd Checker
- Interrupt-driven Input/Output

### ⚙️ How to Assemble & Run (NASM Example)
```bash
nasm -f elf32 filename.asm
ld -m elf_i386 -s -o output_name filename.o
./output_name
```

> 📌 *Note:* Make sure you're running on a system that supports 32-bit execution, or use emulators like DOSBox for 16-bit programs.

---

### 📌 Note:
These projects are intended to illustrate the understanding of registers, memory addressing, stack operations, loops, conditionals, and system calls at the assembly level. They reflect foundational knowledge in computer architecture and low-level programming.

```

---
