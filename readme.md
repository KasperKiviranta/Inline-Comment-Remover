# Inline Code Cleaner

A lightweight, browser-based tool designed to prepare code for production by stripping inline comments and removing comment-only lines. 

It keeps your code clean and reduces file size while preserving the original structure of your logic.

## 🚀 Features

* **Custom Delimiters:** Works with any comment style (`//`, `#`, `--`, `REM`, etc.).
* **Smart Trimming:** * Removes text *after* the specific delimiter.
    * Removes lines that contain *only* comments.
    * Preserves code located before a comment on the same line.
    * Preserves original empty lines to maintain code formatting.
* **Privacy First:** Runs entirely in your browser. No code is sent to any server.
* **User Convenience:** Remembers your last used delimiter (via Local Storage) and includes a one-click "Copy to Clipboard" button.

## 📋 How to Use

1.  **Open:** Double-click the `index.html` file to open it in any web browser.
2.  **Paste:** Paste your source code into the top text box.
3.  **Configure:** Enter your comment symbol in the tiny box (e.g., `//` for JavaScript, `#` for Python).
4.  **Run:** Click **Uncomment**.
5.  **Export:** Click **Copy** to grab the clean code.

## 💡 Example

**Settings:**
* Symbol to remove: `//`

**Input:**
```javascript
const maxUsers = 100; // Set maximum limit

// TODO: Update this later
const minUsers = 5;

function init() {
    start(); // Launch app
}