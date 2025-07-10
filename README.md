# 🚀 Eduverse API — A Complete Course Selling Backend Platform

Eduverse API is a powerful, production-ready backend system for a course-selling platform. It supports role-based access control for users and admins, secure authentication, course management, and purchase tracking — built using modern Node.js best practices.

This project is designed to demonstrate real-world backend engineering skills and can easily integrate with any frontend framework.

---

## 📌 Live Features

### 👤 User Functionality
- ✅ Sign up & login securely
- ✅ JWT-based user authentication
- ✅ Purchase courses
- ✅ View purchased courses

### 🔐 Admin Functionality
- ✅ Admin registration & login
- ✅ JWT-based admin authentication
- ✅ Create new courses
- ✅ Update existing courses
- ✅ View all created courses

### 🧰 Middleware & Security
- ✅ Custom authentication middleware for users & admins
- ✅ Passwords hashed using `bcrypt`
- ✅ Role-based access protection
- ✅ Input validation with `zod` and `safeParse()`

### 🧪 API Response
- ✅ Consistent status codes and JSON responses
- ✅ Error handling for validation & database failures

---

## 🛠️ Tech Stack

| Tech             | Purpose                                      |
|------------------|----------------------------------------------|
| **Node.js**       | Runtime environment for backend              |
| **Express.js**    | Fast, minimalist backend framework           |
| **MongoDB**       | NoSQL database for persistent storage        |
| **Mongoose**      | ODM for MongoDB                              |
| **JWT**           | Secure authentication tokens                 |
| **bcrypt**        | Password hashing                             |
| **dotenv**        | Environment variable handling                |
| **zod**           | Schema-based input validation                |

---

## 📂 Project Structure
```
eduverse-api/
├── middleware/
│ ├── admin.js    # Admin auth middleware
│ └── user.js    # User auth middleware
├── routes/
│ ├── admin.js    # Admin endpoints
│ ├── course.js    # Course endpoints (via admin)
│ └── user.js    # User endpoints
├── db.js    # Mongoose schemas and models
├── index.js    # Server entry point
├── .env    # Secret config (local)
├── .env.example    # Sample env file
├── package.json
└── README.md
```

## 🧪 Sample Endpoints

### User
- `POST /user/signup` — Register new user
- `POST /user/login` — Login user
- `GET /user/purchases` — Get all purchased courses (JWT required)

### Admin
- `POST /admin/signup` — Register new admin
- `POST /admin/login` — Login admin
- `POST /admin/course` — Create new course (JWT required)
- `PUT /admin/course` — Update course
- `GET /admin/course/bulk` — View all created courses

---

## 🧾 Environment Variables

Create a `.env` file in the root folder with the following:
- MONGODB_URI=mongodb+srv://youruser:yourpass@yourcluster.mongodb.net/eduverse
- JWT_SECRET_USER=your_user_secret
- JWT_SECRET_ADMIN=your_admin_secret

---

## 💡 Setup & Run Locally

```bash
git clone https://github.com/sanjitxdutta/eduverse-api
cd eduverse-api
npm install
touch .env # Add your environment variables
node index.js
```

---

## ✨ Author
Sanjit Dutta
📍 India | 💻 Backend Developer
GitHub | LinkedIn

---

## 📝 License
MIT License

