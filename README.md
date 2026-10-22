# ATELIER VÉRA — E-Commerce Clothing Website (HTML, CSS, JS + MySQL)

A responsive online clothing store where customers browse product listings, filter by category/size/price, inspect garments, manage their shopping bag, and place orders backed by a relational MySQL database.

## Project Structure for VS Code

```text
atelier-vera-ecommerce/
├── index.html              # Responsive SPA Storefront (Home, Shop, Lookbook, MySQL Console)
├── css/
│   └── styles.css          # Editorial stylesheet, custom variables & responsive layouts
├── js/
│   └── app.js              # Storefront state, filtering, cart drawer, checkout & SQL engine
├── backend/
│   ├── schema.sql          # MySQL 8.0 DDL schema (6 tables) + seed catalog data
│   └── server.js           # Node.js + Express + mysql2 REST API server
└── package.json            # Dependencies for running the MySQL backend
```

## Quick Start in VS Code

### Option A: Instant Frontend Preview (VS Code Live Server)
1. Open the `atelier-vera-ecommerce` folder in **VS Code**.
2. Install the **Live Server** extension (`ritwickdey.LiveServer`).
3. Right-click `index.html` and select **"Open with Live Server"**.
4. The storefront automatically uses its built-in **MySQL In-Memory Relational Engine** when running statically, logging every generated `SELECT` and `INSERT` query in real time!

### Option B: Full-Stack Mode with Local MySQL 8.0 Server
1. Import the database schema into MySQL:
   ```bash
   mysql -u root -p < backend/schema.sql
   ```
2. Install Node dependencies and start the Express server:
   ```bash
   npm install
   npm start
   ```
3. Open `http://localhost:3000` in your browser.
