# ExamTrend.ai — University Question Paper Trend & Pattern Analyzer

**ExamTrend.ai** is an interactive, browser-based analytics platform tailored specifically for university and college semester examinations. It decodes recurring trends, topic weightages, difficulty evolution, and predicts high-yield topics using multi-year question paper datasets.

---

## ✨ Features

### 1. 📊 Interactive Trend & Frequency Dashboard
- **Topic Marks & Question Count Distribution:** View which syllabus modules dominate semester papers over 4-5 years. Toggle seamlessly between *Marks Weightage* and *Question Count*, as well as *Bar* vs *Trend Line* views.
- **Difficulty Evolution (Blooms Taxonomy):** Track how cognitive complexity (Easy / Medium / Hard) shifts across academic terms.
- **Question Format Share:** Donut chart breaking down Problem Solving, Theory, Code / Design, and Proof / Theorem questions.
- **Dynamic Year & Metric Filtering:** Filter by any individual semester or aggregate over the entire multi-year range.

### 2. 🟩 Topic-Year Intensity Heatmap
- Visual color-coded matrix mapping syllabus chapters against consecutive examination years.
- Instantly identify chapters that are tested consistently every semester versus sporadic topics.

### 3. 🔁 Repeat & Pattern Recognition Engine
- Jaccard similarity and token clustering algorithm that detects **identical and semantically recurring questions** across consecutive years.
- Shows total appearances, recurrence rate, and historical mark pool for each hotspot topic.

### 4. 🔮 Upcoming Exam Blueprint (80/20 Pareto Rule)
- **Tier 1 (Guaranteed Core):** Topics appearing in >80% of papers that account for 50-60% of total exam marks.
- **Tier 2 (High-Yield Cyclical):** Topics rotated every 2-3 semesters.
- **Tier 3 (Minor / Optional):** Low-frequency or optional sub-questions.

### 5. 🗂️ Question Bank Explorer
- Complete searchable, filterable repository of all extracted questions.
- Filter by topic, difficulty level, marks (2-3M, 5-7M, 10+M), or free-text search.

### 6. 📄 Universal Ingestion (PDF & Text)
- **PDF Upload:** In-browser multi-page PDF text extraction via PDF.js.
- **Raw Text Paste:** Paste questions directly with an automatic format template.
- **Preloaded Benchmarks:** Instant access to 3 rich, 4 to 5-year university datasets:
  - *Data Structures & Algorithms* (5 Years, 88 Questions)
  - *Operating Systems* (4 Years, 72 Questions)
  - *Database Management Systems* (4 Years, 66 Questions)

### 7. 🖨️ Executive Print & Export
- Formatted Printable / Save-as-PDF summary report.
- One-click JSON data export for custom analysis.

---

## 🚀 How to Run

### Option A: Direct Browser (No setup required)
Simply double-click or open `index.html` in any browser:
```bash
open index.html
```

### Option B: Local Node Server
A lightweight server is included:
```bash
node server.js
```
Then visit [http://localhost:3000](http://localhost:3000) in your browser.

---

## 📁 File Structure
```
Hash_QP_trend/
├── index.html               # Main dashboard UI & modals
├── style.css                # Glassmorphic dark theme & animations
├── app.js                   # Analytics, Chart.js, PDF parser & datasets
├── server.js                # Built-in Node static server
├── sample_paper_cn_2024.txt # Sample university question paper for testing
└── README.md                # Documentation
```
