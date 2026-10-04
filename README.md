# Electric Truck TCO & Fleet Economics Analysis

## Objective
Build a business case comparing diesel and battery-electric heavy freight truck economics using TCO, ₹/km, ₹/ton-km, payback, ROI proxy and fleet scenarios for 10, 100 and 1,000 trucks.

## Files
- `Electric_Truck_TCO_Fleet_Economics.xlsx` — interactive Excel model.
- `ev_tco_analysis.py` — Python model with charts and sensitivity analysis.
- `README.md` — project documentation.

## Key published references used
1. Tata Motors Prima E.55S: 450 kWh battery option and up to 350 km range.
2. Tata Motors Prima 5530.S: 55,000 kg diesel tractor specifications.
3. CSE policy brief: heavy-duty truck energy-consumption benchmarks.
4. APERC: FY2026-27 tariff order/press note.
5. IndianOil: official retail fuel-price page.
6. Dated Vijayawada diesel-price reference: ₹105.61/L on 3 Oct 2026.

## Important methodology note
The model deliberately separates published/reference values from scenario assumptions. EV purchase price, maintenance cost, payload, charging overhead, annual utilization and charging infrastructure cost are not treated as verified market facts. They are editable assumptions for a portfolio case study.

## Main calculations
- Diesel energy cost/km = diesel price / km per litre
- EV energy cost/km = electricity price × (battery kWh / advertised range) × (1 + charging overhead)
- Operating cost/km = energy + maintenance + other OPEX
- ₹/ton-km = operating cost/km / payload
- Simple payback = incremental EV investment / annual OPEX savings
- 5-year TCO = initial investment + 5-year OPEX − residual value
- ROI proxy = (5-year operating savings − incremental investment) / incremental investment

## How to use
1. Open the Excel file.
2. Edit the yellow cells in `Inputs`.
3. Review `Unit Economics`, `Fleet Scenarios` and `Sensitivity`.
4. Replace assumptions with company-specific or better-sourced values if you use this in an interview.
5. Run the Python script if Python, pandas and matplotlib are installed.

## Resume version
**Electric Truck TCO & Fleet Economics Analysis | Excel, Python**
- Built a comparative financial model to evaluate diesel vs. electric freight truck economics using TCO, ₹/km and ₹/ton-km.
- Estimated CAPEX, OPEX, annual savings and simple payback under multiple operating assumptions.
- Modeled fleet economics for 10, 100 and 1,000 trucks and performed electricity-price sensitivity analysis.
