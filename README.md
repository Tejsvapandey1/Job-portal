Nice 🚀 — now I see your **routes** for the Job-portal app. That means your API is not just CRUD for jobs, but also has **authentication, stats, and user management**.

Let me update both the **README.md** and the **resume description** to reflect these properly.

---

## 📘 Updated README.md (with your routes)

```markdown
# Job Portal Application

A backend web application for managing job postings and user accounts.  
Built with **Node.js** and **Express**, featuring authentication, job statistics, and secure CRUD operations.

---

## ✨ Features

- 🔐 User authentication (register & login with rate limiting)
- 👤 User profile update endpoint
- 📋 Create, read, update, and delete job postings
- 📊 Job statistics & filtering
- 🛡️ Protected routes with middleware (`userAuth`)
- 🚦 Rate limiting to prevent brute-force login/register attempts
- 🧩 Modular project structure with controllers, models, routes, and middleware

---

## 📁 Project Structure

```

.
├── config/              # Config files (DB, JWT, etc.)
├── controllers/         # Route handlers (jobs, auth, users)
├── middlewares/         # userAuth, validation, rate limiting
├── models/              # Data models (User, Job)
├── routes/              # Express route definitions
├── server.js            # App entry point
├── package.json
└── README.md

````

---

## 🚀 Getting Started

### Prerequisites

- Node.js (v14+ recommended)  
- npm or yarn  
- MongoDB (local or cloud, if integrated)

### Installation

```bash
git clone https://github.com/Tejsvapandey1/Job-portal.git
cd Job-portal
npm install
````

### Running the App

```bash
npm start
```

Visit `http://localhost:3000` (or your configured port).

---

## 🧭 API Endpoints

### 🔐 Authentication

| Method | Route       | Description       |
| ------ | ----------- | ----------------- |
| POST   | `/login`    | User login        |
| POST   | `/register` | User registration |

### 📋 Jobs

| Method | Route             | Description               |
| ------ | ----------------- | ------------------------- |
| POST   | `/create-job`     | Create a new job          |
| GET    | `/get-job`        | Get all jobs (for a user) |
| PATCH  | `/update-job/:id` | Update a job by ID        |
| DELETE | `/delete-job/:id` | Delete a job by ID        |
| GET    | `/job-stats`      | Get job stats & filters   |

### 👤 Users

| Method | Route          | Description         |
| ------ | -------------- | ------------------- |
| PUT    | `/update-user` | Update user profile |

### 🧪 Testing

| Method | Route        | Description               |
| ------ | ------------ | ------------------------- |
| POST   | `/test-post` | Test protected POST route |

---

## 🔧 Future Enhancements

* Add JWT refresh tokens & session handling
* Role-based access (Admin, Employer, Candidate)
* Advanced job filters (location, salary, remote, etc.)
* Resume uploads & file handling
* Integration with frontend client (React, Angular, Vue)
* Containerization with Docker

---

## 👨‍💻 Author

Developed and maintained by **Tejsva Pandey**.
Feel free to fork and extend this project.

