# 🔍 Number Search Game in a Sorted Matrix

This is a C++ interactive game based on the algorithm for searching a number in a **sorted 2D matrix**, where each row and column is sorted in ascending order. The game challenges the player to find a hidden number with as few moves as possible!

---

## 🎮 Game Overview

The game starts with a welcome screen and offers three difficulty levels:

- 🟢 Easy: 5x5 matrix  
- 🟡 Medium: 10x10 matrix  
- 🔴 Hard: 15x15 matrix

Each matrix is randomly generated and sorted row-wise and column-wise. You can either:
- Let the system pick a random number to search for, or
- Choose your own number to find.

---

## 🧠 How to Play

- The system gives you **hints** based on the comparison between your target number and the number at the current position.
- Move **left** if the current number is greater.
- Move **down** if the current number is smaller.
- Try to find the number in **less than 20 moves**!

---

## 💡 Algorithm Logic

This project implements the **"Search in a Row-wise and Column-wise Sorted Matrix"** algorithm using the following pseudocode:

```text
Start from top-right corner (0, n-1)
While within bounds and turns < 2n-1:
    - If current == target → return FOUND
    - If target < current → move left
    - If target > current → move down

