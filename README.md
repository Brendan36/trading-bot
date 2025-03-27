# 📈 Automated Trading Bot (Python + Alpaca API)

This project is a Python-based automated trading bot developed for educational, experimental, and future deployment purposes. It supports:

- Historical data ingestion
- Strategy development (SMA, RSI, MACD, Smart Money Concepts, etc.)
- Pattern recognition and confluence logic
- Backtesting
- Live data streaming (coming soon)
- Trade execution + performance logging (in progress)

---

# Features

- **Data Sources:** Alpaca API for stocks/crypto
- **Visualization:** Matplotlib, Plotly
- **Strategies:** SMA Crossovers, RSI, Smart Money Concepts (SMC)
- **Architecture:** Modular files for ingestion, analysis, and trading
- **Logging:** Trade log + success/failure events

---

# Repo Structure

trading-bot/
│
├── README.md
├── requirements.txt
├── .gitignore
│
├── config/                      # API keys, constants (safely ignored)
│   └── config_template.py       # Sample config (exclude real keys)
│
├── data/
│   ├── raw/                     # Raw historical data
│   ├── processed/               # Cleaned and transformed data
│   └── logs/                    # Strategy logs, trade logs
│
├── notebooks/                   # Exploratory notebooks (e.g., backtests)
│   └── strategy_case_study.ipynb
│
├── strategies/                  # Trading strategies
│   ├── sma_rsi_strategy.py
│   ├── smc_confluence.py
│   └── utils.py
│
├── core/                        # Main bot logic
│   ├── data_ingestion.py
│   ├── live_stream.py
│   ├── trade_execution.py
│   └── performance_tracker.py
│
├── deployment/
│   ├── run_bot.py               # Launch script
│   └── package_instructions.md # EXE build or cloud deploy steps
│
└── tests/                       # Unit tests
    └── test_strategies.py
