# 💬 Quote Generator

A simple and interactive **Quote Generator** built with **HTML, CSS, and JavaScript**. The application fetches random quotes from the **DummyJSON Quotes API** and displays the quote along with its author.

Users can generate a new quote with a single click and share the displayed quote through Twitter/X.

---

## 📌 Overview

The Quote Generator is a frontend web application designed to demonstrate how JavaScript can communicate with a third-party REST API and dynamically update the webpage with the returned data.

When the application loads, it automatically fetches a random quote. Users can then generate additional quotes using the **New Quote** button or share the current quote using the **Tweet** button.

---

## ✨ Features

* 💬 Fetches random quotes from an external API
* 🔄 Generates a new quote with one click
* 👤 Displays the quote author
* 🐦 Tweet/share button for the current quote
* ⚡ Asynchronous API requests using `fetch()`
* 🛡️ Basic API error handling
* 🎨 Clean quote-card interface
* ✨ Styled typography using Google Fonts
* 📱 Simple browser-based frontend application

---

## 🛠️ Technologies Used

| Technology            | Purpose                                  |
| --------------------- | ---------------------------------------- |
| **HTML5**             | Application structure                    |
| **CSS3**              | Layout, styling, typography, and buttons |
| **JavaScript (ES6+)** | API integration and dynamic content      |
| **Fetch API**         | Retrieving random quotes                 |
| **DummyJSON API**     | Source of random quotes                  |
| **Google Fonts**      | Playfair Display typography              |

---

## 🌐 API Used

This project uses the **DummyJSON Quotes API**:

```text
https://dummyjson.com/quotes/random
```

The API response provides the quote text and author, which are then displayed dynamically on the webpage.

---

## 📂 Project Structure

```text
Quote-Generator/
│
├── images/
│   └── tweet-icon.png
│
├── index.html
├── script.js
├── style.css
└── README.md
```

The repository currently contains the `images` directory along with the three main frontend files.

---

## ⚙️ How It Works

### 1. Initial Quote Loading

When the page loads, JavaScript automatically calls:

```javascript
getQuote();
```

This means the user sees a quote without having to click the **New Quote** button first.

### 2. Fetching a Random Quote

The application sends an asynchronous request to:

```javascript
const api_url = "https://dummyjson.com/quotes/random";
```

The `fetch()` API retrieves the JSON response.

### 3. Displaying the Quote

The returned data is used to update the page:

```javascript
quote.innerHTML = data.quote;
author.innerHTML = data.author;
```

The quote is displayed inside the `<blockquote>` element and the author is displayed below it.

### 4. Generating Another Quote

Clicking **New Quote** calls:

```javascript
getQuote()
```

which sends another request to the API and replaces the current quote with a new one.

### 5. Sharing the Quote

The **Tweet** button calls:

```javascript
tweet()
```

The function opens Twitter/X's intent URL and includes the currently displayed quote and author in the text.

### 6. Error Handling

If the API request fails, the application displays:

```text
Something went wrong
```

and clears the author field while logging the error to the console.

---

## 🧠 JavaScript Concepts Practiced

This project provides practical experience with:

* DOM manipulation
* `getElementById()`
* Functions
* `async/await`
* `fetch()`
* Promises
* JSON responses
* `try...catch`
* Updating HTML dynamically
* Event handling
* Browser `window.open()`
* API integration
* Error handling

---

## 🎨 UI Design

The interface uses a centered white quote card placed over a light blue background.

The styling includes:

* Centered quote container
* Rounded corners
* Box shadow
* Large quote typography
* Author attribution
* Blue accent color
* Rounded action buttons
* Tweet icon
* **Playfair Display** Google Font

The quote card is styled in `style.css`, including its layout, typography, buttons, and tweet icon.

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/KhushiChaubey-493/Quote-Generator.git
```

### 2. Navigate to the project

```bash
cd Quote-Generator
```

### 3. Run the project

Open:

```text
index.html
```

in a modern web browser.

No backend, database, package manager, or build tool is required.

---

## 📸 Project Preview

If you add a screenshot to the repository, you can display it in this section:

```markdown
![Quote Generator Screenshot](screenshot.png)
```

---

## 🎯 Learning Objectives

This project was built to practice:

* Consuming a REST API from a frontend application
* Working with asynchronous JavaScript
* Using `fetch()` and `async/await`
* Processing JSON API responses
* Updating the DOM dynamically
* Handling API failures
* Opening external sharing links
* Building a clean frontend interface

---

## 🔮 Future Improvements

Possible future enhancements include:

* Add a **Copy Quote** button.
* Add a loading indicator while fetching quotes.
* Add a dedicated API error message in the UI.
* Add quote categories.
* Add favorite quotes using `localStorage`.
* Add Facebook/LinkedIn sharing.
* Add responsive improvements for smaller screens.
* Add smooth transitions when changing quotes.
* Disable the button while a request is in progress.
* Add a quote history section.

---

## 📌 Project Status

**Status:** Completed

This is a frontend JavaScript project focused on **REST API integration, asynchronous programming, DOM manipulation, and social sharing functionality**.

---

## 👩‍💻 Author

**Khushi Chaubey**

GitHub:
https://github.com/KhushiChaubey-493

---

## 📄 License

This project is available for educational and personal use.
