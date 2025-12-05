**Delta-Neutral Strategy Backtesting**
Python simulation and performance analysis of a Delta-Neutral Yield Farming strategy combining Uniswap V3 liquidity provision with Aave short hedging.

**Project Overview**
This project demonstrates a quantitative approach to DeFi yield farming by neutralizing directional risk through hedging. The strategy aims to capture fee income from Uniswap V3 while protecting against Impermanent Loss using a short ETH position on Aave.​

**Strategy Components**
- Uniswap V3 LP Position: Concentrated liquidity in a specified price range (90%-110% of initial price)
- Aave Short Hedge: Borrow ETH to create a delta-neutral position
- Fee Accumulation: Simulate LP fee earnings (20% APR) over 30 days

**Why Simulated Data?**
This backtest uses synthetic price data (Random Walk) rather than real on-chain data for several strategic reasons:

*1. Independence from External APIs*
- No rate limits, API keys, or network dependencies
- Script runs offline and executes instantly
- Zero risk of API changes breaking the code

*2. Full Scenario Control*
- Test extreme market conditions (crashes, pumps and etc.)
- Adjust volatility parameters to stress-test the strategy

*3. Rapid Prototyping*
- Iterate on strategy logic without waiting for blockchain queries
