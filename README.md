# Series Searcher

A fast, browser-based search tool for exploring word and phrase occurrences across multiple fantasy and fiction series 
The tool automatically fetches the EPUB files, parses them client-side, and displays every match—organized by **series → book → chapter → occurrence**.

Future updates will add support for additional book series.

---

## Features

- **Full-text search** across multiple series
-  **Automatic EPUB fetching** — no renaming or configuration required  
-  Results grouped by **book → chapter → occurrence**  
- Expand/collapse navigation for clean browsing  
-  Clickable occurrences that open a **modal with sentence-level context**  
-  Fully client-side — **no server needed**  
-  **Batch multi-word searching** via console script  

---

## Installation

Download only the files you want:

| File | Purpose |
|------|---------|
| `main/Series Searcher Code.html` | Main search interface |
| `main/Multiple occurences.html` | Batch-search console script |

### Steps
1. Download the `.html` file(s).  
2. Open them in any modern web browser (**Chrome recommended**).  
3. No configuration is required — EPUBs are fetched automatically.

---

##  How to Use

### Standard Search
1. Open **Series Searcher Code.html**.  
2. In the sidebar, select any book or series or use the 'Select all' option to select all series
3. Enter a word or phrase in the search bar.  
4. Press **Enter** or click **Search**.  
5. Explore results grouped by:
   - Book  
   - Chapter  
   - Occurrence  
6. Click any occurrence to open a **context modal** showing the sentence where it appears.

---

## Multiple-Term Batch Search (Console Script)

1. Open **Multiple occurences.html**.  
2. Copy the script displayed in the file.  
3. With the searcher open in Chrome, open **DevTools → Console**.  
4. Paste the script.

Default placeholder:

```js
const words = ["example", "word", "list"];
```
Replace with your own array.  
Each term is searched individually, and results are output in a table.

---

## Tech Stack

- **HTML**, **CSS**, **JavaScript**
- **JSZip** for EPUB extraction
- Browser APIs:
  - `DOM`
  - `MutationObserver`
- 100% client-side — **no backend required**

## Configuration

No configuration is necessary.  
EPUBs are fetched automatically and parsed in-browser.

To batch-search multiple terms, edit the `words` array in `Multiple occurences.html`.

---

## 📄 License

**MIT License**
MIT License

Copyright (c) 2025 underscorep2

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.

---
