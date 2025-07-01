
# 🧠 Textual Analysis & Web Scraping Project with Python

This project automates the process of **scraping article content from URLs**, cleaning and processing text, and performing **natural language processing (NLP)** to analyze the **polarity, subjectivity, and sentiment** of the content.

It uses tools such as **BeautifulSoup** for web scraping, **NLTK** for natural language processing, and **pandas** for data handling and Excel export.

> 📌 [Run on Google Colab](https://colab.research.google.com/drive/1PFolDMuYbIphIp-QxVX3oZ-huZG-6Za8)

---

## 📌 Project Overview

This Python-based solution reads a CSV of article URLs, scrapes their content, cleans the text, and performs a comprehensive textual analysis. The final results — including various sentiment scores and counts — are saved in an Excel file for reporting and further data analysis.

---

## 📚 Features & Approach

### 🔍 Web Scraping

- ✅ Scrapes article **titles** and **text bodies** from given URLs
- ✅ Uses `requests` and `BeautifulSoup` for HTML parsing
- ✅ Extracts clean, structured content ready for NLP

### 🧼 Text Cleaning

- ✅ Removes **stop words** from text (custom stop words list supported)
- ✅ Prepares text for tokenization and analysis

### 🧠 Textual Analysis

- ✅ **Word tokenization**
- ✅ **Frequency counts**
- ✅ **Polarity score** (positive vs negative word density)
- ✅ **Subjectivity score**
- ✅ Counts of:
  - Positive words
  - Negative words
  - Complex words
  - Average sentence length
  - Fog Index
  - Word Count
  - Sentence Count

### 📁 File Input & Output

- 🧾 Takes a CSV input file with article URLs
- 📂 Stores scraped articles as individual `.txt` files
- 📊 Outputs results into a formatted **Excel sheet**

---

## 🧠 Project Workflow

```plaintext
📥 Input CSV (URLs)
      ↓
🔍 Scrape article titles & text (requests + BeautifulSoup)
      ↓
🧽 Clean & preprocess text (remove stopwords, tokenize)
      ↓
📊 Perform NLP analysis (NLTK)
      ↓
📁 Save results as text + Excel
```

---

## 🧰 Dependencies & Setup

Ensure you have the following installed in your environment:

### ✅ Dependencies

- Python >= 3.6
- [pandas](https://pandas.pydata.org/)
- [requests](https://pypi.org/project/requests/)
- [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
- [nltk](https://www.nltk.org/)

## 💻 Installation

Install all required libraries using `pip`:

```bash
pip install pandas requests beautifulsoup4 nltk
```

---

## 🛠️ How to Run the Script

### 🖥️ On Local System

1. Make sure the following files are present in your working directory:
   - `input.csv` — contains the list of article URLs
   - `positive-words.txt` — list of positive words
   - `negative-words.txt` — list of negative words
   - `stopwords.txt` — list of stop words

2. Clone or download the repository:

```bash
git clone https://github.com/your-username/your-repo-name.git
cd your-repo-name
```

3. Run the Python script:

```bash
python script_name.py
```

4. Output files will be generated:
   - Scraped `.txt` files in the designated folder
   - Final analysis in `output.xlsx`

---

## 📊 Sample Output Columns

| URL | Title | Polarity Score | Subjectivity Score | Average Sentence Length | Fog Index | Word Count | Complex Word Count |
|-----|-------|----------------|--------------------|--------------------------|-----------|-------------|---------------------|
| ... | ...   | 0.25           | 0.67               | 12.3                     | 8.5       | 450         | 68                  |

---

## 🧪 Code Structure

```plaintext
📁 Project Root
├── script_name.py              # Main Python script
├── input.csv                   # Input URLs
├── stopwords.txt               # Stop words list
├── positive-words.txt          # Positive sentiment words
├── negative-words.txt          # Negative sentiment words
├── output/                     # Folder for scraped .txt articles
└── output.xlsx                 # Final analysis report
```

---

## 📈 Future Enhancements

- 🔄 Add support for additional sentiment lexicons (e.g., VADER, TextBlob)
- 🌐 Use newspaper3k or langchain for richer article parsing
- 📊 Generate visual dashboards (matplotlib/Plotly)
- ☁️ Automate in the cloud using Airflow or Lambda

---

## 🧾 License

This project is licensed under the **MIT License**.  
Feel free to modify and use it for your own educational or commercial purposes.

---

## 👤 Author

- **Ayush Anand**
- 📧 [0310ayushanand@gmail.com](mailto:0310ayushanand@gmail.com)
- 🔗 [GitHub: Ayush03A](https://github.com/Ayush03A)

---

⭐️ *Found this helpful? Give it a star and share it with your peers!*
