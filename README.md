# Indian Tax Code Dataset Preparation for Continued Pretraining

This project aims to collect and curate high-quality Indian tax law text data for continued pretraining or fine-tuning of language models. The corpus includes data scraped from government websites, legal resources, and official PDF documents.

## 📂 Project Structure

- `scraped/` – Contains HTML and PDF-extracted raw text files.
- `indian_tax_code_combined.txt` – Combined output from all scraped sources.
- `indian_tax_code_special_sources.txt` – Output from special handling (problematic URLs).
- `indian_tax_code_full.pdf` – Official PDF document of the Indian Tax Code.
- `indian_tax_code_final_corpus.txt` – Final merged dataset ready for model training.

## 🛠️ Technologies Used

- Python
- `requests`, `BeautifulSoup` – For HTML scraping
- `pdfplumber` – For PDF text extraction
- `pandas`, `openpyxl` – For handling URL lists from Excel

## 🚀 How It Works

1. URLs of relevant sources are stored in an Excel sheet.
2. A scraper fetches and cleans content from those URLs.
3. PDF documents are parsed using `pdfplumber`.
4. All text sources are combined into a single plain text corpus.

## ✅ Output

The final output, `indian_tax_code_final_corpus.txt`, contains clean, plain-text content from multiple sources — suitable for continued pretraining, supervised fine-tuning (SFT), or legal NLP research.

## 🔍 Use Cases

- Continued pretraining on Indian legal text
- Domain-specific fine-tuning for legal question-answering systems
- Tax law chatbot development
- Named entity recognition and document classification in Indian finance/law

## 📌 License

This dataset is intended for educational and research purposes. Verify the licensing of the scraped content before commercial use.
