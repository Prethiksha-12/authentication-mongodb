# Authentication Module — MongoDB + Tailwind CSS

This version replaces MySQL with MongoDB and Bootstrap with Tailwind CSS.

## Features
- Registration
- Login/logout
- bcrypt password hashing
- JWT authentication
- Role-based access
- Change password
- Forgot/reset password
- Protected React route

## Setup
1. Install MongoDB Community Server or use MongoDB Atlas.
2. Extract this project.
3. Backend: `cd backend`, `npm install`, copy `.env.example` to `.env`, then `npm run dev`.
4. Frontend: open another terminal, `cd frontend`, `npm install`, `npm run dev`.
5. Open `http://localhost:5173`.

Default local MongoDB URI: `mongodb://127.0.0.1:27017/employee_management`

MongoDB automatically creates the database and `users` collection when the first user registers. You no longer need the MySQL Workbench database/table for this version.

Public registration creates EMPLOYEE users. ADMIN and PROJECT_MANAGER should be assigned through an authorized admin workflow.

The development forgot-password endpoint returns a reset token for testing; production should email a reset link instead.
