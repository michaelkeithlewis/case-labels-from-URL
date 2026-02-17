# Case Label Printer — for Truck Packer Crewview

A standalone HTML tool that generates printable case labels from [Truck Packer](https://www.truckpacker.com/) crewview pack links. No server required — just open the HTML file in your browser.

## Quick Start

1. Open `index.html` in any modern browser
2. Click **Load Demo** to see it in action with sample data
3. Navigate through the 4 tabs: **Input → Review → Settings → Preview & Print**

## Getting Data from Truck Packer

### Method 1: Bookmarklet (Recommended)

1. Open `index.html` in your browser
2. Drag the **"📋 Extract Cases"** button to your bookmarks bar
3. Open your Truck Packer crewview link (e.g. `https://app.truckpacker.com/packs/...`)
4. Click the bookmarklet — it copies the case data to your clipboard
5. Go back to the Case Label Printer and paste the data

### Method 2: Copy & Paste

1. Open your Truck Packer crewview link
2. Select and copy the case list from the page
3. Paste into the text area in the Case Label Printer
4. The parser supports: JSON, CSV, tab-separated, and plain text

### Method 3: Manual Entry

Use the manual entry form to add cases one at a time with name, quantity, dimensions, color, and category.

## Supported Input Formats

| Format | Example |
|--------|---------|
| **JSON** | `[{"name": "FOH Rack", "qty": 2, "dimensions": "44x24x36", "color": "#4f8cff", "category": "Audio"}]` |
| **CSV** | `Name, Qty, Dimensions, Color, Category` (header row + data rows) |
| **Tab-separated** | Paste directly from spreadsheets |
| **Plain text** | One case name per line; supports `2x FOH Rack` quantity prefix |

## Label Settings

- **Layout:** 2-column (Avery 5163), 1-column (full width), or 3-column (small labels)
- **Sort by:** Input order, name, category, or color
- **Font size:** Small, medium, large, or extra large
- **Toggle fields:** Sequence number, dimensions, color bar, category, weight, pack name, quantity

## Printing

1. Configure your labels in the **Settings** tab
2. Go to the **Preview & Print** tab to see how they'll look
3. Click **Print Labels** — the browser print dialog opens with a print-optimized layout
4. For best results, set margins to "Minimum" or "None" in the print dialog

### Label Sheet Compatibility

| Layout | Labels per Page | Compatible With |
|--------|----------------|-----------------|
| 2 Columns | 10 per page | Avery 5163, 8163 (4" × 2") |
| 1 Column | ~6 per page | Full-width adhesive stock |
| 3 Columns | 15 per page | Avery 5160, 8160 (2.63" × 1") |

## Features

- Zero dependencies — single HTML file, works offline
- Dark-themed UI for comfortable use
- Print-optimized CSS with proper page breaks
- Color-coded labels by department/category
- Expand quantities into individual labels (e.g. Qty 3 = 3 separate labels)
- Export items to CSV
- Bookmarklet for extracting data from Truck Packer pages

## License

Free to use. Built as a companion tool for Truck Packer crewview links.
