# AlumNexus — Alumni Platform

A full-stack web application that connects alumni, facilitates networking, and manages community engagement for educational institutions.

---

## 🚀 Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| React 19 + TypeScript | UI Framework |
| Vite | Build tool & dev server |
| Tailwind CSS | Styling |
| React Router v7 | Client-side routing |
| TanStack Query | Data fetching & caching |
| React Hook Form + Yup | Form handling & validation |
| Axios | HTTP client |
| Lucide React | Icon library |

### Backend
| Technology | Purpose |
|---|---|
| Node.js + Express 5 | REST API server |
| MongoDB + Mongoose | Database & ODM |
| JSON Web Tokens (JWT) | Authentication |
| bcryptjs | Password hashing |
| Multer | File/image uploads |
| dotenv | Environment config |
| nodemon | Dev auto-reload |

---

## ✨ Features

- 🔐 **Authentication** — Register, login, and JWT-protected routes
- 👤 **Alumni Profiles** — View and edit personal profiles with photo uploads
- 📋 **Alumni Directory** — Browse and search all registered alumni
- 💼 **Job Board** — Post and discover job opportunities shared by alumni
- 📅 **Events** — Create and list upcoming alumni events
- 🤝 **Mentorship** — Connect mentors with mentees within the community
- 📰 **Stories** — Share and read alumni success stories
- 💰 **Donations** — Support institutional causes via donation listings

---

## 📁 Project Structure

```
alumni-platform/
├── backend/                  # Node.js + Express REST API
│   ├── controllers/          # Route handler logic
│   ├── middleware/           # Auth & other middleware
│   ├── models/               # Mongoose data models
│   ├── routes/               # API route definitions
│   │   ├── auth.js
│   │   ├── profile.js
│   │   ├── users.js
│   │   ├── jobs.js
│   │   ├── events.js
│   │   ├── donations.js
│   │   ├── stories.js
│   │   └── mentorship.js
│   ├── uploads/              # Uploaded media files
│   ├── utils/                # Utility scripts
│   ├── server.js             # App entry point
│   └── .env                  # Environment variables
│
└── frontend/                 # React + TypeScript SPA
    └── src/
        ├── components/       # Reusable UI components
        ├── context/          # React context (Auth, etc.)
        ├── pages/            # Route-level page components
        │   ├── Home.tsx
        │   ├── Login.tsx
        │   ├── Register.tsx
        │   ├── Profile.tsx
        │   ├── Directory.tsx
        │   ├── JobBoard.tsx
        │   ├── JobPost.tsx
        │   ├── EventList.tsx
        │   ├── EventCreate.tsx
        │   ├── Mentorship.tsx
        │   ├── Stories.tsx
        │   ├── StorySubmit.tsx
        │   └── Donation.tsx
        └── main.tsx          # App entry point
```

---

## ⚙️ Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v18+
- [MongoDB](https://www.mongodb.com/) (local or MongoDB Atlas)
- npm

---

### 1. Clone the Repository

```bash
git clone https://github.com/OmRakholiya/AlumNexus.git
cd AlumNexus
```

---

### 2. Setup the Backend

```bash
cd backend
npm install
```

Create a `.env` file in the `backend/` directory:

```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/alumnexus
JWT_SECRET=your_jwt_secret_key
```

Start the backend server:

```bash
# Development (with auto-reload)
npm run dev

# Production
npm start
```

The API will be available at: `http://localhost:5000`

---

### 3. Setup the Frontend

```bash
cd frontend
npm install
```

Start the development server:

```bash
npm run dev
```

The app will be available at: `http://localhost:5173`

---

## 🔌 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/api/auth/register` | Register a new user |
| POST | `/api/auth/login` | Login and get JWT token |
| GET | `/api/profile/:id` | Get user profile |
| PUT | `/api/profile/:id` | Update user profile |
| GET | `/api/users` | List all alumni |
| GET | `/api/jobs` | List all jobs |
| POST | `/api/jobs` | Post a new job |
| GET | `/api/events` | List all events |
| POST | `/api/events` | Create a new event |
| GET | `/api/mentorship` | List mentorship requests |
| POST | `/api/mentorship` | Create mentorship request |
| GET | `/api/stories` | List all stories |
| POST | `/api/stories` | Submit a new story |
| GET | `/api/donations` | List donation campaigns |

---

## 🛠️ Available Scripts

### Backend (`/backend`)

| Command | Description |
|---------|-------------|
| `npm start` | Start server with Node.js |
| `npm run dev` | Start server with Nodemon (auto-reload) |

### Frontend (`/frontend`)

| Command | Description |
|---------|-------------|
| `npm run dev` | Start Vite dev server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm run lint` | Run ESLint |

---

## 🤝 Contributing

1. Fork the repository
2. Create your feature branch: `git checkout -b feature/your-feature`
3. Commit your changes: `git commit -m "Add your feature"`
4. Push to the branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

---

> Built with ❤️ by [Om Rakholiya](https://github.com/OmRakholiya)
