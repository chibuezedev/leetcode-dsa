# Plus One

## Problem Description

You are given a **large integer** represented as an array of digits, where each `digits[i]` is the ith digit of the integer. The digits are ordered from **most significant to least significant**, left-to-right. The integer **does not contain leading zeros**.  

Increment the integer by one and return the resulting array of digits.

---

## Examples

**Example 1:**

Input: digits = [1,2,3]
Output: [1,2,4]
Explanation: 123 + 1 = 124


**Example 2:**
Input: digits = [4,3,2,1]
Output: [4,3,2,2]
Explanation: 4321 + 1 = 4322


**Example 3:**

Input: digits = [9]
Output: [1,0]
Explanation: 9 + 1 = 10


---

## Constraints

- `1 <= digits.length <= 100`  
- `0 <= digits[i] <= 9`  
- `digits` does not contain any leading zeros

---

## Approach

1. Start from the **last digit** of the array.  
2. Add **1** to the current digit.  
3. If the digit becomes **10**, set it to 0 and **carry 1** to the next digit on the left.  
4. Repeat until there is **no carry left** or all digits are processed.  
5. If there is still a carry after the first digit, **insert 1 at the front** of the array.

---

## Complexity Analysis

- **Time Complexity:** `O(n)` – each digit is processed at most once  
- **Space Complexity:** `O(1)` – modifying the array in place, except possibly adding a new first digit

---
