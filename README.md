# Snippet Samurai

A full-stack web app that lets developers search, view, and share code snippets — built in one week as a School of Code bootcamp project.

![Snippet Samurai](https://i.imgur.com/xYKiF06.png)

---

## About

Snippet Samurai was built with bootcampers in mind. Learning to code means constantly revisiting syntax and patterns — this app gives you a quick, low-friction way to find code snippets by keyword and contribute your own. The UI is intentionally minimal to reduce cognitive load.

### Features

- Search snippets by title with live filtering
- View snippet details including code syntax, description, docs, and video links
- Submit new snippets to the shared database
- Responsive UI built with Material UI

---

## Tech Stack

### Frontend
| Technology | Purpose |
|---|---|
| React 18 | UI framework |
| React Router | Client-side routing |
| Axios | HTTP requests to the API |
| Material UI (MUI) | Component library and styling |
| Cypress | End-to-end testing |
| Jest + React Testing Library | Unit and component testing |

### Backend
| Technology | Purpose |
|---|---|
| Node.js + Express | REST API server |
| PostgreSQL | Relational database |
| `pg` | PostgreSQL client for Node |
| dotenv | Environment variable management |
| cors | Cross-origin request handling |
| nodemon | Development auto-reloading |

---

## API Endpoints

| Method | Endpoint | Description |
|---|---|---|
| GET | `/snippets?title=<query>` | Search snippets by title |
| POST | `/snippets` | Submit a new snippet |
| DELETE | `/snippets/:id` | Delete a snippet by ID |

---

## Running Locally

You'll need **Node.js** and a **PostgreSQL** database set up before starting.

### 1. Clone both repositories

```bash
git clone https://github.com/SchoolOfCode/w9_backend-project-syntax-samurai-s
git clone https://github.com/SchoolOfCode/w9_frontend-project-syntax-samurai-s
```

### 2. Set up the Backend

```bash
cd w9_backend-project-syntax-samurai-s
npm install
```

Create a `.env` file in the backend root with your database connection string:

```
DATABASE_URL=your_postgresql_connection_string
```

Set up the database:

```bash
npm run db:createTable
npm run db:populateTable
```

Start the backend server (runs on port 3000):

```bash
npm run dev
```

### 3. Set up the Frontend

In a new terminal:

```bash
cd w9_frontend-project-syntax-samurai-s
npm install
npm start
```

The app will open at `http://localhost:3001`.

---

## Authors

- [Katie Walters](https://github.com/KatieClarinet)
- [Matt Davies](https://github.com/DevMattDavies)
- [Mari](https://github.com/wisteria-hawthorn)
- [CJ](https://github.com/Esva)

---

## License

[![AGPL License](https://img.shields.io/badge/license-AGPL-blue.svg)](http://www.gnu.org/licenses/agpl-3.0)
