# Investment Calculator

A React and Vite web application for estimating investment growth over time. Enter an initial investment, recurring annual contribution, expected annual return, and investment duration to view yearly projections, summary totals, and a growth chart.

## Why use it?

- Quickly compare how contributions and expected returns affect projected growth.
- View yearly investment value, annual interest, cumulative interest, and invested capital.
- Highlight the year with the highest projected annual interest.
- Export the projection and chart as a PDF report.
- Use a lightweight front end with no server or account required.

## Getting started

### Prerequisites

- Node.js 18 or newer
- npm

### Install and run locally

From the repository root:

```bash
npm install
npm run dev
```

Open the local URL printed by Vite, usually `http://localhost:5173`.

### Use the calculator

1. Enter the beginning investment amount.
2. Enter the amount added each year.
3. Enter the expected annual return percentage.
4. Enter the number of years to invest.
5. Review the projection table and chart.
6. Select **Generate PDF Report** to download the current projection.

The calculator starts with these example values:

```text
Beginning investment: $4,000
Annual investment:    $1,200
Expected return:      6%
Duration:             35 years
```

> Projections are estimates based on the values entered. They are not financial advice or a guarantee of future returns.

## Development commands

```bash
npm run dev       # Start the Vite development server
npm run lint      # Run ESLint
npm run build     # Create a production build in dist/
npm run preview   # Preview the production build locally
```

## Project structure

```text
src/
├── components/           # Calculator inputs, results, header, and chart
├── util/investments.js   # Investment projection calculation and currency formatting
├── util/generatereport.js# PDF report generation
├── App.jsx               # Application state and component composition
└── main.jsx              # React entry point
```

The main calculation is available in `src/util/investments.js` as
`calculateInvestmentResults({ initialInvestment, annualInvestment, expectedReturn, duration })`.

## Help and documentation

For project questions or bug reports, [open an issue](https://github.com/VoidLance/course-files-javascript-react-investment-calc-project/issues).
For framework and library documentation, see:

- [React documentation](https://react.dev/)
- [Vite documentation](https://vite.dev/guide/)
- [Recharts documentation](https://recharts.org/)
- [jsPDF documentation](https://github.com/parallax/jsPDF)

## Contributing

Contributions are welcome. To propose a change:

1. Fork the repository and create a focused branch.
2. Install dependencies with `npm install`.
3. Make and test your changes with `npm run lint` and `npm run build`.
4. Open a pull request describing the change and how it was verified.

Please keep pull requests focused and avoid committing generated files such as
`dist/` or `node_modules/`.

## Maintainer

This project is maintained by [VoidLance](https://github.com/VoidLance).
