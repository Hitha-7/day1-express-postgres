# Day 1: Express + PostgreSQL CRUD API

## Overview
This project is a Node.js Express API connected to a PostgreSQL database.  
It supports full CRUD operations (Create, Read, Update, Delete) on an `items` table.

---

## Project Structure

day1-express-postgres/
├─ index.js
├─ db.js
├─ routes/items.js
├─ package.json
├─ README.md
├─ .gitignore
├─ .env.example


---

## Environment Variables

Create a `.env` file in the project root (do **not** push `.env` to GitHub).  
Use `.env.example` as a template:

PORT=3000
DB_USER=your_username
DB_PASSWORD=your_password
DB_HOST=localhost
DB_PORT=5432
DB_DATABASE=day1db


> **Note:** `.env` contains sensitive credentials and should **never** be pushed to GitHub. `.env.example` provides placeholders for setup.

---

## How to Run Locally

1. Clone the repository:
```bash
git clone https://github.com/Hitha-7/day1-express-postgres.git
npm run dev

| Method | Endpoint        | Description                        |
| ------ | --------------- | ---------------------------------- |
| GET    | /               | Check if server is running         |
| POST   | /api/items      | Create a new item (Body → JSON)    |
| GET    | /api/items      | Get all items                      |
| GET    | /api/items/\:id | Get a single item by ID            |
| PUT    | /api/items/\:id | Update an item by ID (Body → JSON) |
| DELETE | /api/items/\:id | Delete an item by ID               |

{
  "name": "Pen",
  "description": "Blue ink"
}

"C:\Users\Dell\OneDrive\Task1\screenshots.postman1.zip"  Screenshot File

POST /api/items → Creating a new item

GET /api/items → Fetching all items

GET /api/items/:id → Fetching a single item

PUT /api/items/:id → Updating an item

DELETE /api/items/:id → Deleting an item
