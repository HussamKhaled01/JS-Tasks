# Smart User Directory — README

## 📌 Project Overview
The **Smart User Directory** is a dynamic web application that fetches user data from an external API, caches it locally for performance, and provides an interactive interface to search and view user details. This project demonstrates proficiency in **Asynchronous JavaScript**, **Storage APIs (Local & Session)**, and **DOM Manipulation**.

---

## 🎯 Key Features

* **Smart Data Fetching:** Fetches data from the [JSONPlaceholder API](https://jsonplaceholder.typicode.com/users) only once. Subsequent visits load data directly from `localStorage`.
* **Session Management:** Uses `sessionStorage` to track active sessions and greet the user with a "Session started" notification via a Bootstrap Toast.
* **Featured Users Slider:** A curated "Featured" section displaying the first three users in a modern, visually appealing slider.
* **Dynamic Search System:** A real-time search bar that filters users by **Name** or **Username**. The search state is persisted in `localStorage`, so your results remain even after a page refresh.
* **Detailed User Profiles:** A "View Details" feature that triggers a Bootstrap Modal to show comprehensive information, including address, phone, and company catchphrase.
* **Responsive UI:** Built with **Bootstrap 5** and custom CSS to ensure a seamless experience across desktop, tablet, and mobile devices.

---

## 🛠️ Technical Stack

* **Frontend:** HTML5, CSS3 (Custom Variables & Gradients)
* **Framework:** Bootstrap 5.3 (Grid, Modals, Toasts, Carousel)
* **Icons:** Bootstrap Icons
* **Logic:** Vanilla JavaScript (ES6+)
* **Data Handling:** * `Fetch API` for remote data.
    * `localStorage` for persistent user data and search history.
    * `sessionStorage` for session-state flags.

---

## 📂 Project Structure

```text
.
├── index.html          # Main structure and UI components
├── style (internal)    # Custom modern styling and responsive overrides
└── script (internal)   # Logic for API, Storage, Search, and DOM rendering
```

---

## ⚙️ Logic Workflow

1.  **Initialization:** The app checks `sessionStorage` for an `isActive` flag. If missing, it shows a "New session started" toast.
2.  **Data Retrieval:** * Checks `localStorage` for `users`.
    * If empty, it fetches from the API, saves to `localStorage`, and hides the loading spinner.
3.  **Rendering:** * `carouselData()`: Slices the first 3 users for the top slider.
    * `bodyData()`: Filters the full list based on the search input and renders user cards.
4.  **Search & Persistence:** Every keystroke updates `localStorage.setItem("search", value)`. On reload, the app retrieves this value to keep the UI consistent.

---

## 🚀 How to Run

1.  Clone the repository or copy the code into an `.html` file.
2.  Open the file in any modern web browser.
    * *Note: An active internet connection is required to load Bootstrap CDN and the initial API data.*

---

## ⚠️ Important Notes

* **localStorage Dependency:** If you wish to refresh the data from the API, you must manually clear your browser's Local Storage or use `localStorage.clear()`.
* **Avatar Logic:** Since the API doesn't provide images, the app uses a logic-based placeholder system (alternating images based on User ID).
* **Search Behavior:** The search is **case-insensitive** and ignores leading/trailing whitespace.

---

## 🧠 What I Learned
* Implementing **CRUD-like data persistence** without a backend.
* Building complex UI components (Sliders/Modals) using **document.createElement** for better performance over `innerHTML`.
* Handling asynchronous operations with **Async/Await**.
* Managing UI states (Loading, No Results, and Session Toasts).

---
