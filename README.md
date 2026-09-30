# Library Management System

A complete starter library management application built with:

- Node.js
- Express
- SQLite (`better-sqlite3`)
- HTML
- CSS
- Vanilla JavaScript

## Features

- Dashboard with library statistics
- Add, edit, delete and search books
- Add, edit, delete and search members
- Issue books to members
- Return books
- Automatic availability tracking
- Automatic overdue detection
- Automatic overdue fine calculation (₹5/day)
- Reports for popular books and overdue books
- Payment management with Cash, UPI, Card and Bank Transfer
- Payment history, receipt numbers, references and totals
- SQLite database created automatically
- Responsive interface for desktop and mobile

## Requirements

Install Node.js 18+.

## Run

Open a terminal inside this folder:

```bash
npm install
npm start
```

Then open:

http://localhost:3000

The SQLite database file `library.db` is created automatically the first time the application starts.

## Project structure

```text
LibraryManagementSystem/
├── database.js
├── server.js
├── package.json
├── README.md
└── public/
    ├── index.html
    ├── style.css
    └── app.js
```

## Main API

- `GET /api/dashboard`
- `GET/POST /api/books`
- `PUT/DELETE /api/books/:id`
- `GET/POST /api/members`
- `PUT/DELETE /api/members/:id`
- `GET /api/loans`
- `POST /api/loans/issue`
- `POST /api/loans/:id/return`
- `GET /api/payments`
- `POST /api/payments`
- `GET /api/payments/summary`
- `GET /api/reports`

## Production note

For a real college/enterprise deployment, add authentication and role-based access (admin/librarian/member), input validation, backups, audit logs, pagination, and a production database such as PostgreSQL/MySQL.
