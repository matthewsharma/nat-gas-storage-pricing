# nat-gas-storage-pricing

This project analyzes and plots data of natural gas storage prices and then extrapolates it for an extra year. The data is from the J.P. Morgan Quantitative Research Forage task.

The notebook "nat_gas_pricing.ipynb" :

Task 1:
- Loads monthly natural gas prices from "Nat_Gas.csv".
- Visualizes historical prices and interpolates to a daily time series.
- Computes seasonal average prices by calendar month.
- Extrapolates prices one year into the future using those seasonal averages.
- Defines "estimate_nat_gas_price(date_str)" to return a price for any date in the supported range.

Task 2:
- Uses a price curve to value simple gas storage contracts
- Models day by day inventory and cash flows
- Main function respects and includes:
    - Injection and withdrawal dates
    - Maximum daily injection/withdrawal rates
    - Maximum storage capacity
    - Per-unit storage cost per day
    - Per-unit injection and withdrawal fees
    - Peroperation transport fees
