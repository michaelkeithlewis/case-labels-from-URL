# Case Labels — for Truck Packer

Generate printable PDF case labels from any [Truck Packer](https://www.truckpacker.com/) crewview link. Designed for production teams, tour managers, and logistics professionals.

## How It Works

1. **Drag the bookmarklet** to your bookmarks bar (one-time setup)
2. Open any Truck Packer crewview page
3. Click the bookmarklet — extracts case names, colors, and order numbers
4. Paste into the app — see a live preview
5. Configure label size, style, and content
6. **Download a PDF** ready to print

## Features

- **PDF download** — clean vector PDFs via jsPDF, no print dialog headaches
- **Universal label sizing** — 4×6 thermal, 4×2 Avery, 3×2, custom dimensions, portrait or landscape
- **Three styles** — Color Fill, Color Outline, and Black & White
- **Live preview** — see exactly what your labels look like before downloading
- **Text sizing sliders** — adjust case name, order #, and show name independently
- **Logo upload** — add your logo to every label
- **Category colors** — extracted from Truck Packer's colored icons
- **Wizard UI** — step-by-step flow built with Tailwind CSS

## Deploying

This is a static single-page app — just `index.html` with CDN dependencies. Deploy anywhere:

- **Vercel**: `vercel --prod`
- **Netlify**: drag the folder into Netlify Drop
- **GitHub Pages**: push to `main`, enable Pages in repo settings
- **Any static host**: upload `index.html`

No build step required.

## Tech Stack

- Single `index.html` file
- [Tailwind CSS](https://tailwindcss.com/) via CDN
- [jsPDF](https://github.com/parallax/jsPDF) for PDF generation
- [Inter](https://fonts.google.com/specimen/Inter) typeface via Google Fonts
- No build tools, no framework, no server

## License

MIT — free to use and modify.
