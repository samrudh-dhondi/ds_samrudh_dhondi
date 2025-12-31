# 📊 Trader Behavior vs Market Sentiment Analysis  
**Web3 Trading Team – Data Science Assignment**

**Candidate:** Samrudh Dhondi  

---

## 📌 Project Overview

This project analyzes how **real trader behavior** (profitability, risk, volume, and trade direction) aligns or diverges from **overall market sentiment** (Fear vs Greed) in the cryptocurrency market.

By combining:
- A **Bitcoin Fear & Greed Index** dataset, and  
- **Historical trade execution data** from Hyperliquid  

the analysis uncovers behavioral patterns that can inform **sentiment-aware and risk-efficient trading strategies**.

---

## 📊 Datasets Used

### 1️⃣ Bitcoin Market Sentiment (Fear & Greed Index)
- Columns:
  - `Date`
  - `Classification` (Fear / Greed)
- Purpose:
  - Represents daily aggregated market psychology

### 2️⃣ Historical Trader Data (Hyperliquid)
- Key columns:
  - Execution Price
  - Size Tokens
  - Size USD
  - Side (Buy/Sell)
  - Timestamp (IST)
  - Closed PnL
- Purpose:
  - Captures real trade execution behavior and outcomes

---

## 🔧 Data Processing & Methodology

### Data Cleaning
- Standardized timestamps and extracted trade dates
- Converted numeric columns safely
- Removed invalid or incomplete trade records

### Feature Engineering
- **Trade Volume:** USD exposure per trade  
- **Profitability Flag:** Profitable vs non-profitable trades  
- **Direction:** Long (Buy) vs Short (Sell)  
- **Risk-Adjusted Return:**  


> Note: Leverage data was not available in the dataset. USD exposure was used as a realistic proxy for risk.

---

## 📈 Key Analyses Performed

- Profitability comparison during Fear vs Greed
- Trading volume and participation patterns
- Long vs short directional bias
- Risk-adjusted performance across sentiment regimes

Visual outputs are saved in the `outputs/` directory.

---

## 🔍 Key Insights (Summary)

- Fear periods tend to produce **better risk-adjusted returns**
- Greed periods show **higher volume but lower efficiency**
- Trader behavior shifts significantly with sentiment, affecting:
- Position sizing
- Directional bias
- Profitability stability

---

## ▶️ How to Run the Project

1. Open `notebook_1.ipynb` in **Google Colab**
2. Ensure required Python libraries are available:
 - pandas
 - numpy
 - matplotlib
 - seaborn
3. Run all cells sequentially
4. CSV outputs and plots will be generated automatically

---

## 📄 Final Report

Detailed explanations, interpretations, limitations, and trading implications are documented in:

**`ds_report.pdf`**

---

## ⚠️ Note on Dataset Size

The full cleaned trade-level dataset exceeds GitHub’s file size upload limits.

A representative sampled dataset (`cleaned_trades_sample.csv`) has been included
for reference. All results, figures, and insights were generated using the full
dataset and can be fully reproduced by running the provided Google Colab notebook.

---

## ✅ Compliance Statement

- All analysis was performed in **Google Colab**
- Folder structure strictly follows assignment instructions
- Repository is intended for **evaluation and review purposes only**

---

## 📬 Contact

**Samrudh Dhondi**  
