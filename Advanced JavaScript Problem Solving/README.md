# 🚀 Algorithm Practice Tasks

## 📌 Rules (Strict)

* ❌ No built-in functions
  (`map`, `filter`, `reduce`, `sort`, `includes`, etc.)
* ❌ No shortcuts or helpers
* ✅ Use only:

  * loops
  * conditions
  * variables
* ✅ Always consider time complexity (`O(n)`, `O(n²)`, ...)

---

## 🧩 Problems

---

### 1️⃣ Log Compression System

**Problem:**
You are given a list of event logs. Compress consecutive identical events by counting occurrences.

**Input:**

```js
[
  { event: "click", time: 1 },
  { event: "click", time: 2 },
  { event: "scroll", time: 3 },
  { event: "scroll", time: 4 },
  { event: "click", time: 5 }
]
```

**Output:**

```js
[
  { event: "click", count: 2 },
  { event: "scroll", count: 2 },
  { event: "click", count: 1 }
]
```

**Concept:**
Track current event and count consecutive repetitions.

**Time Complexity Target:** `O(n)`

---

### 2️⃣ Subarray with Given Sum

**Problem:**
Find a continuous subarray whose sum equals a target value.

**Input:**

```js
arr = [1,4,20,3,10,5]
target = 33
```

**Output:**

```js
start = 2
end = 4
```

**Concept:**
Try each starting index and accumulate sum forward.

**Time Complexity Target:** `O(n²)` → (can be optimized to `O(n)`)

---

### 3️⃣ Maximum Profit

**Problem:**
Find the maximum profit from buying and selling a stock once.

**Input:**

```js
[7,1,5,3,6,4]
```

**Output:**

```js
5
```

**Concept:**
Track minimum price so far and compute profit at each step.

**Time Complexity Target:** `O(n)`

---

### 4️⃣ Trap Rain Water 💀

**Problem:**
Calculate how much water is trapped between bars.

**Input:**

```js
[0,1,0,2,1,0,1,3,2,1,2,1]
```

**Output:**

```js
6
```

**Concept:**
Water at index = `min(maxLeft, maxRight) - height[i]`

**Time Complexity Target:** `O(n²)` → (optimal `O(n)`)

---

### 5️⃣ Longest Unique Subarray

**Problem:**
Find the longest subarray with no repeated elements.

**Input:**

```js
[1,2,3,1,2,3,4,5]
```

**Output:**

```js
[1,2,3,4,5]
```

**Concept:**
Expand until duplicate appears, then restart.

**Time Complexity Target:** `O(n²)` → (optimal `O(n)`)

---

### 6️⃣ Product of Array Except Self

**Problem:**
Return an array where each element is the product of all other elements.

**Input:**

```js
[1,2,3,4]
```

**Output:**

```js
[24,12,8,6]
```

**Concept:**
Use left and right product accumulation.

**Time Complexity Target:** `O(n)`

---

### 7️⃣ Spiral Matrix Traversal

**Problem:**
Traverse a matrix in spiral order.

**Input:**

```js
[
  [1,2,3],
  [4,5,6],
  [7,8,9]
]
```

**Output:**

```js
[1,2,3,6,9,8,7,4,5]
```

**Concept:**
Control boundaries: top, bottom, left, right.

**Time Complexity Target:** `O(n × m)`

---

### 8️⃣ Minimum Window Subarray

**Problem:**
Find the smallest subarray containing all target elements.

**Input:**

```js
arr = [1,2,2,3,1,2,3]
target = [1,2,3]
```

**Output:**

```js
[2,3,1]
```

**Concept:**
Check all subarrays and track the smallest valid one.

**Time Complexity Target:** `O(n²)`

---

### 9️⃣ Detect Cycle in Array 💀

**Problem:**
Determine if movement through the array forms a cycle.

**Input:**

```js
[2,-1,1,2,2]
```

**Output:**

```js
true
```

**Concept:**
Use values as jumps; detect revisiting indices.

**Time Complexity Target:** `O(n)`

---

### 🔟 Reconstruct Queue 💀💀

**Problem:**
Reconstruct queue based on height and number of taller people in front.

**Input:**

```js
[
  { height:7, inFront:0 },
  { height:4, inFront:4 },
  { height:7, inFront:1 },
  { height:5, inFront:0 },
  { height:6, inFront:1 },
  { height:5, inFront:2 }
]
```

**Output (One valid solution):**

```js
[
  { height:5, inFront:0 },
  { height:7, inFront:0 },
  { height:5, inFront:2 },
  { height:6, inFront:1 },
  { height:4, inFront:4 },
  { height:7, inFront:1 }
]
```

**Concept:**
Place taller people first, then insert others based on `inFront`.

**Time Complexity Target:** `O(n²)`

---

## 📊 Summary

| Task                | Difficulty | Optimal Complexity |
| ------------------- | ---------- | ------------------ |
| Log Compression     | Easy       | O(n)               |
| Subarray Sum        | Medium     | O(n)               |
| Max Profit          | Easy       | O(n)               |
| Trap Water          | Hard       | O(n)               |
| Longest Unique      | Medium     | O(n)               |
| Product Except Self | Medium     | O(n)               |
| Spiral Matrix       | Medium     | O(n×m)             |
| Min Window          | Hard       | O(n)               |
| Detect Cycle        | Hard       | O(n)               |
| Reconstruct Queue   | Hard       | O(n²)              |

