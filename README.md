# FinCast

FinCast is a browser-based sector growth forecasting tool. It creates transparent five-year revenue, EBITDA, and net income forecasts using historical company data, sector-specific drivers, and Bear, Base, and Bull scenarios.

## Features

- Supports Utilities, Consumer Staples, and Pharmaceuticals
- Calculates historical revenue, EBITDA, and net income CAGRs
- Uses driver-based formulas for each supported sector
- Flags assumptions outside typical benchmark ranges
- Compares Bear, Base, and Bull scenarios
- Displays forecast KPIs, charts, assumptions, and an explanation of the calculation
- Runs entirely in the browser with no backend or build process

## Run Locally

1. Open `index.html` in a modern web browser.
2. For the best experience, serve the folder with a local web server, for example:

   ```powershell
   python -m http.server 8000
   ```

3. Visit `http://localhost:8000`.

The page loads Chart.js and Google Fonts from CDNs, so an internet connection is required for the chart and custom fonts.

## How to Use

1. Enter a company name, currency, scale, sector, and at least two years of revenue data.
2. Review the historical CAGRs and the sector growth formula.
3. Adjust the sector assumptions and review benchmark warnings.
4. Build Bear, Base, and Bull scenarios.
5. Review the five-year forecast, chart, KPI cards, and narrative summary.

## Sector Models

- **Utilities:** Customer Count x Consumption per Customer x Rate per Unit
- **Consumer Staples:** Store Count + Same-Store Sales + New-Store Contribution
- **Pharmaceuticals:** Prescription Volume x Price per Prescription - Patent Cliff Erosion

Technology, commodity, biotech, and real estate selections are intentionally excluded because their results are less suitable for this simplified CAGR-based model.

## Disclaimer

FinCast is an educational forecasting aid. Its outputs depend on user-provided data and assumptions and should not be treated as financial, investment, or professional advice.