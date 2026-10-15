# Agaetis_task_saalim--15-10

# Employee Directory

A simple full-stack Employee Directory application that allows users to add, view, edit, delete, and search employee records.

## Tech Stack

**Frontend**
- React + TypeScript (Vite)
- Redux Toolkit for state management
- Axios for API requests
- CSS for styling

**Backend**
- Node.js + Express.js
- Prisma ORM
- PostgreSQL / MySQL
- REST API

## Features

- Add new employees with name, email, and job role
- View all employee records
- Edit existing employee details
- Delete employee records
- Search employees by name
- Manage frontend state using Redux Toolkit
- Store employee data in a relational database using Prisma ORM
- REST API with CORS enabled

## Database Schema

Each employee record includes:

- `id` — Primary key
- `name` — Employee name
- `email` — Employee email
- `role` — Job role
- `created_at` — Record creation timestamp

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/employees` | Fetch all employees |
| POST | `/employees` | Add an employee |
| PUT | `/employees/:id` | Update an employee |
| DELETE | `/employees/:id` | Delete an employee |

## Getting Started

1. Clone the repository.
2. Install frontend and backend dependencies.
3. Configure your database connection in the backend `.env` file.
4. Run Prisma migrations to create the database tables.
5. Start the backend server.
6. Start the frontend development server.

## Environment Variables

Configure the required variables in your backend `.env` file, such as:

```env
PORT=5000
```

## Run the Project

**Frontend**
```bash
cd frontend
npm install
npm run dev
```

**Backend**
```bash
cd backend
npm install
npx prisma migrate dev
npm run dev
```

Ensure your database is running and the backend API URL is configured correctly in the frontend.

## Author

Developed as a full-stack development task to demonstrate CRUD operations, REST API integration, database management, and state management.
