# Employee Salary Analysis and Table Webpage

## Overview

This is a **full-stack application** for managing and analyzing employee salaries. The application allows users to view, add, edit, and analyze employee data stored in a **MySQL database**. The front-end is built using **React**, while the back-end is powered by **Node.js**. The database runs on **XAMPP**.

---

## Features

- **Employee Management**: Add, update, and delete employee records.
- **Salary Analysis**: Generate reports and visualize salary data.
- **Dynamic Table**: Display employee data in a user-friendly, sortable, and searchable table.
- **Secure Backend**: API endpoints for CRUD operations with authentication.
- **Responsive Design**: Optimized for all device sizes.

---

## Tech Stack

### Frontend
- **React.js**
- **Tailwind CSS** (or CSS framework of choice)
- **Axios** for API requests

### Backend
- **Node.js**
- **Express.js**

### Database
- **MySQL** (using **XAMPP** for local development)

---

## Installation and Setup

### Prerequisites
1. **Node.js** (v16.x or above)
2. **XAMPP** with MySQL
3. **npm** or **yarn**

### Clone the Repository
```bash
git clone https://github.com/your-repo/Employee-Salary-Analysis.git
cd Employee-Salary-Analysis
```

### Backend Setup
1. Navigate to the backend directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add the following variables:
   ```env
   DB_HOST=localhost
   DB_USER=root
   DB_PASSWORD=your_mysql_password
   DB_NAME=employee_db
   PORT=5000
   ```
4. Start the server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the frontend directory:
   ```bash
   cd ../frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm start
   ```

### Database Setup
1. Open **XAMPP** and start **Apache** and **MySQL**.
2. Access **phpMyAdmin** at `http://localhost/phpmyadmin`.
3. Create a new database named `employee_db`.
4. Import the `employee_db.sql` file from the `/database` folder into the database.

---

## Project Structure

### Frontend
```
frontend/
├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── App.js
└── package.json
```

### Backend
```
backend/
├── routes/
├── controllers/
├── models/
├── config/
├── server.js
└── package.json
```

### Database
```
database/
└── employee_db.sql
```

---

## API Endpoints

### Base URL: `http://localhost:5000/api`

| Method | Endpoint       | Description                 |
|--------|----------------|-----------------------------|
| GET    | `/employees`   | Fetch all employee records  |
| POST   | `/employees`   | Add a new employee          |
| PUT    | `/employees/:id` | Update an employee record |
| DELETE | `/employees/:id` | Delete an employee record |

---

## Scripts

### Backend
- Start the backend server:
  ```bash
  npm start
  ```

### Frontend
- Start the React development server:
  ```bash
  npm start
  ```

---

## Future Enhancements

- Add JWT authentication for secure access.
- Integrate advanced data visualizations for salary trends.
- Include role-based access control (RBAC).

---

## Troubleshooting

- Ensure MySQL is running on XAMPP.
- Check `.env` file for correct database credentials.
- Make sure the front-end and back-end servers are running on their respective ports.

---

## Contributors

- **Gokul Nath S** - Developer
- Feel free to contribute by submitting a pull request!

---
