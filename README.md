# Hi, I'm Gregory 👋

**Python developer and data analyst focused on crypto markets**, based in Johannesburg, South Africa.

I spent six years building **RAPTOR**, a real-time operations platform for private-security drone teams: live telemetry and video, incident alerts, SHA-256 evidence integrity and audit trails. Now I apply the same habits to market data: validate everything, log everything, and don't trust a result until it survives data it hasn't seen.

## 📈 Featured projects

### [crypto-backtest-lab](https://github.com/Do0vm/crypto-backtest-lab)
Do simple trading rules beat holding crypto once you pay fees? SMA crossover, momentum and RSI mean reversion on daily BTC, ETH and SOL, **with parameters fitted on 2018–2022 and tested on unseen 2023–2026 data**.
- No-look-ahead execution, proven by a unit test; fees and slippage on every trade
- Finding: in-sample Sharpe ratios as high as 1.97 fell to 0.33–1.05 out-of-sample, and only 2 of 9 strategies beat buy-and-hold, but trend filters cut BTC's max drawdown from -53% to -32%

`Python` `pandas` `NumPy` `matplotlib`

### [zar-crypto-spreads](https://github.com/Do0vm/zar-crypto-spreads)
Live BTC and ETH spreads between South Africa's two biggest rand exchanges (VALR and Luno), fee-adjusted, plus the **ZAR premium** over the global Binance price.
- Exchange adapters behind one common quote model, with sanity checks and a CSV logger that survives network failures
- Finding: no positive fee-adjusted gap in any sample; VALR's BTC book was about 7x tighter than Luno's

`Python` `REST APIs` `zero dependencies`

## 🧰 Toolbox

**Data & markets:** Python, pandas, NumPy, Excel, REST/JSON APIs, descriptive statistics, backtesting, order books & spreads
**Engineering:** Git, unit testing, CLI tools, JavaScript, PHP, C/C++ (see my raytracer projects)
**Security & integrity:** CompTIA Security+, SHA-256, audit trails, log analysis

## 🔭 Working on next
- Rolling walk-forward optimisation and volatility-targeted position sizing
- Order-book depth analysis on VALR via WebSocket

📫 Portfolio: [3d-web-portfolio-60.aura.build](https://3d-web-portfolio-60.aura.build)
