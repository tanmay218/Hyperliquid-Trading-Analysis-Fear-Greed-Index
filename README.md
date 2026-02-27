# 📊 Hyperliquid Trading Analysis: Impact of Market Sentiment on Trader Behavior

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1TF36fYpvUbq3If1ONxQ1icg6HUecXuIJ)

## 📝 Project Overview

This project analyzes how market sentiment (Fear & Greed Index) relates to trader behavior and performance on the Hyperliquid exchange. The goal is to uncover patterns that could inform smarter trading strategies.

**🔗 Google Colab Link**: Click the badge above to access the complete code and analysis.

---

## 📁 Datasets Required

This repository contains two datasets that you need to upload to the Colab notebook:

### 1. Historical Trading Data (`historical_data.csv`)
Contains individual trade records from Hyperliquid exchange:

| Column | Description |
|--------|-------------|
| Account | Unique wallet address of the trader |
| Coin | Trading pair/symbol (@ for perpetuals) |
| Execution Price | Price at which trade was executed |
| Size Tokens | Quantity of tokens traded |
| Size USD | Notional value in USD |
| Side | BUY (long) or SELL (short) |
| Timestamp IST | Date and time in Indian Standard Time |
| Start Position | Position size before this trade |
| Direction | Overall position direction after trade |
| Closed PnL | Realized profit/loss from closed positions |
| Transaction Hash | Unique blockchain transaction ID |
| Order ID | Exchange order identifier |
| Crossed | TRUE = market order, FALSE = limit order |
| Fee | Trading fee paid in USD |
| Trade ID | Unique trade identifier |

### 2. Fear & Greed Index (`fear_greed_index.csv`)
Daily market sentiment data from alternative.me:

| Column | Description |
|--------|-------------|
| timestamp | Unix timestamp |
| value | Fear & Greed score (0-100) |
| classification | Sentiment category (Extreme Fear to Extreme Greed) |
| date | Human-readable date |

---

## 📥 How to Use This Repository

### Step 1: Download the Datasets
- Download both `historical_data.csv` and `fear_greed_index.csv` from this repository
- Save them to your local computer

### Step 2: Open the Colab Notebook
- Click the **"Open in Colab"** badge at the top of this README
- The notebook will open in Google Colab

### Step 3: Upload the Datasets to Colab
When you run the first code cell in the notebook, you will see a file upload prompt:

