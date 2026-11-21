# Colby's Investment Chief of Staff

Single-file, view-only dashboard (`index.html`) Colby opens before the market.

- **Schwab data:** drop the Positions export and the Transactions export (Jan 1 to today) onto the page. Files are parsed in the browser and kept only in that browser's local storage. Nothing is uploaded.
- **Reconciliation:** the page checks positions + cash against Schwab's Account Total, matches every sale to a purchase (FIFO), and compares share counts rebuilt from transactions against positions.
- **Return:** enter the Jan 1 account value (December statement ending balance). Return uses modified Dietz, so deposits and withdrawals don't count as gains.
- **Still example content:** morning brief, Gmail, and the earnings/economic calendar.
- `test-data/` holds mock exports in Schwab's CSV layout for testing.

Next: Schwab Trader API sync (read-only), brief feed, Gmail (read-only), Google Calendar for travel.
