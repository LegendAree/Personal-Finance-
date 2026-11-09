# Personal Finance — PWA

A private, offline-capable personal finance planner designed for iPhone and GitHub Pages. No account, backend, analytics, or third-party libraries are required.

## Features
- Dashboard with monthly metrics, savings chart, category breakdown and quick actions.
- Month-specific salary settings and payslip calculation.
- Leave planner that counts actual Thursdays, Fridays, Saturdays and Sundays in each month, excluding leave dates.
- USD and MVR expense entries, with a monthly editable exchange rate.
- Other income tracking for side jobs, freelance work, gifts and any income outside salary.
- Savings allocation by month and purpose (for example Holiday, Medical or Emergency), with an independently editable USD/MVR currency for every allocation.
- Dedicated debts and loans tracker for money you owe and money other people owe you, including payment records and outstanding balances.
- Annual report and CSV export.
- JSON backup and restore.
- Local browser storage and offline PWA cache.

## Savings and allocations
Monthly savings are calculated as net salary + other income − expenses. MVR amounts are converted using the selected month's exchange rate (or the actual USD exchange amount entered for MVR expenses). Savings allocations are labels showing how you intend to divide that month's surplus; they do not subtract the allocation a second time from your savings balance.

## Salary calculation
Gross = base salary + (daily allowance × paid working days) + telephone allowance.
Net = gross − (base salary × pension percentage) − social fund.

## Debts & loans
- **I borrowed (I owe):** money you need to repay to another person or lender.
- **Someone borrowed from me (they owe me):** money another person needs to repay to you.
- Add the original amount, currency, person, date, optional due date and notes.
- Use **Record payment** to add repayments or collections and update the outstanding balance.

## Publish free with GitHub Pages
1. Create a GitHub repository (for example, `personal-finance`).
2. Upload **all files inside this folder** to the repository root: `index.html`, `styles.css`, `app.js`, `manifest.webmanifest`, `sw.js`, `icon.svg`, and `README.md`.
3. Open repository **Settings → Pages**.
4. Under **Build and deployment**, select **Deploy from a branch**; choose `main` and `/ (root)`, then Save.
5. Wait for GitHub Pages to publish. Your app address will look like `https://YOUR-USERNAME.github.io/personal-finance/`.

## Install on iPhone
1. Open the published address in Safari.
2. Tap Share → Add to Home Screen.
3. Enable “Open as Web App” if shown, then tap Add.

## Data and backups
- Finance records are stored in this browser's local storage on the device. They are not uploaded to GitHub.
- Existing Ameer Finance browser records are retained because the app keeps the original local-storage keys.
- Export a JSON backup regularly, especially before clearing Safari website data, changing browsers, or changing phones.
- To move records to another device, export the backup on the old device and import it on the new device.
- A public repository makes the source code visible; never put personal finance records or backup files in the repository.
- This is a budgeting tool, not a payroll system. Confirm payslips against your employer's actual payroll calculation.
