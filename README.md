# mobilityalpha-7zo8

This repository contains a sample **Mobility-as-a-Service (MaaS)** demonstration project.

It includes:

- **Backend (Flask + SQLite)**: REST API for transport modes, trips, and bookings.
- **Frontend (vanilla HTML/CSS/JS)**: Simple UI to search trips and create bookings.

---

## 🚀 Getting Started (Backend)

1. Create a Python virtual environment (recommended):

   ```bash
   python -m venv .venv
   .venv\Scripts\activate
   ```

2. Install dependencies:

   ```bash
   pip install -r backend/requirements.txt
   ```

3. Initialize the database and seed sample data:

   ```bash
   python backend/app.py --init-db
   ```

4. Run the API server:

   ```bash
   python backend/app.py
   ```

   The API is available at: http://localhost:5000/api

---

## 🌐 Frontend

To use the frontend, open `frontend/index.html` in a browser. The frontend expects the backend to be running at `http://localhost:5000`.

---

## 🧩 API Endpoints (Sample)

- `GET /api/health` – health check
- `GET /api/modes` – list transport modes
- `GET /api/trips` – search trips (query params: `origin`, `destination`, `mode_id`)
- `POST /api/bookings` – create a booking
- `GET /api/bookings/:id` – view a booking
