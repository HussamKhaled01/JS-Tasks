# 🚀 JavaScript Practice — Functions & Arrays (30 Tasks)

## 📌 Rules

* ✅ Every solution must be written as a **function**
* ❌ Do **NOT use `map()`**
* ✅ Combine:

  * Array methods (`slice`, `splice`, `concat`, `filter`, `sort`, etc.)
  * Loops when needed
* ❌ Do not rely on loops alone
* ✅ Prefer array methods whenever possible
* ✅ Test each function with multiple inputs

---

## 🟢 Level 1 — Array Manipulation

---

### 1️⃣ `firstAndLast(arr)`

Return an array containing the **first and last elements**.

```js
// [1,2,3,4,5] → [1,5]
```

---

### 2️⃣ `removeMiddle(arr)`

Remove the **middle element**.

```js
// [1,2,3,4,5] → [1,2,4,5]
```

---

### 3️⃣ `swapFirstLast(arr)`

Swap the **first and last elements**.

```js
// [1,2,3,4,5] → [5,2,3,4,1]
```

---

### 4️⃣ `insertAtMiddle(arr, value)`

Insert a value **in the middle**.

```js
// [1,2,3,4], 10 → [1,2,10,3,4]
```

---

### 5️⃣ `duplicateArray(arr)`

Duplicate the array content.

```js
// [1,2,3] → [1,2,3,1,2,3]
```

---

## 🟡 Level 2 — Filtering & Searching

---

### 6️⃣ `removeDuplicates(arr)`

Remove duplicate values.

```js
// [1,2,2,3,4,4,5] → [1,2,3,4,5]
```

---

### 7️⃣ `findSecondLargest(arr)`

Return the **second largest number**.

```js
// [4,9,2,10,6] → 9
```

---

### 8️⃣ `findSecondSmallest(arr)`

Return the **second smallest number**.

---

### 9️⃣ `removeGreaterThan(arr, value)`

Remove values **greater than a given number**.

```js
// [10,5,20,3,8], 10 → [5,3,8]
```

---

### 🔟 `removeLessThan(arr, value)`

Return values **greater than or equal to a given number**.

---

## 🔵 Level 3 — Advanced Array Logic

---

### 1️⃣1️⃣ `countOccurrences(arr, value)`

Count how many times a value appears.

```js
// [1,2,3,2,4,2], 2 → 3
```

---

### 1️⃣2️⃣ `arrayIntersection(arr1, arr2)`

Return elements present in **both arrays**.

```js
// [1,2,3,4] & [3,4,5] → [3,4]
```

---

### 1️⃣3️⃣ `arrayDifference(arr1, arr2)`

Return elements in `arr1` **not in `arr2`**.

```js
// [1,2,3,4] & [3,4] → [1,2]
```

---

### 1️⃣4️⃣ `uniqueMerge(arr1, arr2)`

Merge arrays and remove duplicates.

```js
// [1,2,3] + [3,4,5] → [1,2,3,4,5]
```

---

### 1️⃣5️⃣ `removeNegativeNumbers(arr)`

Remove all negative numbers.

```js
// [5,-2,10,-3,7] → [5,10,7]
```

---

## 🔴 Level 4 — String & Array Combined

---

### 1️⃣6️⃣ `wordsLongerThan(arr, length)`

Return words longer than a given length.

```js
// ["alex","mohammad","ali"], 4 → ["mohammad"]
```

---

### 1️⃣7️⃣ `countLetterInWords(arr, letter)`

Count words that contain a specific letter.

```js
// ["apple","banana","car"], "a" → 3
```

---

### 1️⃣8️⃣ `removeShortWords(arr, length)`

Remove words shorter than a given length.

---

### 1️⃣9️⃣ `findLongestWord(arr)`

Return the longest word.

---

### 2️⃣0️⃣ `findShortestWord(arr)`

Return the shortest word.

---

## 🟣 Level 5 — Complex Challenges

---

### 2️⃣1️⃣ `sortByLength(arr)`

Sort words by length.

```js
// ["apple","hi","banana"] → ["hi","apple","banana"]
```

---

### 2️⃣2️⃣ `removeEverySecond(arr)`

Remove every second element.

```js
// [1,2,3,4,5,6] → [1,3,5]
```

---

### 2️⃣3️⃣ `sumEvenNumbers(arr)`

Return the sum of even numbers.

```js
// [1,2,3,4,5,6] → 12
```

---

### 2️⃣4️⃣ `sumOddIndex(arr)`

Sum values at odd indexes.

---

### 2️⃣5️⃣ `reverseWithoutReverse(arr)`

Reverse array without using `reverse()`.

---

## ⚡ Level 6 — Hard Challenges

---

### 2️⃣6️⃣ `findMissingNumber(arr)`

Find the missing number from `1 → N`.

```js
// [1,2,3,5,6] → 4
```

---

### 2️⃣7️⃣ `pairSum(arr, target)`

Return two numbers that sum to target.

```js
// [2,7,11,15], 9 → [2,7]
```

---

### 2️⃣8️⃣ `rotateArray(arr, steps)`

Rotate array to the right.

```js
// [1,2,3,4,5], 2 → [4,5,1,2,3]
```

---

### 2️⃣9️⃣ `chunkArray(arr, size)`

Split array into chunks.

```js
// [1,2,3,4,5,6], 2 → [[1,2],[3,4],[5,6]]
```

---

### 3️⃣0️⃣ `groupByLength(arr)`

Group words by length.

```js
// ["hi","cat","dog","apple"]
// → {2:["hi"], 3:["cat","dog"], 5:["apple"]}
```

---

## 📊 Difficulty Overview

| Level | Focus                  |
| ----- | ---------------------- |
| 🟢 1  | Basic array operations |
| 🟡 2  | Filtering & searching  |
| 🔵 3  | Set-like operations    |
| 🔴 4  | Strings + arrays       |
| 🟣 5  | Logic building         |
| ⚡ 6   | Problem solving        |
