# Data Structures Laboratory in C

A professional collection of **Data Structures Laboratory programs** implemented in **C**, covering the core Abstract Data Types (ADTs) and linear data structures required for undergraduate Computer Science and Engineering laboratories.

The repository focuses on **correctness, clean code, efficiency, and readability**, making it suitable for academic submissions, practical examinations, and GitHub portfolios.

---

## Repository Overview

This project contains menu-driven implementations of fundamental data structures using both **arrays** and **linked lists**. Every program is written in standard **C11**, follows modular programming practices, and includes proper input validation and memory management.

### Features

- Clean and well-documented C programs
- Modular function-based implementation
- Menu-driven user interface
- Optimized time complexity where applicable
- Safe memory management using `malloc()` and `free()`
- GCC compatible (`C11`)
- Suitable for DS laboratory practicals and viva preparation

---

## Experiments Included

| Experiment | Title | Data Structure |
|-----------|-------|----------------|
| **Ex 1.A** | Array Implementation of List ADT | Array |
| **Ex 1.B** | Implementation of Singly Linked List | Linked List |
| **Ex 2** | Implementation of Circular Linked List | Circular Linked List |
| **Ex 3.A** | Array Implementation of Stack | Stack |
| **Ex 3.B** | Array Implementation of Queue | Queue (Circular Array) |
| **Ex 4.A** | Linked List Implementation of Stack | Stack |
| **Ex 4.B** | Linked List Implementation of Queue | Queue |
| **Ex 5** | Binary Search Tree | Binary Search Tree |

---

## Repository Structure

```text
DS_Lab/
│
├── README.md
│
├── Ex_1A_Array_Implementation_of_List_ADT.c
├── Ex_1B_Implementation_of_Singly_Linked_List.c
├── Ex_2_Implementation_of_Circular_Linked_List.c
├── Ex_3A_Array_Implementation_of_Stack.c
├── Ex_3B_Array_Implementation_of_Queue.c
├── Ex_4A_Linked_List_Implementation_of_Stack.c
├── Ex_4B_Linked_List_Implementation_of_Queue.c
└── Ex_5_Binary_Search_Tree.c
```

---

## Data Structures Covered

### List ADT

- Create List
- Insert Element
- Delete Element
- Search Element
- Display List

### Singly Linked List

- Insert at Beginning
- Insert at End
- Delete by Position
- Search Element
- Traverse List

### Circular Linked List

- Insert at end
- Delete the first matching value
- Search for a value
- Traverse from the head until the head is reached again

### Stack

Array Implementation

- Push
- Pop
- Peek
- Display

Linked List Implementation

- Dynamic Push
- Dynamic Pop
- Peek
- Traverse Stack

### Queue

Array Implementation (Circular Queue)

- Enqueue
- Dequeue
- Peek
- Display

Linked List Implementation

- Enqueue
- Dequeue
- Peek
- Display

### Binary Search Tree

- Create a fresh BST from a batch of values
- Ignore duplicate values
- Display preorder, inorder, and postorder traversals
- Search for a value
- Release all allocated nodes before exit

---

## Time Complexity Analysis

| Operation | Array | Linked List |
|-----------|------:|-----------:|
| Insert | O(n) | O(1) / O(n) |
| Delete | O(n) | O(n) |
| Search | O(n) | O(n) |
| Push | O(1) | O(1) |
| Pop | O(1) | O(1) |
| Enqueue | O(1)* | O(1) |
| Dequeue | O(1)* | O(1) |

> *Array queue uses a **Circular Queue**, providing constant-time enqueue and dequeue.

### Binary Search Tree Complexity

For a tree with height $h$:

| Operation | Average Case | Worst Case |
|-----------|-------------:|-----------:|
| Insert | O(log n) | O(n) |
| Search | O(log n) | O(n) |
| Traversal | O(n) | O(n) |
| Space | O(n) | O(n) |

The worst case occurs when inserted values produce a completely skewed tree.

---

## Algorithms Implemented

- Array-based List ADT
- Dynamic Singly Linked List
- Circular Linked List
- Stack using Array
- Stack using Linked List
- Queue using Circular Array
- Queue using Linked List
- Binary Search Tree with recursive traversals

---

## Compilation and Execution

Install GCC through MinGW-w64, MSYS2, or a similar toolchain, then compile one
source file at a time with warnings enabled:

```powershell
gcc -std=c11 -Wall -Wextra -Wpedantic -O2 `
	Ex_5_Binary_Search_Tree.c -o Ex_5_Binary_Search_Tree.exe
.\Ex_5_Binary_Search_Tree.exe
```

In PowerShell, use `.\program.exe` to run an executable in the current
directory. In a Unix-like shell, use `./program`. Replace the source and output
names with the experiment you want to run. Each program is interactive and
expects integer input at its menu prompts.

Example for Experiment 3.A:

```powershell
gcc -std=c11 -Wall -Wextra -Wpedantic -O2 `
	Ex_3A_Array_Implementation_of_Stack.c -o Ex_3A_Array_Implementation_of_Stack.exe
.\Ex_3A_Array_Implementation_of_Stack.exe
```

---

## Learning Outcomes

After completing these programs, students will understand:

- Abstract Data Types (ADT)
- Dynamic memory allocation
- Pointer manipulation
- Linear data structures
- Circular linked structures
- Stack and Queue operations
- Binary Search Tree insertion, search, and traversal
- Algorithmic time complexity
- Modular programming in C

---

## Technologies Used

- **Language:** C (C11)
- **Compiler:** GCC
- **Paradigm:** Procedural Programming
- **Platform:** Linux / Windows / macOS

---

## Quality Improvements

Compared to conventional laboratory implementations, these programs include:

- Proper boundary validation
- Overflow and underflow handling
- Memory leak prevention
- Consistent coding style
- Readable function decomposition
- Professional documentation and comments

---

## Academic Use

This repository is intended for:

- Data Structures Laboratory
- Practical Examination Preparation
- University Assignments
- GitHub Academic Portfolio
- C Programming Revision

---

## Author

**Thamizh Selvan**

Computer Science & Engineering

---

## License

This repository is created for **educational and academic purposes**. Feel free to use it for learning and laboratory practice.
