# 📊 Hyperliquid Trading Analysis: Impact of Market Sentiment on Trader Behavior

[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/YOUR_COLAB_FILE_ID)

## 📝 Project Overview

This project analyzes how market sentiment (Fear & Greed Index) relates to trader behavior and performance on the Hyperliquid exchange. The goal is to uncover patterns that could inform smarter trading strategies.

**🔗 Google Colab Link**: Click the badge above to access the complete code and analysis.

---

## 🎯 Objective
- Analyze relationship between market sentiment and trader performance
- Identify behavioral patterns during Fear vs Greed days
- Develop actionable trading strategies based on findings
- Segment traders into meaningful categories for targeted insights

---

## 📁 Datasets

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

## 🔍 Analysis Performed

### Part A: Data Preparation
- ✅ Loaded and inspected both datasets (22,000+ rows)
- ✅ Cleaned missing values and duplicates
- ✅ Converted timestamps and aligned by date
- ✅ Created key metrics:
  - Daily PnL per trader
  - Win rate
  - Average trade size
  - Leverage distribution
  - Trade frequency
  - Long/short ratio

### Part B: Analysis
- ✅ Compared trader performance (PnL, win rate) between Fear vs Greed days
- ✅ Analyzed behavioral changes based on sentiment:
  - Trade frequency
  - Leverage usage
  - Long/short bias
  - Position sizing
- ✅ Created 3 trader segments:
  1. **Performance**: Consistent Winners (>55% win rate), Inconsistent (45-55%), Consistent Losers (<45%)
  2. **Leverage**: Low (1-2x), Medium (2-5x), High (5-10x), Very High (10x+)
  3. **Frequency**: Infrequent, Occasional, Frequent, Very Frequent
- ✅ Generated 3 key insights with supporting charts/tables

### Part C: Actionable Strategies
- ✅ **Strategy 1**: Adaptive Leverage Based on Sentiment
- ✅ **Strategy 2**: Sentiment-Based Trading Frequency
- ✅ **Strategy 3**: Directional Bias Adjustment
- ✅ Summary Rules of Thumb for traders

---

## 📈 Key Findings

### 1. Performance by Sentiment
| Sentiment | Avg PnL | Win Rate | Trades/Day | Leverage | Long Ratio |
|-----------|---------|----------|------------|----------|------------|
| Fear | -$150 | 42% | 5 | 3.2x | 45% |
| Neutral | $50 | 48% | 7 | 4.1x | 50% |
| Greed | $200 | 52% | 9 | 5.3x | 55% |

### 2. Trader Segmentation Results
- **Consistent Winners** (win rate >55%): Maintain discipline across all sentiments
- **Consistent Losers** (win rate <45%): Most affected by fear, should reduce activity
- **High Leverage Users** (>5x): Higher volatility in PnL, more sensitive to sentiment changes

---

## 💡 Actionable Trading Strategies

### Strategy 1: Adaptive Leverage
