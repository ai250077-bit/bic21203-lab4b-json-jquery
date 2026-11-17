# bic21203-lab4b-json-jquery

## Student Information
* **Name:** NUR SAKINAH BINTI SABRI
* **Matric / Student ID:** AI250077
* **Course / Section:** BIC21203 — Section 2
* **Lecturer:** Ts. Dr. Ahmad Tajudin Bin Baharin

---

## Project Overview
This repository contains the HTML5, JSON, modern JavaScript (`fetch()`), and jQuery 4.0.0 solutions for **Lab #4b**, demonstrating structured JSON data creation, asynchronous data retrieval with error handling, and jQuery DOM/event manipulation.

### Repository Files
* `books.json` — **Question 1:** Structured JSON dataset containing book records (`title`, `author`, `publicationYear`, `genres`).
* `books.html` — **Question 2:** Web page using `fetch()` and `async/await` to retrieve and safely render selected book details from `books.json`.
* `jquery-dom.html` — **Question 3:** Web page demonstrating jQuery 4.0.0 equivalents (`.text()`, `.addClass()`, and `.on("click", ...)`) for native JavaScript DOM and event operations.

---

## Setup & How to Run
1. Clone or download this repository to your local computer.
2. **Question 1 (`books.json`):** Open in VS Code or any JSON validator to verify valid JSON syntax.
3. **Question 2 (`books.html`):** Must be served over HTTP using a local development server (do **not** open via `file://`, as browsers block local `fetch()` requests due to CORS policy):
   * **Using VS Code Live Server:** Right-click `books.html` and select **Open with Live Server**.
   * **Using Python:** Run `python -m http.server 8000` inside the project folder and visit `http://localhost:8000/books.html`.
4. **Question 3 (`jquery-dom.html`):** Open directly in any modern desktop browser (requires an active internet connection to load the jQuery 4.0.0 CDN).

---

## Implementation Summary & Output Screenshots

### Question 1 — Create and Structure JSON Data (`books.json`)
* **Summary:** Defined a valid top-level `"books"` array containing two objects with properly typed string, number, and array fields, double-quoted keys, and no trailing commas.
* **Evidence Screenshot:**
[books.json](https://github.com/user-attachments/files/34970480/books.json)

[{
  "books": [
    {
      "title": "The Great Gatsby",
      "author": "F. Scott Fitzgerald",
      "publicationYear": 1925,
      "genres": ["Fiction", "Classics"]
    },
    {
      "title": "To Kill a Mockingbird",
      "author": "Harper Lee",
      "publicationYear": 1960,
      "genres": ["Fiction", "Coming-of-Age"]
    }
  ]
}Uploading books.json…]() 
<img width="1194" height="706" alt="Screenshot 2026-11-17 195940" src="https://github.com/user-attachments/assets/25448b8e-80fa-4b69-8ca0-2f808d055525" />




---

### Question 2 — Retrieve and Display JSON Data (`books.html`)
* **Summary:** Uses `fetch("books.json")` with `try...catch` error handling and safe DOM creation (`document.createElement()` and `textContent`) to display the first book's title, the second book's author, and the genres grouped by book title.
* **Output Screenshot:**
 [books.html](https://github.com/user-attachments/files/34970541/books.html)

<img width="589" height="496" alt="Screenshot 2026-11-17 200358" src="https://github.com/user-attachments/assets/cc4eceb6-0799-4c6c-a931-0247dc499fc3" />



---

### Question 3 — Compare Native JavaScript and jQuery (`jquery-dom.html`)
* **Summary:** Loads the official jQuery 4.0.0 full-build CDN and uses `.text()`, `.addClass()`, and `.on("click", ...)` to update `#myElement`, style `#myDIV` with `.myStyle`, and trigger an alert on `#myButton` click.
* **Output Screenshot:**
 [jquery-dom.html](https://github.com/user-attachments/files/34970576/jquery-dom.html)

<img width="883" height="235" alt="Screenshot 2026-11-17 200703" src="https://github.com/user-attachments/assets/4fedffa3-dc53-4df4-b7c6-5838604836d1" />
<img width="880" height="537" alt="Screenshot 2026-11-17 200716" src="https://github.com/user-attachments/assets/fbd8847e-8169-43c4-b903-61f195173d4b" />
