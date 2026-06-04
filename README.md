# Personal Expense Ledger

A local personal expense ledger with Express, built-in SQLite, CSV export, and a small web UI.

## Features

- Add expenses with title, amount, category, date, and note.
- Store data locally in SQLite.
- Filter by month and category.
- View total spending and entry count.
- Delete entries.
- Export filtered data as CSV.

## Tech Stack

- Node.js 24
- Express
- Built-in `node:sqlite`
- HTML, CSS, JavaScript

## Getting Started

```bash
npm install
npm run dev
```

Open:

```txt
http://127.0.0.1:8001
```

## Production Run

```bash
npm install --omit=dev
npm start
```

## Data Storage

The SQLite database is created at:

```txt
data/expenses.sqlite
```

The `data` directory is ignored by Git so personal expenses are not committed.

## API

```txt
GET    /api/expenses
POST   /api/expenses
DELETE /api/expenses/:id
GET    /api/summary
GET    /api/export.csv
```

## License

MIT
