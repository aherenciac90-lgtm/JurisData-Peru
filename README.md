# JurisData Peru 🇵🇪

**An open-source legal data infrastructure for Peruvian Jurisprudence and Doctrine.**

## 📖 Overview
Access to structured legal information in Peru is highly fragmented. Crucial jurisprudence—especially in specialized fields such as Administrative Law (Ley 27444), Municipal governance, Public Investment (Obras por Impuestos), and Real Estate/Registry Law—is often locked in scanned, non-searchable PDFs scattered across various governmental portals (e.g., Tribunal Registral, OSCE, Tribunal Constitucional). 

**JurisData Peru** is an open-source initiative designed to scrape, extract, parse, and structure these legal documents into machine-readable datasets. Our goal is to democratize legal research and provide the foundational data layer for civic tech and legal-tech applications (such as RAG systems and NLP analysis) in Latin America.

## 🎯 Objectives
*   **Data Extraction:** Build robust scrapers to collect public resolutions and legal doctrine from Peruvian government portals.
*   **Document Parsing:** Implement OCR and NLP pipelines to convert unstructured PDFs into clean, searchable text.
*   **Metadata Structuring:** Use LLMs to automatically extract key entities: *Ratio Decidendi*, cited norms, legal principles, and resolution outcomes.
*   **Open Datasets:** Publish structured JSON/CSV datasets for public use, academic research, and AI model training.

## 🏗️ Architecture & Tech Stack (Planned)
*   **Scraping:** Python, BeautifulSoup, Selenium / Playwright
*   **PDF Processing:** pdfplumber, Tesseract OCR
*   **Data Structuring & NLP:** LangChain, LlamaIndex, OpenAI/Anthropic APIs
*   **Database:** PostgreSQL / SQLite
*   **API:** FastAPI (Future roadmap)

## 📂 Project Structure (Draft)
```text
├── data/                  # Raw and processed datasets (JSON/CSV)
├── scrapers/              # Scripts to extract data from government portals
│   ├── tribunal_registral/
│   └── osce/
├── processors/            # NLP and OCR scripts for PDF parsing
├── notebooks/             # Jupyter notebooks for data analysis and LLM testing
├── docs/                  # Documentation and legal data taxonomy
├── requirements.txt       # Python dependencies
└── README.md
