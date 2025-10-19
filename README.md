# Prematips Football Prediction Scraper

This project automates the process of scraping football prediction data from **Primatips.com** using **Requests** and **BeautifulSoup**. It collects match predictions such as **1X2**, **Over/Under 2.5**, and **Both Teams to Score (BTS/OTS)** for the current date, merges them into a single clean dataset, and saves the results as a CSV file for easy analysis.

---

## 🚀 Features
- Automatically fetches football prediction data from Primatips.
- Extracts and merges:
  - **1X2 predictions** (Home, Draw, Away percentages)
  - **Over/Under 2.5 goals predictions**
  - **Both Teams to Score predictions**
- Cleans, merges, and removes duplicate entries.
- Saves data as a **CSV file** inside a daily folder.
- Ready for further analysis or use in football betting strategy models.

---

## ⚙️ Setup

### 1. Clone the repository
```bash
git clone https://github.com/yourusername/prematips-data-scraper.git
cd prematips-data-scraper
2. Install dependencies

Make sure you have Python 3 installed, then run:
pip install pandas beautifulsoup4 requests

3. Project structure
prematips-data-scraper/
│
├── func.py
├── prematips.py
└── README.md
Note: func.py must contain helper functions such as
save_daily_csv, drop_duplicate, and main_date.

▶️ Usage

Simply run:
python prematips.py
The script will:

Automatically fetch match data for today’s date.

Merge all prediction categories into one DataFrame.

Save the final data to a CSV file named prematips.csv inside the daily folder.

📊 Output Example

A sample output saved as prematips.csv:
DATE,TIME,HOME TEAM,AWAY TEAM,HOME PER,DRAW PER,AWAY PER,UNDER 2.5,OVER 2.5,BTS,OTS,NAME
2025-10-19,14:00,Arsenal,Chelsea,55%,25%,20%,40%,60%,65%,35%,PREMA
2025-10-19,16:00,Real Madrid,Barcelona,48%,28%,24%,45%,55%,50%,50%,PREMA

💡 Example Use Case

You can integrate this data into:

A machine learning football betting model.

A Kelly Criterion-based bankroll system.

A dashboard that compares predictions across multiple sites.

Or simply for tracking prediction accuracy over time.

🧰 Tech Stack

Python 3

Requests – for fetching HTML data.

BeautifulSoup4 – for web scraping.

Pandas – for data manipulation and merging.

Time module – for handling match date/time.

👨‍💻 Author

Ezee Kits
Passionate about automation, data analysis, and Python programming.
📺 YouTube: Ezee Kits

📄 License

This project is licensed under the MIT License – you are free to use, modify, and distribute it with attribution.
