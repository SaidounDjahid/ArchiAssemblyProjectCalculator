# ⚙️ Low-Level Numeric Processing System (x86 Assembly)

A low-level system developed in x86 Assembly (MASM) to process numeric input, perform arithmetic operations, and visualize processor behavior through register flags.

This project was developed as part of the Computer Architecture module at USTHB.

---

## 🚀 Features

- Keyboard input handling (decimal numbers)
- Input validation (digits only, error handling)
- ASCII to binary conversion
- Array initialization and memory manipulation
- Element-wise addition of numeric arrays
- Display of numbers in decimal format
- Binary visualization of processor flags (PSW)
- Optional hexadecimal display of results

---

## 🧠 Concepts Covered

- CPU registers manipulation (AX, BX, CX, DX)
- Stack operations (PUSH / POP)
- Interrupt handling (INT 21H, INT 10H)
- Memory segmentation (DATA, STACK, CODE)
- Arithmetic operations at low level
- Processor flags (Zero, Carry, Overflow, etc.)
- Number conversion (ASCII ↔ Binary ↔ Decimal)

---

## 🏗️ Program Overview

The program provides a menu-driven interface allowing the user to:

1. Input decimal numbers (with validation)
2. Convert and store values in arrays
3. Initialize two arrays of numbers
4. Perform element-wise addition between arrays
5. Display results in decimal format
6. Display processor flags (PSW) after each operation

Example execution:


NB1 + NB2 = RESULT
[FLAGS DISPLAYED IN BINARY]


---

## ⚙️ Technologies

- x86 Assembly (MASM / TASM compatible)
- DOS Interrupts (INT 21H, INT 10H)
- Low-level memory and register manipulation

---

## ▶️ How to Run

### 1. Assemble the program
```bash
masm projet.asm
link projet.obj
2. Run the program (DOS environment / DOSBox recommended)
projet.exe
📌 Key Procedures
LIRE_NOMBRE_DECIMAL → Reads and validates user input
AFFICHE_NOMBRE_DECIMAL → Displays numbers in decimal
INIT_TAB → Initializes arrays with user input
SOMMENB1NB2 → Performs element-wise addition
AFFICHAGE_FLAGS → Displays processor flags (PSW)
AX2BIN → Converts register values to binary
AFFICHE_NOMBRE_HEXA → Displays hexadecimal values
📁 Project Structure
DATA segment → variables, arrays, messages
STACK segment → program stack
CODE segment → logic and procedures
🎓 Academic Context

Developed at USTHB (University of Science and Technology Houari Boumediene)
Module: Computer Architecture (ARCHI 02)

⚠️ Notes
The feature related to transforming the result array into a LIFO queue was not implemented
Designed for educational purposes to demonstrate low-level programming concepts
👨‍💻 Author

Djahid Saidoun
