# Experiment Review

## Scope

All five experiments were reviewed for data-structure behavior, boundary checks,
input handling, ownership, and exit cleanup.

## Findings and Resolutions

| Experiment | Review result |
|-----------|---------------|
| 1.A Array List ADT | Position checks protect insertion and deletion bounds; checked input prevents invalid sizes and values from being used. |
| 1.B Singly Linked List | Beginning/end insertion and position deletion preserve links; allocated nodes are released on exit. |
| 2 Circular Linked List | Empty, single-node, head, and missing-value deletion paths preserve circularity; the list is released on exit. |
| 3.A Array Stack | Empty and full states are guarded; push, pop, peek, and display preserve LIFO order. |
| 3.B Array Queue | The count-based circular queue reuses released slots and guards empty/full states. |
| 4.A Linked Stack | Push and pop update the top pointer correctly; remaining nodes are released on exit. |
| 4.B Linked Queue | Front and rear pointers remain consistent through empty, single-node, and multi-node transitions. |
| 5 Binary Search Tree | Insertion skips duplicates, traversals preserve their ordering rules, repeated creation replaces the old tree, and exit cleanup frees every node. |

## Input Contract

Every experiment checks integer input before using it. Invalid input is reported
and the current program exits safely; no failed read is used as an uninitialized
or stale integer.

## Verification

- VS Code diagnostics reported no errors for all eight C source files and README.md.
- A GCC build was attempted for every C file, but GCC is not installed on the
  current Windows environment. Run the documented warning-enabled builds after
  installing a C toolchain.
- Interactive boundary scenarios should be exercised after compilation: empty
  operations, full array structures, invalid positions, duplicate BST values,
  negative BST counts, repeated BST creation, and exit with allocated nodes.
