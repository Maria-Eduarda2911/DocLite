# ⚡ DocLite 

> **Universal file viewer 100% offline, secure, and lightweight.**

**DocuLite** is a *single-file* tool that allows you to open, view, and analyze spreadsheets and documents directly in the browser, without uploading them to any server.

[![Watch the Demo Video](https://img.youtube.com/vi/sicFI6fTIcs/maxresdefault.jpg)](https://youtu.be/sicFI6fTIcs)
> *Click the image above to watch the demo video.*
![Main Screen](/prints/8b76e80c-3476-4fdb-a5e0-f83256ad7a39.jpg)

---

## 🎯 Purpose and Usability

The project was born from the need to view heavy files or various formats quickly, without relying on proprietary software (like Office) or online converters that compromise data privacy.

### Usability Highlights:
* **Persistent History:** Thanks to **IndexedDB**, your files are saved within the browser. You can close the tab and come back later, and the file will open instantly without annoying security alerts.
* **Comfortable Reading:** Documents (PDF/DOCX) are rendered in a "paper sheet" layout with drop shadows, centered alignment, and optimized zoom.
* **Native Text Selection:** Copy text from PDFs and DOCX files without broken formatting or strange visual blocks.
* **Visual Feedback:** The system notifies you when text is copied or when a file is being processed.

---

## 🚀 Key Features

### 1. Data Analysis (CSV and Excel)
Transforms raw files into interactive, modern tables.
* **Smart Processing:** Automatically detects **Currency** columns (right-aligned, green color), **Dates** (converts Excel serial numbers e.g., `45929` to `09/15/2025`), and **Text**.
* **Grid Mode:** Option to view data like classic Excel.
* **Advanced Filters:** Filter by column or use the global search.

![Table View](/prints/{D3642435-A0ED-48E5-B625-C5FEBE12CF6C}.png)

### 2. Document Viewer (PDF and Word)
Faithful rendering of text documents.
* **PDF:** Canvas rendering with a transparent text layer for precise selection.
* **DOCX:** Clean conversion to HTML, maintaining paragraph and title structure.

![PDF Viewer](/prints/f600fb7b-3b79-4601-9f44-1a1ed0fe7945.jpg)
![DOCX Viewer](/prints/ed1cbe1c-df65-44f3-9bc8-da4ebed8bae8.jpg)

### 3. Productivity Tools
* **Details Modal:** Click on any table row to see data in organized cards. Links (HTTP/HTTPS) automatically become clickable buttons.
* **Quick Search:** Optimized search bar in the header.

![Details Modal](/prints/{FFCDC16B-911B-464F-BD4E-DA36749A4E02}.png)
![Links in Modal](/prints/{86CB511B-C368-4F4F-B000-E819FDF33444}.png)

---

## 🛠️ How it was made (Technology)

DocuLite was built with a **Zero-Backend** philosophy. All logic resides in a single HTML file containing minified CSS and JS for maximum performance.

### Technologies:
* **Core:** HTML5, CSS3 (with CSS Variables), Vanilla JavaScript (ES6+).
* **Storage:** `IndexedDB` (NoSQL database inside the browser) for caching large files.
* **Icons:** Lucide Icons.

### Processing Libraries:
* `PapaParse`: For ultra-fast CSV parsing.
* `SheetJS (XLSX)`: For reading and converting Excel spreadsheets.
* `Mammoth.js`: To convert .docx to clean HTML.
* `PDF.js`: Mozilla technology to render PDFs with precision.

---

## 📦 How to Use

1.  Download the `DocLite.html` file.
2.  Open it in any modern browser (Chrome, Edge, Firefox, Brave).
3.  Drag a file or click on **Import**.
4.  Your recent files will appear in the sidebar automatically.

### Supported Formats
| Type | Extensions |
| :--- | :--- |
| Spreadsheets | `.csv`, `.xlsx`, `.xls` |
| Documents | `.docx`, `.doc`, `.pdf` |
| Data/Text | `.json`, `.txt` |

---

*Developed by Maria Eduarda.*
