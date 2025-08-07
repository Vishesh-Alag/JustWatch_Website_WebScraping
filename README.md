# 🎬 JustWatch Web Scraping Project

This project demonstrates end-to-end **web scraping**, **data cleaning**, and **analysis** by extracting movie and TV show data from the [JustWatch India](https://www.justwatch.com/in/movies?release_year_from=2000) website using **Selenium**, **BeautifulSoup**, and **Pandas** in a Google Colab environment.

---

## 📌 Objective

Scrape movie and TV show metadata from JustWatch (not using any API), clean and filter the data, perform basic analysis, and save the final dataset in CSV format.

---

## 🚀 Technologies Used

- Python 3
- Google Colab
- Selenium (for dynamic content rendering)
- BeautifulSoup (for HTML parsing)
- Pandas & NumPy (for data manipulation)
- Regular Expressions (`re` module)

---

## 🔍 Data Extracted

For **100 Movies** and **100 TV Shows**, the following details are scraped:

- Title
- Release Year
- Genre(s)
- IMDb Rating
- Duration (Movies only)
- Age Rating
- Production Country
- Streaming Services
- Direct URL to JustWatch Page

---

## 📊 Data Analysis Performed

- Filtered for:
  - Titles released in the **last 2 years**
  - IMDb rating **≥ 7**
- Analytical Insights:
  - Average IMDb ratings
  - Top 5 most common genres
  - Streaming service with the most content offerings

---

## 📁 Output

- ✅ Cleaned and structured dataset exported as:
  - `justwatch_movies_cleaned.csv`
  - `justwatch_tv_shows_cleaned.csv` 
- 📍 Dataset includes clean formatting, standardized genres, and duplicate removal.
- Analysed and Filtered Movies and TVshows exported as :
   - `filtered_movies_2023_2025_imdb7plus.csv` and `filtered_tvshows_2023_2025_imdb7plus.csv`

---

## 🧪 Key Features

- 🔄 Dynamic page handling with Selenium
- 🎯 Robust scraping with fallback mechanisms and error handling
- 🧹 Advanced data cleaning and deduplication
- 📥 CSV export for further reporting/visualization

---

## 🛠️ Setup Instructions

### Option 1: Run on Google Colab (Recommended)
1. Open the Colab notebook: `Web_Scraping_JustWatchWebsite.ipynb`
2. Downlaod this google colab notebook as copy.    
3. Ensure runtime is set to GPU/CPU (no special hardware required).
4. Run all cells sequentially.
5. Final datasets will be saved to your Colab session and downloadable.

### Option 2: Local Environment
> ⚠️ Due to heavy JavaScript usage on JustWatch, **Colab or a properly set up headless Chrome environment is strongly recommended**.

1. Install required libraries:
   ```bash
   pip install selenium beautifulsoup4 pandas
