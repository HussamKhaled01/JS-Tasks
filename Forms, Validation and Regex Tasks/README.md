# JavaScript Form Validation: Mastery Series

This project consists of four progressive tasks designed to master form handling, DOM manipulation, and complex validation using Regular Expressions (Regex).

---

## 🟢 Task 1 — Basic Form Handling
### 🎯 Objective
Practice capturing user data and preventing default browser behaviors.

### 💻 Requirements
* **Fields:** First Name, Last Name, Email.
* **Functionality:**
    * Prevent page reload on submit using `event.preventDefault()`.
    * Get all input values using JavaScript.
    * Display the entered data dynamically inside the page.

---

## 🟡 Task 2 — Basic Validation
### 🎯 Objective
Apply fundamental validation rules to ensure data integrity.

### 💻 Requirements
* **Validation Rules:**
    * All fields are **required**.
    * **First & Last Name:** Must contain only letters.
    * **Email:** Must not be empty.
* **Functionality:**
    * Show error messages in **red** directly under each input.
    * Prevent form submission if any field is invalid.

---

## 🟠 Task 3 — Regex Validation
### 🎯 Objective
Use Regular Expressions (Regex) for precise pattern matching.

### 💻 Requirements
* **New Field:** Mobile Number.
* **Validation Rules:**
    * **Email:** Must follow a valid format using Regex (e.g., `name@domain.com`).
    * **Mobile Number:** Must be exactly **10 digits** and contain **numbers only**.
* **Functionality:**
    * Show appropriate error messages for format errors.
    * Prevent submission if Regex patterns are not met.

---

## 🔵 Task 4 — Advanced Form Validation
### 🎯 Objective
Build a robust registration form with multiple complex dependencies.

### 💻 Requirements
* **Fields:** First Name, Last Name, Birth Date, Email, Confirm Email, Password, Confirm Password.
* **Validation Rules:**
    * **Names:** Letters only.
    * **Birth Date:** Must be a valid date and not empty.
    * **Email:** Valid Regex; Email and Confirm Email **must match**.
    * **Password Criteria:**
        * Must start with a **Capital Letter**.
        * Must contain at least **2 numbers**.
        * Must contain at least **1 special character**.
        * Length: **8 to 32 characters**.
        * Password and Confirm Password **must match**.

---

## 🛠️ Implementation Guide
1. **DOM Selection:** Use `document.getElementById()` or `document.querySelector()`.
2. **Event Listening:** Use `element.addEventListener('submit', ...)` to handle the logic.
3. **Regex Patterns:**
    * Email: `/^[^\s@]+@[^\s@]+\.[^\s@]+$/`
    * Password Capital Start: `/^[A-Z]/`
    * Password Special Char: `/[!@#$%^&*(),.?":{}|<>]/`

    ---