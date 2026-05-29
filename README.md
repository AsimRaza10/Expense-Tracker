# Expense Tracker

A full-stack web application for tracking personal income and expenses with charts, analytics, user authentication, and profile management.

## Features

- Register and log in with JWT-based authentication
- Add, edit, and delete expenses by category
- Track income sources
- View dashboard analytics and recent transactions
- Upload and manage a profile photo
- Export or work with spreadsheet-based financial data
- Use the app from desktop or mobile layouts

## Tech Stack

- Backend: Node.js, Express, MongoDB, Mongoose, JWT, Multer, Cloudinary
- Frontend: React, Vite, Recharts, Axios, Tailwind CSS
- Utilities: xlsx, file-saver, dayjs, moment

## Project Structure

```text
.
|-- Backend/
|   |-- config/
|   |-- controllers/
|   |-- middleware/
|   |-- models/
|   |-- routes/
|   |-- uploads/
|   `-- server.js
|-- Frontend/
|   `-- MySpend/
|       |-- src/
|       |-- package.json
|       `-- vite.config.js
|-- LICENSE
`-- README.md
```

## Getting Started

Clone the repository:

```bash
git clone https://github.com/AsimRaza10/Expense-Tracker.git
cd Expense-Tracker
```

Install backend dependencies:

```bash
cd Backend
npm install
```

Create `Backend/.env`:

```env
MONGODB_URI=your_mongodb_connection_string
JWT_SECRET=replace-with-a-secure-secret
PORT=5000
```

Start the backend:

```bash
npm run dev
```

Install frontend dependencies in another terminal:

```bash
cd Frontend/MySpend
npm install
```

Start the frontend:

```bash
npm run dev
```

Default local URLs:

- Frontend: `http://localhost:5173`
- Backend: `http://localhost:5000`

## API Overview

- `POST /api/auth/register` - register a user
- `POST /api/auth/login` - log in
- `GET /api/auth/profile` - fetch the current profile
- `GET /api/expenses` - list expenses
- `POST /api/expenses` - create an expense
- `PUT /api/expenses/:id` - update an expense
- `DELETE /api/expenses/:id` - delete an expense
- `GET /api/income` - list income records
- `POST /api/income` - create an income record
- `GET /api/dashboard/stats` - fetch dashboard stats

## License

This project is licensed under the MIT License. See [LICENSE](LICENSE) for details.
