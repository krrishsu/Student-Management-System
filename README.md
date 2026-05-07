# 🎓 Student Management System

A full-stack web application for managing students, courses, attendance, grades, fees, and teachers — built with **React + Vite** (frontend) and **Node.js + Express + MongoDB** (backend).

---

## 📁 Project Structure

```
student-management-system/
├── client/          # React frontend (Vite)
└── server/          # Node.js + Express backend
```

---

## 🚀 Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| React 19 | UI framework |
| React Router DOM v7 | Client-side routing |
| Axios | HTTP requests |
| React Hook Form | Form handling |
| Vite | Build tool & dev server |

### Backend
| Technology | Purpose |
|---|---|
| Node.js + Express | REST API server |
| MongoDB + Mongoose | Database & ODM |
| JWT (jsonwebtoken) | Authentication |
| bcryptjs | Password hashing |
| dotenv | Environment config |
| nodemon | Dev auto-reload |

---

## ✨ Features

- 🔐 **Authentication** — Login with JWT-based auth
- 👩‍🎓 **Students** — Add, view, and manage student profiles
- 📚 **Courses** — Create and manage course listings
- 📅 **Attendance** — Track student attendance
- 📊 **Grades** — Record and view student grades
- 💰 **Fees** — Manage student fee records
- 👨‍🏫 **Teachers** — Teacher management module
- 📋 **Dashboard** — Overview of key metrics

---

## ⚙️ Getting Started

### Prerequisites
- Node.js (v18+)
- MongoDB (Atlas or local)

### 1. Clone the Repository

```bash
git clone <your-repo-url>
cd student-management-system
```

### 2. Setup the Server

```bash
cd server
npm install
```

Create a `.env` file in the `server/` directory:

```env
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
NODE_ENV=development
```

Start the server:

```bash
# Development (with auto-reload)
npm run dev

# Production
npm start
```

The server runs on **http://localhost:5000**

### 3. Setup the Client

```bash
cd client
npm install
npm run dev
```

The client runs on **http://localhost:5173**

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| POST | `/api/auth/...` | Authentication routes |
| GET/POST/PUT/DELETE | `/api/students/...` | Student CRUD operations |
| GET/POST/PUT/DELETE | `/api/courses/...` | Course CRUD operations |

---

## 🗃️ Database Models

- **User** — Admin/teacher accounts with hashed passwords
- **Student** — Student profiles and details
- **Course** — Course information and assignments

---

## 🔒 Environment Variables

| Variable | Description |
|---|---|
| `PORT` | Server port (default: 5000) |
| `MONGO_URI` | MongoDB connection string |
| `JWT_SECRET` | Secret key for JWT tokens |
| `NODE_ENV` | Environment (`development` / `production`) |

> ⚠️ **Never commit your `.env` file to version control.**

---

## 📦 Build for Production

```bash
# Build the frontend
cd client
npm run build

# The output will be in client/dist/
```

---

## 🤝 Contributing

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a Pull Request

---

## 📄 License

This project is open-source and available under the [MIT License](LICENSE).
