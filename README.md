# 📊 Hyperliquid Trading Analysis: Impact of Market Sentiment on Trader Behavior

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TF36fYpvUbq3If1ONxQ1icg6HUecXuIJ)

## 📝 Project Overview

This project analyzes how market sentiment (Fear & Greed Index) relates to trader behavior and performance on the Hyperliquid exchange. The goal is to uncover patterns that could inform smarter trading strategies.

**🔗 Google Colab Link**: Click the badge above to access the complete code and analysis.

---

## 📁 Datasets Required

Due to file size limitations (>25MB), the datasets are hosted on Google Drive. You need to download both files before running the Colab notebook.

---

### 📌 Dataset 1: Bitcoin Market Sentiment (Fear & Greed Index)

| Detail | Information |
|--------|-------------|
| **Description** | Daily market sentiment data showing whether the market was in Fear, Neutral, or Greed mode |
| **File Name** | `fear_greed_index.csv` |
| **Columns** | Date, Classification (Fear/Greed/Neutral), Value |
| **Download Link** | [⬇️ Click here to download Fear & Greed Dataset](https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing) |

**Instructions for downloading:**
1. Click the link above
2. Look for the **download symbol** (⬇️) in the **top-left corner** of the Google Drive page
3. Click the download symbol to save the file to your computer

**Direct Link:** `https://drive.google.com/file/d/1PgQC0tO8XN-wqkNyghWc_-mnrYv_nhSf/view?usp=sharing`

---

### 📌 Dataset 2: Historical Trader Data (Hyperliquid)

| Detail | Information |
|--------|-------------|
| **Description** | Complete trading history from Hyperliquid exchange with individual trade records |
| **File Name** | `historical_data.csv` |
| **Columns** | account, symbol, execution price, size, side, time, start position, event, closedPnL, leverage, and more |
| **Download Link** | [⬇️ Click here to download Hyperliquid Trading Dataset](https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing) |

**Instructions for downloading:**
1. Click the link above
2. Look for the **download symbol** (⬇️) in the **top-left corner** of the Google Drive page
3. Click the download symbol to save the file to your computer

**Direct Link:** `https://drive.google.com/file/d/1IAfLZwu6rJzyWKgBToqwSmmVYU6VbjVs/view?usp=sharing`

---

## 📥 How to Use This Repository

### Step 1: Download Both Datasets
- Download **both CSV files** from the Google Drive links above
- Save them to your local computer (remember where you saved them!)

### Step 2: Open the Colab Notebook
- Click the **"Open in Colab"** badge at the top of this README
- The notebook will open in Google Colab

### Step 3: Upload the Datasets to Colab
When you run the first code cell in the notebook, you will see a file upload prompt:

```python
# This cell will prompt you to upload files
from google.colab import files
print("Please upload BOTH CSV files when prompted")
uploaded = files.upload()
