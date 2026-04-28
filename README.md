<div align="center">

Topics: trading-bot, mt5-script, instant-mt-close, indicators, expert-advisors, metatrader5, mql-all-close, dual-mt5-close, mql5, quick-mt5-exit, forex-trading, mt5-stop-all, mt5-close-utility, order-management, order-close, risk-management, expert-advisor


# Information

**Advanced MT5 / MT4 forex trading tool and indicator suite designed for modern trading platforms, featuring automation, risk management, trade execution, market analysis, and algorithmic trading capabilities. This project supports traders with expert advisors (EAs), indicators, scalping systems, position sizing tools, and real-time trading assistance.**

# ⚡ MT5 Auto Scripts

**A professional desktop tool for executing MT5 trading scripts instantly built for traders who can't afford to be slow.**

<br>

[![Stars](https://img.shields.io/github/stars/torvalds/linux?style=for-the-badge&color=FFD700&label=Stars)](https://github.com/your-username/mt5-auto-scripts/stargazers)
[![Forks](https://img.shields.io/github/forks/torvalds/linux?style=for-the-badge&color=3F51B5&label=Forks)](https://github.com/your-username/mt5-auto-scripts/network)
[![Issues](https://img.shields.io/github/issues/torvalds/linux?style=for-the-badge&color=E53935&label=Issues)](https://github.com/your-username/mt5-auto-scripts/issues)
[![License](https://img.shields.io/badge/License-MIT-2EA043?style=for-the-badge)](LICENSE)
[![Platform](https://img.shields.io/badge/Platform-MetaTrader%205-1565C0?style=for-the-badge)](https://www.metatrader5.com)

</div>

---

## 🚨 The Problem Every Trader Knows

> *"Market is crashing. You need to close everything. Now."*
>
> You open MT5 — close position 1, close position 2, cancel order 1, cancel order 2...
>
> **By the time you're done, the damage is done.**

MT5 Auto Scripts gives you a single button to close every open position and cancel every pending order across your entire account instantly, with a clean confirmation flow and real-time feedback.

---

## Screenshot

<div align="center">

<p align="center">
  <img src="https://i.ibb.co/PBzS1Lc/close.png" alt="photo" width="820">
</p>

</div>

---

## 🎬 Demo

<div align="center">

<img src="https://i.imgur.com/XWmOYAm.gif" alt="Demo">

</div>

---

## What It Does

**Close All Orders Script** connects to your active MT5 session and performs the following in sequence:

1. Reads all open market positions from the account
2. Sends a close request for each position at the current market price
3. Reads all pending orders (limit, stop, stop-limit)
4. Cancels every pending order individually
5. Verifies each closure and reports the final result

The entire process takes a few seconds and gives you step-by-step progress feedback throughout.

---

## Features

| Feature | Description |
|---|---|
| Close All Positions | Closes every open market position regardless of symbol, direction, or volume |
| Cancel All Pending Orders | Removes all limit, stop, and stop-limit orders from the account |
| Multi-Symbol Support | Works across forex pairs, metals, indices, crypto — any instrument on your MT5 broker |
| Pre-Execution Preview | Before running, the app shows a full table of every position and order that will be affected |
| Confirmation Requirement | The Run button stays disabled until you explicitly check the confirmation box — no accidents |
| Live Connection Status | Sidebar shows your MT5 server name, login ID, and live connection state at all times |
| Animated Progress Bar | Each step of the script is shown in real time: connect → close positions → cancel orders → verify → done |
| Disconnect / Reconnect | Toggle your MT5 connection directly from the sidebar without restarting the app |
| Real-Time Status Bar | Bottom bar shows the current operation and a live clock |

---

## 🛡️ Safety Design

This tool handles irreversible trading actions, so it was designed with several layers of protection:

- **Confirmation gate** — the Run button is visually disabled and non-clickable until the user ticks the acknowledgement checkbox
- **Order preview** — a full grid of all open positions and pending orders is displayed before any action is taken, so you always know exactly what will be closed
- **Connection check** — if MT5 is disconnected, the script refuses to run and shows a warning in the status bar
- **Warning banner** — a clearly visible red warning reminds the user that the action cannot be undone
- **No auto-run** — the script never runs automatically; every execution requires a manual trigger

---

## Quick Start

**Requirements:**
- Windows 10 or 11
- [.NET 6 or higher](https://dotnet.microsoft.com/en-us/download)
- MetaTrader 5 terminal installed and logged in
- Visual Studio 2022 (to build from source)

**Steps:**

```bash
# Clone the repository
git clone https://github.com/your-username/mt5-auto-scripts.git

# Open the solution in Visual Studio 2022
# File → Open → WinFormsApp1.sln

# Build and run — press F5
```

> No external NuGet packages required. The project builds and runs out of the box on any Windows machine with .NET 6+.

---

## How to Use

1. Launch the application
2. Check the sidebar — confirm MT5 shows **Connected** with your server and login details
3. Review the **Open Positions** and **Pending Orders** tables in the Preview section
4. Read the warning, then tick the confirmation checkbox
5. Click **Run Script**
6. Watch the progress bar — the status bar will update at each step
7. When complete, all positions will show **Closed** and all pending orders will show **Cancelled**

---

## Roadmap

- [x] Close All Orders Script
- [ ] Close by Symbol — close only positions on a specific instrument (e.g. XAUUSD only)
- [ ] Close by Direction — close only Buy positions, or only Sell positions
- [ ] Close by Loss — automatically close any position in drawdown beyond a set threshold
- [ ] Scheduled Execution — trigger a close script at a specific time
- [ ] Telegram Notification — send a message to your Telegram after execution completes

> Have a script idea? [Open an issue](https://github.com/your-username/mt5-auto-scripts/issues) and describe what you need.

---

## Contributing

Pull requests are welcome. For significant changes, please open an issue first to discuss the approach.

```
1. Fork the repository
2. Create a feature branch:  git checkout -b feature/close-by-symbol
3. Commit your changes:      git commit -m "Add: close by symbol script"
4. Push to your fork:        git push origin feature/close-by-symbol
5. Open a Pull Request
```

---

## ⭐ Support

If this saved you from a bad trade, consider leaving a star — it helps other traders find this tool.

<div align="center">

[![Star this repo](https://img.shields.io/badge/Star%20this%20repo-FFD700?style=for-the-badge)](https://github.com/your-username/mt5-auto-scripts)

</div>

---

<div align="center">

**MT5 Auto Scripts** &nbsp;·&nbsp; Built for traders, by traders &nbsp;·&nbsp; v1.0.0

</div>
