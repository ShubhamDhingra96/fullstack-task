# Full Stack Task - Django + React

This is a simple full-stack project built using Django for the backend and React (Vite) for the frontend. It supports basic CRUD operations for managing items.

---

## Tech Stack

**Backend**
- Django
- Django REST Framework
- SQLite

**Frontend**
- React (Vite)
- Axios

---

## Project Structure


backend/
frontend/


---

## Features

- Create, read, and update items
- REST API built with Django REST Framework
- React frontend connected to backend API
- Validation: item names must be unique within each group (Primary / Secondary)

---

## Backend Setup

```bash
cd backend
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python manage.py migrate
python manage.py runserver

Backend runs at:
http://127.0.0.1:8000

Frontend Setup
cd frontend
npm install
npm run dev

Frontend runs at:
http://localhost:5173

API Endpoints
Method	Endpoint	Description
GET	/api/items/	Get all items
POST	/api/items/	Create item
GET	/api/items/<id>/	Get single item
PATCH	/api/items/<id>/	Update item
Item Model

Each item has:

name
group (Primary / Secondary)
created_at
updated_at
Notes
Backend and frontend run separately
Make sure the backend is running before the frontend
API uses JSON format for requests
