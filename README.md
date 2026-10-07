# PDF Toolkit

A free, fully offline PDF toolkit in a **single HTML file**. Download it, double-click it, and it runs in your browser. No install, no server, no account, and your files never leave your computer.

## Features

| Tool | What it does |
|---|---|
| 🧩 **Merge** | Combine several PDFs into one. Drag or use the arrows to set the order. |
| 🗜️ **Compress** | Shrink scanned or image-heavy PDFs (low / medium / high). |
| ✂️ **Split** | Extract page ranges like `1-3,5,8-10`, or split every page into its own PDF (downloaded as one `.zip`). |
| 🗂️ **Reorder / Delete** | Drag page thumbnails to reorder, delete pages, rotate single pages. |
| 🔄 **Rotate** | Rotate all pages or only the ones you pick. |
| 📑 **Extract** | Click the pages you want and save them as a new PDF. |
| 📝 **Convert to Word** | Turn a PDF into an editable `.docx`, or an image-based `.docx` that looks identical to the original. |

## Usage

1. Download [`PDF_Toolkit.html`](PDF_Toolkit.html) (on GitHub: open the file → **Download raw file**).
2. Open it in any modern browser (Chrome, Edge, Firefox).
3. Pick a tool, drop in your PDF, and download the result.

It works with no internet connection, so it's safe for confidential documents and usable on locked-down or air-gapped machines.

## Privacy & security

- All processing happens locally in the browser with JavaScript.
- No network requests: every library is bundled inside the HTML file, with no CDN and no analytics.
- You can verify this yourself by opening the browser DevTools → Network tab while using it.

## Limitations

- **Compress** re-renders pages as images, so text in the compressed file is no longer selectable or searchable. Text-only PDFs may not get smaller.
- **Convert to Word** is best-effort. Complex layouts, tables and multi-column text may not be preserved exactly. Scanned pages are kept as images (there is no OCR).
- **Password-protected PDFs** aren't supported. Remove the protection first (open the file and "Print to PDF").
- Very large PDFs (hundreds of pages) depend on your browser's memory.

## Built with

| Library | Purpose | License |
|---|---|---|
| [pdf-lib](https://github.com/Hopding/pdf-lib) | Creating and editing PDFs | MIT |
| [PDF.js](https://github.com/mozilla/pdf.js) | Rendering pages and extracting text | Apache 2.0 |
| [docx](https://github.com/dolanmiu/docx) | Generating Word documents | MIT |

The libraries are embedded unmodified in the HTML file and keep their original licenses.

## License

MIT, see [LICENSE](LICENSE).
