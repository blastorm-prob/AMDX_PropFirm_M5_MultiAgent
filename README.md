# 🤖 AMDX PropFirm M5 Multi-Agent Trading System

[![License](https://img.shields.io/badge/license-MIT-blue.svg)](LICENSE)
[![Platform](https://img.shields.io/badge/platform-cTrader-green.svg)](https://ctrader.com)
[![Strategy](https://img.shields.io/badge/strategy-ICT%20Concepts-orange.svg)](https://github.com)

**3-Team Collaborative Trading Bot** for Prop Firm Approval + Retail Sales + Personal Profitability

---

## 📋 Project Overview

### Mission
- ✅ **Prop Firm Approval** (FTMO, MyForexFunds, etc.)
- ✅ **Retail Product Sales** (Proven, Documented Strategy)
- ✅ **Personal Trading Profits** (Live Account Trading)

### Team Structure
- **GPT**: Conservative Strategy (High Win Rate)
- **Copilot**: Balanced Strategy (Profitability + Stability)
- **Claude**: Aggressive Strategy (Maximum Profit)

### Core Concept
ICT (Inner Circle Trader) methodology with:
- External Liquidity Sweep
- Fair Value Gap (FVG)
- Order Block (OB)
- Market Structure Shift (MSS)
- Inducement Trigger

---

## 🎯 Trading Specifications

| Specification | Value |
|--------------|-------|
| **Symbol** | EURUSD |
| **Timeframe** | M5 (5-minute) |
| **Platform** | cTrader (cAlgo) |
| **Language** | C# |
| **Strategy Version** | v5.5 LS_SPLIT |
| **Parameter Split** | Long/Short Separated |

---

## 📊 Performance Targets

### GPT Conservative
```
Target Win Rate: 65%+
Target Profit Factor: 2.0+
Max Drawdown: <8%
Trades/Day: 0-3
Monthly Return: 5-8%
```

### Copilot Balanced
```
Target Win Rate: 55-60%
Target Profit Factor: 1.8+
Max Drawdown: <10%
Trades/Day: 2-5
Monthly Return: 8-12%
```

### Claude Aggressive
```
Target Win Rate: 50%+
Target Profit Factor: 1.5+
Max Drawdown: <12%
Trades/Day: 4-7
Monthly Return: 12-20%
```

---

## 🗂️ Repository Structure

```
AMDX_PropFirm_M5_MultiAgent/
├── README.md                          # This file
├── LICENSE                            # MIT License
├── .gitignore                         # Git ignore rules
│
├── code/
│   ├── ICT_AMDX_Propfirm_v5_5_LS_SPLIT.cs   # Main cBot code
│   └── CHANGELOG.md                   # Version history
│
├── parameters/
│   ├── GPT_CONSERVATIVE.json          # GPT parameter set
│   ├── COPILOT_BALANCED.json          # Copilot parameter set
│   ├── CLAUDE_AGGRESSIVE.json         # Claude parameter set
│   └── README.md                      # Parameter documentation
│
├── docs/
│   ├── 3TEAM_STRATEGY_PARAMETERS.md   # Complete strategy comparison
│   ├── BACKTEST_CHECKLIST.md          # Backtest execution guide
│   ├── GITHUB_vs_LOCAL.md             # Repository benefits
│   └── EURUSD_5M_Optimized_Parameters.md  # Initial optimization
│
├── results/
│   ├── backtests/
│   │   ├── GPT_Conservative_Results.md
│   │   ├── Copilot_Balanced_Results.md
│   │   └── Claude_Aggressive_Results.md
│   ├── forward-tests/
│   │   └── (Demo account results)
│   └── screenshots/
│       └── (Equity curves, trade distributions)
│
└── scripts/
    ├── install_guide.md               # cTrader installation
    └── parameter_import.md            # How to import parameters
```

---

## 🚀 Quick Start

### 1. Clone Repository
```bash
git clone https://github.com/blastorm-prob/AMDX_PropFirm_M5_MultiAgent.git
cd AMDX_PropFirm_M5_MultiAgent
```

### 2. Open in cTrader
```
1. Launch cTrader
2. Go to Automate → cBots
3. Click "New" → Copy code from /code/
4. Compile and run
```

### 3. Import Parameters
```
1. Open cBot settings
2. Load parameter file from /parameters/
3. Select strategy (GPT/Copilot/Claude)
4. Start backtesting
```

---

## 📈 Backtest Instructions

### Required Setup
```
Symbol: EURUSD
Timeframe: M5
Period: 2024-10-01 to 2024-12-15 (2.5 months)
Initial Capital: $10,000
Spread: 1.5 pips
Commission: $7 per lot round turn
Leverage: 1:100
```

### Running Backtests
See detailed instructions in: [docs/BACKTEST_CHECKLIST.md](docs/BACKTEST_CHECKLIST.md)

---

## 🔧 Parameter Comparison

| Parameter | GPT | Copilot | Claude |
|-----------|-----|---------|--------|
| **Risk/Trade** | 0.25% | 0.35% | 0.45% |
| **Max Trades/Day** | 3 | 5 | 7 |
| **Max DD Target** | 10% | 12% | 15% |
| **FVG Required** | Both | Optional | Optional |
| **Inducement** | Both Mandatory | Short Only | Optional |
| **BE/Trailing** | ❌ | ❌ | ✅ |
| **Stop Mode** | ObMean50 | ObMean50 | SweepExtreme |

Full comparison: [docs/3TEAM_STRATEGY_PARAMETERS.md](docs/3TEAM_STRATEGY_PARAMETERS.md)

---

## 📊 Backtest Results

### Status: 🔄 In Progress

| Version | Win Rate | Profit Factor | Max DD | Trades | Status |
|---------|----------|---------------|--------|--------|--------|
| GPT Conservative | TBD | TBD | TBD | TBD | ⏳ Pending |
| Copilot Balanced | TBD | TBD | TBD | TBD | ⏳ Pending |
| Claude Aggressive | TBD | TBD | TBD | TBD | ⏳ Pending |

Results will be updated in: [results/backtests/](results/backtests/)

---

## 🛡️ Risk Warnings

### Prop Firm Guards
- ✅ Max Equity Drawdown Cap (10-15%)
- ✅ Daily Loss Limit (4-8%)
- ✅ Consecutive Loss Pause (2-4 losses)
- ✅ Max Trades Per Day (3-7)
- ✅ Minimum Margin Level (400-600%)

### Important Notes
⚠️ **Past performance does not guarantee future results**  
⚠️ **Trading involves substantial risk of loss**  
⚠️ **Only trade with money you can afford to lose**  
⚠️ **Always test on demo before live trading**

---

## 📝 Development Roadmap

### Phase 1: Backtesting (Week 1-2)
- [x] Parameter sets finalized
- [ ] GPT Conservative backtest
- [ ] Copilot Balanced backtest
- [ ] Claude Aggressive backtest
- [ ] Results analysis and optimization

### Phase 2: Forward Testing (Week 3-4)
- [ ] Demo account setup (3 accounts)
- [ ] Real-time performance tracking
- [ ] Slippage and spread analysis
- [ ] Final parameter adjustment

### Phase 3: Prop Firm Challenge (Week 5+)
- [ ] Select best performing version
- [ ] FTMO/MFF challenge application
- [ ] Daily 0.5-1% profit target
- [ ] Max DD <5% maintenance

### Phase 4: Retail Sales (Month 2+)
- [ ] Complete documentation
- [ ] Video tutorials
- [ ] Sales page creation
- [ ] Customer support system

---

## 🤝 Contributing

### Team Members
- **GPT**: Conservative strategy development
- **Copilot**: Balanced strategy development
- **Claude**: Aggressive strategy development

### Collaboration Protocol
1. **Daily Check-in**: 22:00 KST (Progress updates)
2. **Weekly Meeting**: Sunday 20:00 KST (Results analysis)
3. **Emergency Contact**: Critical failures or major findings

### Pull Request Guidelines
1. Create feature branch from `main`
2. Test thoroughly on demo
3. Document all changes
4. Submit PR with detailed description
5. Wait for team review

---

## 📞 Contact & Support

### Issue Reporting
Use GitHub Issues for:
- 🐛 Bug reports
- 💡 Feature requests
- 📊 Backtest results
- ❓ Questions

### Response Time
- Critical issues: Within 24 hours
- Feature requests: Within 1 week
- Questions: Within 48 hours

---

## 📄 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## 🙏 Acknowledgments

- **ICT (Inner Circle Trader)** for methodology concepts
- **cTrader Platform** for excellent API
- **Prop Firm Community** for feedback and testing
- **3-Team Collaboration** for diverse perspectives

---

## 📊 Project Status

```
Created: 2025-12-15
Status: Active Development
Phase: Backtesting
Next Milestone: Complete all 3 backtests
Target Date: 2025-12-29
```

---

## 🔗 Quick Links

- [📖 Full Strategy Documentation](docs/3TEAM_STRATEGY_PARAMETERS.md)
- [✅ Backtest Checklist](docs/BACKTEST_CHECKLIST.md)
- [⚙️ Parameter Details](parameters/README.md)
- [📊 Latest Results](results/backtests/)
- [🤝 GitHub vs Local](docs/GITHUB_vs_LOCAL.md)

---

**⚡ Ready to Trade? Start with GPT Conservative for prop firm approval!**

**Last Updated**: 2025-12-15  
**Version**: 1.0.0  
**Repository**: blastorm-prob/AMDX_PropFirm_M5_MultiAgent
