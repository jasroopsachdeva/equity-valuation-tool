# Equity Valuation and Financial Analysis Tool

A Python-based equity research web application that automates financial analysis for any NSE, BSE, or NYSE listed company. Built as a finance project by an engineering undergraduate to demonstrate applied financial modelling skills.

## Live Demo
[Click here to open the app](https://equity-valuation-tool-hgkxhm8chkcgvjqwmjbiiq.streamlit.app/)

## Features

- **Live financial data** — pulls real-time data via Yahoo Finance API
- **Financial ratio analysis** — P/E, EV/EBITDA, EBITDA margin, net margin, gross margin, ROE, debt/equity
- **DCF valuation** — 10-year free cash flow projection with interactive assumption sliders
- **Sensitivity analysis** — intrinsic value across WACC and terminal growth rate scenarios
- **Comparable company analysis** — enter any peer tickers, get side-by-side comps table with implied valuation
- **Excel report download** — formatted investment report with company overview, ratios, and DCF result

## How to Run Locally

**Step 1 — Clone the repository**
git clone https://github.com/jasroopsachdeva/equity-valuation-tool

**Step 2 — Install dependencies**
pip install -r requirements.txt

**Step 3 — Run the app**
streamlit run app.py

**Step 4 — Open in browser**
http://localhost:8501

## Example Analysis — Hindustan Unilever (HINDUNILVR.NS)

| Metric | Value |
|---|---|
| Current Price | ₹2,139 |
| DCF Intrinsic Value | ₹1,826 |
| Recommendation | HOLD |
| EV/EBITDA | 34.7x |
| EBITDA Margin | 22.6% |
| Return on Equity | 21.6% |

Peer comparison against Nestle India, Britannia, Dabur and Marico showed HUL trading at a discount to peer average EV/EBITDA of 39.5x — suggesting relative undervaluation on a comps basis despite the DCF HOLD signal.

## Tech Stack

| Tool | Purpose |
| Python | Core programming language |
| Streamlit | Web application framework |
| yfinance | Live financial data API |
| pandas | Data manipulation |
| openpyxl | Excel report generation |

## Project Structure

equity-valuation-tool/
├── app.py              # Streamlit web application
├── main.py             # Command line version
├── requirements.txt    # Python dependencies
└── README.md           # This file

## Finance Concepts Applied

- Discounted Cash Flow (DCF) valuation
- Terminal value using perpetuity growth method
- EV/EBITDA and P/E comparable company analysis
- Free cash flow calculation (EBIAT + D&A - Capex - Working Capital)
- WACC as discount rate
- Enterprise value to equity value bridge

## Author

Jasroop Singh Sachdeva
