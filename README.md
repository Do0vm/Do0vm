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

## ⚙️ Systems: C++ and Rust

### [orderbook-engine](https://github.com/Do0vm/orderbook-engine) · C++20
A limit order book matching engine like the one at the core of every exchange: price-time priority, limit/IOC/market orders, O(1) cancels.
- About **10 million orders/sec, ~100 ns median latency** on a GitHub Actions runner
- Differential-tested against a reference model on 200k random orders; CI on GCC, Clang, MSVC + ASan/UBSan

### [btc-options-greeks](https://github.com/Do0vm/btc-options-greeks) · Rust
Prices Deribit BTC options with Black-76: Greeks, implied-vol solver, volatility term structure and 25-delta skew.
- Matches **Deribit's own mark IV within 0.14 vol points** on all 477 out-of-the-money options in a real chain
- `erfc` written from scratch (Rust's std has none), bracketed Newton solver, clippy-clean

### [sha256-pow](https://github.com/Do0vm/sha256-pow) · C++20
SHA-256 from scratch, verified on NIST vectors and real Bitcoin blocks, plus a multithreaded midstate miner that **re-mines the genesis block** and finds Satoshi's nonce.

## 🧰 Toolbox

**Data & markets:** Python, pandas, NumPy, Excel, REST/JSON APIs, backtesting, order books, options pricing & implied volatility
**Engineering:** C++20, Rust, CMake, Git, GitHub Actions CI, unit and differential testing, sanitizers, JavaScript, PHP
**Security & integrity:** CompTIA Security+, SHA-256, audit trails, log analysis

## 🔭 Working on next
- Rolling walk-forward optimisation and volatility-targeted position sizing
- Order-book depth analysis on VALR via WebSocket

📫 Portfolio: [3d-web-portfolio-60.aura.build](https://3d-web-portfolio-60.aura.build)
