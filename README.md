# 📈 Multi-Agent Financial Analysis & Reporting System

A sophisticated multi-agent framework designed to automate financial research, sentiment analysis, and automated report generation. By leveraging **LangChain** and **Google Gemini 1.5 Flash**, this system orchestrates specialized agents to perform deep-dive market analysis.

## 🚀 Overview
Unlike standard RAG, this system uses a **Multi-Agent Orchestration** approach:
- **Researcher Agent**: Fetches real-time market data and news via APIs (yfinance, NewsAPI).
- **Analyst Agent**: Performs sentiment analysis on financial news and technical analysis on price trends.
- **Writer Agent**: Synthesizes findings into a professional, structured financial report.

## 🛠️ Tech Stack
- **LLM:** Google Gemini 1.5 Flash (via `langchain-google-genai`)
- **Framework:** LangChain (LCEL) / LangGraph (Planned)
- **Data Sources:** Yahoo Finance (`yfinance`), Mediastack/Finnhub API
- **NLP:** FinBERT (for specialized financial sentiment)
- **Environment:** Python 3.12 (macOS)

## 📁 Project Structure
```text
.
├── src/
│   ├── agents/            # Agent logic and prompt definitions
│   ├── tools/             # API wrappers for financial data
│   └── output/            # Generated PDF/Markdown reports
├── data_prepare.py        # Data cleaning and factor engineering
├── Agent_Financial.ipynb  # Core orchestration & execution
├── .env                   # API Keys (SECURE - Not tracked)
└── requirements.txt       # Environment dependencies 
