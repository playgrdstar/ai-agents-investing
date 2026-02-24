# AI Agents for Investing

Code and notebooks for the book **AI Agents for Investing** by Gary Ang.

Four agent patterns. 30+ working notebooks. One portfolio assistant you can actually run.

---

## Get the Book

The full ebook (PDF) and a ZIP of all notebooks are free to download from my Substack:

👉 [simplyboring.ai](https://simplyboring.ai)

Link to article: Subscribe at the end of this [article](https://open.substack.com/pub/simplyboringai/p/a-free-180-page-ebook-on-ai-agents?utm_campaign=post-expanded-share&utm_medium=post%20viewer)


---

## What's in This Repo

### Agent Notebooks
The core of the book. Each maps to a pattern chapter.

| Notebook | Pattern | Chapter |
|---|---|---|
| `01_tool_calling.ipynb` | Tool Calling | Chapter 5 |
| `02_react_pattern.ipynb` | ReAct | Chapter 6 |
| `03_codeact_pattern.ipynb` | CodeAct | Chapter 7 |
| `04_orchestration.ipynb` | Orchestration | Chapter 8 |
| `05_portfolio_optimization.ipynb` | All four combined | Chapter 8 |

Two versions of each notebook are included:
- `simulated/` — uses simple simulated data, no API keys needed
- `api/` — uses live market data via APIs

### Finance Notebooks
The financial concepts your agents will use.

| Notebook | Topic |
|---|---|
| `01_stock_basics.ipynb` | Prices, OHLC, 52-week ranges, market cap, volume |
| `02_position_and_portfolio_value.ipynb` | Calculating what your holdings are worth |
| `03_portfolio_weights.ipynb` | Allocation and weight calculations |
| `04_returns_and_performance.ipynb` | Daily, cumulative, and annualized returns |
| `05_sharpe_ratio.ipynb` | Risk-adjusted return measurement |
| `06_maximum_drawdown.ipynb` | Worst peak-to-trough decline |
| `07_correlation_and_diversification.ipynb` | How assets move together |
| `08_sortino_ratio.ipynb` | Downside risk measurement |
| `09_sector_analysis.ipynb` | Sector exposure and concentration |
| `10_value_at_risk.ipynb` | Estimating potential losses |
| `11_portfolio_rebalancing.ipynb` | Maintaining target allocations |

### Setup Notebooks
Step-by-step setup for LLM providers and data APIs.

| Notebook | Provider |
|---|---|
| `01_setup_openai.ipynb` | OpenAI |
| `02_setup_anthropic.ipynb` | Anthropic |
| `03_setup_gemini.ipynb` | Google Gemini |
| `04_setup_huggingface.ipynb` | Hugging Face |
| `05_setup_openrouter.ipynb` | OpenRouter |
| `06_setup_alpha_vantage.ipynb` | Alpha Vantage |
| `07_setup_yfinance.ipynb` | yfinance |
| `08_setup_massive.ipynb` | Massive |
| `09_setup_fmp.ipynb` | Financial Modeling Prep |
| `10_setup_twelve_data.ipynb` | Twelve Data |
| `11_setup_eodhd.ipynb` | EODHD |

You only need one LLM provider and one data provider to start. The book uses OpenAI and yfinance by default.

### n8n Workflows
The same four patterns as visual workflows — no Python required.

| File | Pattern |
|---|---|
| `01 - Tool Calling.json` | Tool Calling |
| `02 - REACT.json` | ReAct |
| `03 - Agent + Code Tools.json` | CodeAct |
| `04 - Portfolio Optimization_Full Orchestration Agent.json` | Orchestration |

Import any `.json` file into n8n, add your API credentials, and you have a working agent workflow.

---

## Running the Notebooks

### Easiest: Google Colab (recommended for beginners)

1. Download the ZIP from the Substack article. Subscribe at the end of this [article](https://open.substack.com/pub/simplyboringai/p/a-free-180-page-ebook-on-ai-agents?utm_campaign=post-expanded-share&utm_medium=post%20viewer)
2. Upload the ZIP to your Google Drive
3. Right-click any `.ipynb` file → Open with → Google Colaboratory
4. Paste in your API key and run the cells

No local setup. No environment headaches.

### Alternative: Run locally
```bash
git clone https://github.com/[your-handle]/ai-agents-for-investing
cd ai-agents-for-investing
pip install -r requirements.txt
jupyter notebook
```

See `requirements.txt` for the full list of dependencies. You only need packages for the providers you plan to use — the core dependencies are `smolagents`, `litellm`, `pandas`, and `yfinance`.

---

## What You'll Need

- An LLM API key — OpenAI, Anthropic, or any provider via OpenRouter
- Optional: yfinance (free) or FMP API key for real market data
- Estimated API cost to work through the full book: $5–20

The `simulated/` notebooks work without any data API key.

---

## About the Author

Gary Ang. 

- Newsletter: [simplyboring.ai](https://simplyboring.ai)
- LinkedIn: [linkedin.com/in/garyang](https://linkedin.com/in/garyang)
- Email: gary@quaintitative.com

---

## License

Free to use for learning and personal projects. Please don't repackage and sell.