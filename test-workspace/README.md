# EdgeLab Workspace

This workspace contains your trading strategies and analysis results.

## Folder Structure

- `strategies/` - Your trading strategy files
- `results/` - Analysis results (future feature)

## Example Strategies

### simple_rsi.py
Mean reversion strategy using RSI indicator.
- Buy when RSI < 30 (oversold)
- Sell when RSI > 70 (overbought)

### ema_crossover.py
Trend following strategy using EMA crossovers.
- Buy on golden cross (fast EMA crosses above slow EMA)
- Sell on death cross (fast EMA crosses below slow EMA)

## Running Analysis

```bash
# Analyze strategy on single symbol
edgelab analyze strategies/simple_rsi.py SPY 2023-01-01 2023-12-31

# Analyze on multiple symbols
edgelab analyze strategies/simple_rsi.py SPY,TSLA,NVDA 2023-01-01 2023-12-31

# With ML optimization
edgelab analyze --ml strategies/simple_rsi.py SPY,QQQ 2023-01-01 2023-12-31
```

## Next Steps

1. Review example strategies
2. Modify parameters or create your own strategy
3. Run analysis with `edgelab analyze`
4. View results with `edgelab results list`

## Documentation

- Full docs: https://docs.edgelab.com
- API reference: https://docs.edgelab.com/api
- Strategy examples: https://docs.edgelab.com/strategies
