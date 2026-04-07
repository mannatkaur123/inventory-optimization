# inventory-optimisation

Every retailer faces the same question: **how much stock should we hold?** Too much and you're paying to store inventory that isn't selling. Too little and customers can't buy what they want.

This project works through that problem end to end:

1. **Demand forecasting** — predict future sales using Moving Average and Exponential Smoothing
2. **Monte Carlo simulation** — quantify how uncertain those forecasts are across 10,000 demand scenarios
3. **Inventory optimization** — use Excel Solver to find the order quantity that minimizes total cost
4. **Scenario analysis** — compare 18 different inventory policies and rank them by annual cost

5. ## Forecasting models:
6. **Moving Average** — simple baseline. Predicts next period = average of last N periods.  
**Exponential Smoothing** — weighted average where recent data counts more (controlled by α).  
Both models are implemented in Excel (`Demand Forecasting` sheet) with an adjustable α parameter.
