# Job Finder

A job finder platform where users can register, log in and manage their profile. Built with an Angular frontend and a Flask + MySQL backend.

## Project Structure
```
frontend/   Angular 9 app (auth, user management, profile views)
backend/    Flask REST API (user registration and login)
```

## Features
- User registration and login with JWT-style auth flow
- Passwords hashed with `passlib` (sha256_crypt)
- User list with add, edit and delete
- Profile image view
- Angular route guards and HTTP interceptors

## Tech Stack
- **Frontend:** Angular 9, Angular Material, Flex Layout, RxJS
- **Backend:** Flask, Flask-SQLAlchemy, Flask-CORS, MySQL

## Getting Started

### Backend
```bash
cd backend
pip install flask flask_sqlalchemy flask_cors passlib mysqlclient
python app.py
```

### Frontend
```bash
cd frontend
npm install
npm start
```
API requests are proxied to the Flask server via `src/proxy.conf.json`.

## Credits
The authentication part of the frontend is based on Jason Watmore's Angular 9 registration and login example (MIT licensed, see `frontend/LICENSE`).
