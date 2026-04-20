# 📐 Number of Diagonals in a Polygon

## 🧩 Problem Statement
Given an integer `n` representing the number of sides of a polygon, find the number of diagonals that can be formed.

---

## 💡 Formula Used

\[
\text{Diagonals} = \frac{n(n - 3)}{2}
\]

---

## 🧠 Explanation
- A polygon with `n` vertices can have total line segments:
  \[
  \frac{n(n - 1)}{2}
  \]
- Out of these, `n` are sides of the polygon.
- The remaining are diagonals:
  \[
  \frac{n(n - 1)}{2} - n = \frac{n(n - 3)}{2}
  \]

---

## 🚀 Approach
1. Use the direct mathematical formula.
2. Multiply `n` with `(n - 3)` and divide by `2`.
3. Cast to `long` to avoid integer overflow.

---

## 🧾 Java Implementation

```java
class Solution {
    public long diagonals(int n) {
        return (long) n * (n - 3) / 2;
    }
}
📊 Examples
Input (n)	Output
3	0
4	2
5	5
6	9
⚠️ Edge Cases
n < 3 → Not a valid polygon (no diagonals)
Large n → Use long to prevent overflow
🏷️ Tags

Math Geometry Formula-Based Easy

👨‍💻 Author

Sanjeev Sharma
