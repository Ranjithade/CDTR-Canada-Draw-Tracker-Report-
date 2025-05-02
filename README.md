# 🇨🇦 Canada Immigration Draw Tracker

A Python-based tool that scrapes and aggregates the latest immigration draw results from key Canadian programs, and outputs them in a clean, tabbed HTML report for easy monitoring and comparison.

## 📌 Features

- ✅ Scrapes official data from:
  - Express Entry (IRCC)
  - Ontario Immigrant Nominee Program (OINP)
  - Saskatchewan Immigrant Nominee Program (SINP)
  - British Columbia PNP (BC PNP)
  - Alberta Advantage Immigration Program (AAIP)
  - Manitoba EOI Draws
  - Quebec Regular Skilled Worker Program (RSWP)

- 🧾 Converts draw tables (HTML or PDF) into structured formats
- 🗂️ Generates a unified, tabbed HTML dashboard
- 📤 Optional support for PDF downloads and email alerts
- 🔄 Easily extensible to new provinces or programs

## 📁 Output

The script produces an HTML file that contains:
- Tabs for each program
- Tables with key details: invitation dates, streams, number of invitations, and cut-off scores
- Optional downloadable PDFs (e.g., SINP selection results)



## 🛠️ Technologies Used

- `requests`, `BeautifulSoup` – web scraping
- `pandas` – optional table handling
- `pdfplumber` – PDF parsing (for SINP)
- HTML/CSS – report styling
- AWS Lambda/S3/SES – optional for automation (deployment use case)

## 🚀 Usage

1. Clone the repository:
   ```bash
   git clone https://github.com/yourusername/canada-immigration-draw-tracker.git
   cd canada-immigration-draw-tracker

Install dependencies:

pip install -r requirements.txt
python main.py
