# Authentication API

Base URL: `http://localhost:5000/api/auth`

POST `/register` — name, email, password

POST `/login` — email, password

POST `/logout` — Bearer JWT

GET `/me` — Bearer JWT

PUT `/change-password` — Bearer JWT

POST `/forgot-password` — email

POST `/reset-password` — token, newPassword

GET `/admin` — ADMIN only

GET `/manager` — ADMIN or PROJECT_MANAGER
