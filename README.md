# Government Officer Portal

Admin and Officer logins, each with their own dashboard.
Stack: HTML/CSS/JavaScript frontend, Python (Flask) backend, MySQL database.

## Run it
1. Install Python 3.9+ and MySQL 8 (make sure MySQL is running).
2. `cd backend && pip install -r requirements.txt`
3. Set your MySQL login (defaults: user `root`, empty password, database `gov_portal`):
   - Windows: `set DB_USER=root` and `set DB_PASSWORD=yourpassword`
   - Mac/Linux: `export DB_USER=root DB_PASSWORD=yourpassword`
   - Also set `SECRET_KEY` to a long random string.
4. `python app.py` - creates the database, tables and two starter accounts.
5. Open http://localhost:5000

## Starter accounts (change these passwords after first login)
| Role    | Email           | Password    |
|---------|-----------------|-------------|
| Admin   | admin@gov.in    | Admin@123   |
| Officer | officer@gov.in  | Officer@123 |

## Features
- Admin: dashboard stats, add/remove officers, assign/track/delete tasks, approve/reject leave, post/delete announcements, profile.
- Officer: personal dashboard, view and update own task status, apply for leave and track it, read announcements, profile and password change.

## Folders
- `frontend/` - index.html, css/style.css, js/app.js
- `backend/` - app.py (REST API), schema.sql (MySQL tables), requirements.txt
- `preview.html` - single-file demo that runs without the backend (data kept in browser)
