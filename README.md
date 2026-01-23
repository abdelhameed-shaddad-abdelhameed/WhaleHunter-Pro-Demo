# 🐋 WhaleHunter Pro - Live Market Intelligence

**WhaleHunter Pro** is a powerful, real-time blockchain monitoring dashboard built with Python and Streamlit. It tracks "Whale" wallets across multiple chains (Ethereum, BSC, Polygon) and sends instant alerts when large movements occur.

![System Status](https://img.shields.io/badge/System-Online-brightgreen)
![Python](https://img.shields.io/badge/Python-3.9%2B-blue)
![Streamlit](https://img.shields.io/badge/Streamlit-1.50-FF4B4B)
![License](https://img.shields.io/badge/License-MIT-green)

## ✨ Key Features

* **Multi-Chain Tracking:** Monitor wallets on Ethereum, BSC, and Polygon simultaneously.
* **Real-Time Alerts:** Integration with Telegram, Discord, Slack, and Email.
* **Visual Analytics:** Interactive charts for ETH holdings and Stablecoin (USDT/USDC/DAI) movements.
* **Secure Architecture:** Uses Streamlit Secrets management and Environment variables protection.
* **Resilient Engine:** Auto-retry logic with exponential backoff for RPC connection stability.
* **Persistent Data:** SQLite database to store wallet history and transaction logs.

## 🐉 DragonHunter X (HFT-grade Solana bot engine)

The repository now ships **DragonHunter X**, a Solana-first, asyncio-driven execution stack optimized for ultra-low-latency pool sniping and resilient trade execution.

### Key Pillars
- **Pydantic config** (`config/settings.py`) that fails fast when env vars are missing.
- **Resilient RPC** (`core/rpc_client.py`) with exponential backoff.
- **Circuit breaker + graceful shutdowns** (`core/engine.py`) to halt safely on error spikes.
- **Event-driven sniping** (`modules/sniper.py`) using `asyncio.Queue`.
- **Execution abstraction with Jito bundle hook** (`modules/execution.py`).
- **Rich-powered logging** (`utils/logger.py`) for structured observability.

### Quickstart
1. Export required env vars (see `config/settings.py`).
2. Install deps: `pip install -r requirements.txt`
3. Run: `python main.py`


