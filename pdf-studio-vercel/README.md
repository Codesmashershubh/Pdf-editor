# PDF Studio — Free Browser-Based PDF Editor

A fully free, browser-based PDF editor. No backend, no database, no API keys.  
All PDF processing happens client-side using PDF.js and pdf-lib.

---

## Project Structure

```
pdf-studio/
├── index.html      ← The entire application (single file)
├── vercel.json     ← Vercel deployment configuration
└── README.md       ← This file
```

---


## Cost

| Resource        | Cost       |
|----------------|------------|
| Vercel Hosting  | Free (Hobby plan) |
| PDF.js CDN      | Free (cdnjs / Cloudflare) |
| pdf-lib CDN     | Free (cdnjs / Cloudflare) |
| Google Fonts    | Free       |
| **Total**       | **$0**     |


---



---

## Features

- ✅ Open & view PDF files
- ✅ Edit existing text in PDFs (click any text with Select tool)
- ✅ Add new text annotations
- ✅ Freehand drawing & highlighting
- ✅ Eraser tool
- ✅ Merge multiple PDFs
- ✅ Delete individual pages
- ✅ Extract a single page as a new PDF
- ✅ Zoom in / out
- ✅ Page thumbnails panel
- ✅ Download edited PDF
- ✅ Keyboard shortcuts
- ✅ Drag & drop file open
- ✅ Works on mobile

---

## Libraries Used

| Library   | License | Version |
|-----------|---------|---------|
| [PDF.js](https://mozilla.github.io/pdf.js/) (Mozilla) | Apache 2.0 | 3.11.174 |
| [pdf-lib](https://pdf-lib.js.org/) | MIT | 1.17.1 |
| [Inter](https://rsms.me/inter/) (Google Fonts) | OFL-1.1 | — |

All served from [cdnjs.cloudflare.com](https://cdnjs.cloudflare.com) — no npm install required.
