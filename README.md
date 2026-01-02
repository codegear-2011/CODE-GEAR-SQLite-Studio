# 🧠 CODE GEAR SQLite Studio
### A Full-Featured Browser-Based SQLite Database Studio
[![chrome-screenshot-2-ja-na-2026-9-46-25-AM-IST.jpg](https://i.postimg.cc/Pf0SffWQ/chrome-screenshot-2-ja-na-2026-9-46-25-AM-IST.jpg)](https://postimg.cc/s19Ywr0M)
**CODE GEAR SQLite Studio** is a powerful, modern, browser-based SQLite database manager built entirely with **HTML, CSS, and JavaScript**, running **100% on the client side**.  
It allows you to **open, explore, query, modify, and export SQLite databases** directly from your browser — **without installing SQLite, without a backend, and without a server**.

---

## 📌 Key Highlights

- ✅ **Runs completely in the browser** - No installation required.
- ✅ **Real SQLite Engine** - Uses SQL.js (WebAssembly).
- ✅ **VS Code-style Editor** - Powered by Monaco Editor for a pro coding experience.
- ✅ **Privacy Focused** - No data leaves your device; everything stays local.
- ✅ **Offline Ready** - Works offline after the first load.
- ✅ **Modern UI** - Clean, dark interface inspired by professional DB tools.

---

## 🖼️ Application Overview

The interface is divided into four main sections:

1. **Header Bar**: File loader, database name display, and export/download button.
2. **Left Sidebar (Tables Panel)**: Automatically lists all user-defined tables for instant preview.
3. **Main Content Area**: Scrollable result grid with sticky headers and row numbers.
4. **Footer (SQL Execution Bar)**: Monaco Editor for writing and executing SQL queries.

---

## ✨ Features (Detailed)

### 📂 Database Loading & Export
- Supports `.db` and `.sqlite` files.
- Uses **FileReader API** to load databases into memory instantly.
- **Export Feature**: Save your modified database as a new file (renamed as `originalname_modified.db`).

### ✍️ Monaco SQL Editor
- Same core as **VS Code**.
- SQL syntax highlighting & dark theme (`vs-dark`).
- Auto-layout resizing and monospaced font.

### 📋 Table Browser & Result Viewer
- Click a table to auto-run `SELECT * FROM table_name LIMIT 200;`.
- Sticky headers for easy navigation through large datasets.
- Handles wide tables with graceful horizontal scrolling.

---

## 🛠️ Technologies Used

| Technology | Purpose |
| :--- | :--- |
| **HTML5** | Application structure |
| **CSS3** | Dark theme UI styling |
| **JavaScript (Vanilla)** | Core logic |
| **SQL.js** | SQLite engine via WebAssembly |
| **Monaco Editor** | SQL editor |
| **FileReader API** | Local file loading |
| **Blob API** | Database export |

---

## 🚀 Getting Started

### Method 1: Run Locally
1. Save your code as `index.html`.
2. Open it in a modern browser (Chrome, Edge, Firefox).
3. Load a `.db` file and start querying.

### Method 2: Host Online
Deploy as a static site using **GitHub Pages**, **Netlify**, or **Vercel**. No backend configuration is required.

---

## 🧪 Example SQL Queries

```sql
-- List all tables
SELECT name FROM sqlite_master WHERE type='table';

-- Create a new table
CREATE TABLE users (
  id INTEGER PRIMARY KEY AUTOINCREMENT,
  name TEXT,
  email TEXT
);

-- Insert Data
INSERT INTO users (name, email) VALUES ('Barun Saha', 'barun@example.com');
```
---

## 👨‍💻 Author

**CODE GEAR** *A developer-focused project for learning, experimentation, and practical SQLite usage.*

---

## 📜 License

This project is **open-source** and free to use for:
* 🎓 Educational purposes
* 💻 Personal projects
* 🧪 Learning & experimentation

You are free to modify, extend, and redistribute it.

---
