# Invoice Generator — Built with Claude Code

A professional, browser-based invoice generator that runs entirely as a single HTML file — no backend, no database, no sign-up required. Fill in your business details, add line items, and download a polished PDF invoice in seconds.

## Features

- **Live preview** — a document-chrome preview panel updates in real time as you type, showing exactly what the PDF will look like before you download it
- **Professional PDF output** — coral header bar, two-column business/client layout, alternating-row line items table, highlighted coral total row, and a branded footer
- **Auto-incrementing invoice numbers** — starts at INV-001 and counts up automatically; counter persists across browser sessions via `localStorage`
- **Line items** — add or remove rows dynamically; Quantity × Rate = Amount is calculated automatically
- **Tax support** — optional tax rate field; tax line appears only when a non-zero rate is entered
- **Notes / payment terms** — free-text field rendered in the PDF with a coral accent bar
- **Clear Form button** — resets all fields and advances to the next invoice number in one click
- **Zero dependencies at runtime** — only two CDN scripts (jsPDF + jsPDF-autoTable); works fully offline once loaded
- **Dark SaaS-style UI** — Inter font, `#0f0f1a` background, `#E07A5F` coral accent, card-based layout

## How to Use

1. **Download** — save `invoice-generator.html` to your computer
2. **Open in browser** — double-click the file; no server or installation needed
3. **Fill in & generate** — enter your business info, client details, and line items, then click **Generate & Download Invoice** to save the PDF

## Deploy to Vercel

1. Push `invoice-generator.html` to a GitHub repository (rename it `index.html` or keep the original name)
2. Go to [vercel.com](https://vercel.com), import the repository, and click **Deploy** — no build settings needed
3. Share the live URL with clients so they can access the tool from any browser

## Tech Stack

| Layer | Technology |
|---|---|
| UI & Logic | Vanilla HTML, CSS, JavaScript |
| PDF generation | [jsPDF 2.5.1](https://github.com/parallax/jsPDF) |
| Table rendering | [jsPDF-AutoTable 3.5.28](https://github.com/simonbengtsson/jsPDF-AutoTable) |
| Font | [Inter](https://fonts.google.com/specimen/Inter) via Google Fonts |
| Persistence | Browser `localStorage` (invoice counter) |

---

*Built in under 30 minutes using [Claude Code](https://claude.ai/code) — no coding required.*
