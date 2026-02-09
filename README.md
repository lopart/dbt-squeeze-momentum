# 📈 dbt Squeeze Momentum Strategy

**Squeeze Momentum technical analysis strategy** entirely in **dbt**:

- Feature engineering with dbt models
- Custom dbt macros for technical indicators
- Signal generation (squeeze on / squeeze off / momentum)
- Historical backtesting using SQL
- Reproducible, warehouse-native analytics

The goal is to show how **quantitative trading logic** can be expressed, tested, and versioned using analytics engineering best practices.

---

## Squeeze Momentum?

The **Squeeze Momentum Indicator** is a technical analysis indicator that identifies periods when:

- **Bollinger Bands** are inside **Keltner Channels** is reflected as  *low volatility (squeeze on)*
- A momentum oscillator signals directional bias

Once squeeze releases, momentum often sharply.

This repo implements time-series of:
- Bollinger Bands
- Keltner Channels
- Squeeze state detection
- Momentum calculation
- Entry / exit rules

All using SQL with dbt macros for logging.
