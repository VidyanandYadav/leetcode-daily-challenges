# Day 1 - Rotated Digits (LeetCode 788)

## 🧩 Problem
An integer is called a "good number" if after rotating each digit by 180 degrees, we get a valid number that is different from the original.

Valid rotations:
- 0 → 0
- 1 → 1
- 8 → 8
- 2 ↔ 5
- 6 ↔ 9

Invalid digits:
- 3, 4, 7

Return the count of good numbers in range [1, n].

---

## 💡 Approach
We iterate from 1 to n and check each number:

1. Convert number to string
2. Check each digit:
   - If digit is invalid → skip number
   - If digit changes after rotation → mark as "different"
3. Count only numbers that:
   - are valid
   - and change after rotation

---

## ⏱ Complexity
- Time: O(n * d)   (d = number of digits)
- Space: O(1)

---

## 🏷 Tags
`#math #bruteforce #simulation`
