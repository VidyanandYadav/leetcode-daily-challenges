# 🔄 Rotate String

## 🧩 Problem Statement

Given two strings `s` and `goal`, return `true` if and only if `s` can become `goal` after some number of shifts.

A shift operation moves the **leftmost character** of the string to the **rightmost position**.

### ✨ Example

```
Input: s = "abcde", goal = "cdeab"
Output: true
```

```
Input: s = "abcde", goal = "abced"
Output: false
```

---

## 💡 Approach

Instead of simulating all rotations, we use an optimized trick:

* If `goal` is a rotation of `s`, then it must be a **substring of `s + s`**
* Example:

  ```
  s = "abcde"
  s + s = "abcdeabcde"
  ```

  All possible rotations of `s` are present inside `s + s`

---

## 🚀 Algorithm

1. Check if lengths of `s` and `goal` are equal
2. Concatenate string `s` with itself → `s + s`
3. Check if `goal` is a substring of `s + s`



## ⏱️ Complexity Analysis

* **Time Complexity:** O(n)
* **Space Complexity:** O(n)

---

## 🧠 Key Insight

All rotations of a string are contained within its double concatenation (`s + s`).
This allows us to solve the problem efficiently without explicitly generating rotations.

---

## 📌 Tags

`String` `Rotation` `Easy` `Interview-Prep`

---

## 🙌 Acknowledgment

Problem inspired by common coding interview questions.
