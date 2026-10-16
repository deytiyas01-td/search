# Searchable Listing Dashboard

A modern, responsive, and high-performance searchable listing dashboard built with **HTML5**, **Tailwind CSS**, and **Vanilla JavaScript (ES6+)**[cite: 3]. This application is designed for instant data filtering, real-time debounced searching, multi-category selection, sorting, pagination, and robust empty/error state handling[cite: 3].

---

## 🎯 Objective & Scope

* Display project or job listings with search, category filters, sorting, pagination, and empty/error states[cite: 3].
* Provide a seamless, performant user experience across both desktop and mobile viewports.

---

## 🛠️ Recommended Stack & Tools

* **Markup & Layout:** HTML5, CSS3, Tailwind CSS (Flexbox & Grid)[cite: 3]
* **Logic & Interactivity:** Vanilla JavaScript (ES6+, Fetch API/Array Methods)[cite: 3]
* **Data Source:** Sample mock JSON dataset containing at least 12 distinct listing entries[cite: 3].

---

## 🔍 Search Algorithms & Debouncing Logic

1. **Live Debounced Search:**
   * To prevent excessive re-rendering and maintain high performance during rapid typing, the search input utilizes a **250ms debounce timer**. 
   * When a user types in the search box, the timer resets on every keystroke (`clearTimeout` / `setTimeout`), triggering the filtering logic only after the user stops typing.

2. **Logical AND Combination Filtering:**
   * Multiple filters (Search query, Domain dropdown, Experience level dropdown, and Remote-only toggle) work simultaneously in combination using a logical `AND` operation[cite: 3]. 
   * A listing is only displayed if it satisfies all active filter criteria simultaneously.

3. **Multi-Field Keyword Matching:**
   * The search algorithm checks input terms against the listing title, company name, and the entire array of required skills to ensure accurate results.

---

## 🖥️ UI States & Components

* **Dynamic Card Grid:** Renders responsive cards with badges, metadata, skill tags, and interactive "Apply Now" triggers.
* **Empty State View:** Automatically displays an animated and user-friendly empty state screen with a "Clear All Filters" button whenever zero listings match the active search criteria[cite: 3].
* **Pagination Control:** Dynamically calculates total pages and displays responsive pagination buttons to navigate large datasets smoothly.

---

## ✅ Acceptance Criteria Checklist

* [x] **Combined Filters:** Search and category filters work in logical combination (logical AND)[cite: 3].
* [x] **Empty State Handling:** Empty state clearly displays when zero listings match the search criteria[cite: 3].
* [x] **High Performance:** Performant client-side filtering without perceptible lag[cite: 3].
* [x] **Responsive Design:** Optimized layout for mobile phone screens and desktop viewports.

---

## 🚀 Deliverables Included

* **Application Codebase:** Fully responsive single-file or modular implementation with live hosted preview readiness[cite: 3].
* **Mock JSON Dataset:** 12 distinct listing entries with robust metadata and skills[cite: 3].
* **Documentation:** Detailed `README.md` covering search algorithms, debouncing, and UI states[cite: 3].
