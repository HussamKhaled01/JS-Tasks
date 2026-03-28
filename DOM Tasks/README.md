# DOM Manipulation & Traversing Project

## 🧠 Research Summary

### 1. The DOM (Document Object Model)
The DOM is a tree-like representation of the HTML document. 
- **Node:** The base unit of the tree (Everything is a node: elements, text, comments).
- **Element Node:** Represents HTML tags (`<div>`, `<h1>`).
- **Text Node:** The actual text inside tags.
- **HTML vs DOM:** HTML is the initial text file; the DOM is the live object living in the browser memory.

### 2. Relationships
- `children` vs `childNodes`: `children` only targets elements, while `childNodes` includes text and comments.
- `parentElement` vs `parentNode`: Usually the same, but `parentElement` returns `null` if the parent is not an element (like the Document node).

### 3. Collections
- **HTMLCollection:** Live (updates automatically if the DOM changes), returned by `getElementsByClassName`.
- **NodeList:** Mostly static, returned by `querySelectorAll`.

### 4. Performance: Reflow & Repaint
- **Reflow:** When the browser recalculates positions and sizes (expensive).
- **Repaint:** When the browser redraws the element (less expensive than reflow).
- **Best Practice:** Minimize direct DOM changes. Use `documentFragment` or CSS classes instead of inline styles.

## 🚀 Practical Tasks
- **Task 1:** Analyzed tree navigation using `firstElementChild` and `nextElementSibling`.
- **Task 2:** Built a UI card purely through JS `createElement` and `append`.
- **Task 3:** Navigated a nested list without using selectors by using relationship properties.
- **Task 4:** Demonstrated dynamic element swapping using `replaceWith`.

---