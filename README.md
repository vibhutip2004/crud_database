# W3-A2: Connecting CRUD API to SQLite Database

A database-backed Task Management REST API built with **FastAPI** and **SQLite** for the FlyRank Internship Backend Development Track.

---

## 📌 Features
- **Persistent Storage:** Replaced in-memory storage with SQLite (`tasks.db`), ensuring data survives server restarts.
- **RESTful Endpoints:** Complete CRUD support (`GET`, `POST`, `PUT`, `DELETE`).
- **Data Validation & Error Handling:** Proper HTTP status codes (`200 OK`, `201 Created`, `204 No Content`, `400 Bad Request`, `404 Not Found`).
- **SQL Safety:** Uses parameterized queries to prevent SQL injection risks.
- **Auto-Initialization:** Database table creation and default seeding (3 initial tasks) trigger automatically on first launch.

---

## 🏗️ Architecture & Database Choice

### Why SQLite?
SQLite was chosen because it is serverless, zero-configuration, and stores the entire database in a single local file (`tasks.db`). This allows full persistence across application restarts without requiring external database server installation or setup.

### Database Location
The database file `tasks.db` is automatically created at the root directory of the application upon startup. It is listed in `.gitignore` so that every fresh environment clone initializes independently with default seed data.

---

## 🚀 How to Run the Project

### 1. Setup Virtual Environment
```bash
python -m venv venv
venv\Scripts\activate

**ScreenShots **
<img width="1366" height="768" alt="Screenshot (178)" src="https://github.com/user-attachments/assets/cb8502fc-162c-4c08-a6cf-f4624c5e1161" />
<img width="1366" height="768" alt="Screenshot (175)" src="https://github.com/user-attachments/assets/99f0860f-d3d1-4c29-b1d9-1576c37c3cea" />
<img width="1366" height="768" alt="Screenshot (177)" src="https://github.com/user-attachments/assets/3753b465-87f5-4b2f-a170-aaeba979043f" />
<img width="1366" height="768" alt="Screenshot (182)" src="https://github.com/user-attachments/assets/df8abb74-1fff-40d4-92d2-1e1ec540dd2c" />
<img width="1366" height="768" alt="Screenshot (181)" src="https://github.com/user-attachments/assets/4b57d99b-ec57-4550-b38f-744f00c08cd3" />
<img width="1366" height="768" alt="Screenshot (179)" src="https://github.com/user-attachments/assets/283edd50-c689-4b0f-aae9-4252d294f38e" />
