Here’s a clean, production-ready README.md for BingeBox, written the way open-source and startup projects usually present themselves. You can copy-paste this directly.

⸻


# 🎬 BingeBox

**BingeBox** is a self-hosted movie streaming and watch-party platform that lets users stream local media, fetch metadata from TMDB, and host synchronized watch parties with peers — all powered by a modern Node.js backend and a fast Vite-based frontend.

---

## ✨ Features

- 🎥 Stream locally stored movies
- 🧠 Automatic movie metadata via TMDB
- 👥 Real-time watch parties
- 📡 Peer discovery and tracking
- 💾 SQLite database for lightweight persistence
- 🐳 Fully Dockerized (backend + frontend)
- ⚡ Fast frontend built with Vite

---

## 🏗️ Project Structure

bingeBox/
├── backend/
│   ├── src/
│   ├── dist/
│   ├── media/           # Media files (mounted volume)
│   ├── Dockerfile
│   └── package.json
│
├── frontend/
│   ├── src/
│   ├── dist/
│   ├── Dockerfile
│   └── package.json
│
├── data/                # SQLite database (mounted volume)
│   └── bingebox.db
│
├── docker-compose.yml
├── .env
└── README.md

---

## ⚙️ Tech Stack

### Backend
- Node.js (v20)
- TypeScript
- Express
- better-sqlite3
- TMDB API

### Frontend
- React
- Vite
- TypeScript
- Tailwind CSS

### Infrastructure
- Docker & Docker Compose
- SQLite
- Volume-based persistence

---

## 🔐 Environment Variables

Create a `.env` file in the project root:

```env
PORT=3000
NODE_ENV=production
TMDB_API_KEY=YOUR_TMDB_API_KEY
MEDIA_PATH=/app/media
DB_PATH=/app/data/bingebox.db
PEER_ID=local_peer


⸻

🐳 Running with Docker (Recommended)

Make sure Docker and Docker Compose are installed.

Build and start everything:

docker-compose build
docker-compose up

Access the app:
	•	Frontend: http://localhost:5173
	•	Backend API: http://localhost:3000

⸻

📦 Volumes & Persistence

BingeBox uses Docker volumes to persist data:
	•	./data → SQLite database
	•	./backend/media → Local movie files

Your data remains safe even if containers restart.

⸻

🛠️ Development (Without Docker)

Backend

cd backend
npm install
npm run dev

Frontend

cd frontend
npm install
npm run dev


⸻

🚀 Deployment Notes
	•	Designed to work on Linux, macOS, and Windows
	•	Works well with:
	•	VPS hosting
	•	Home servers
	•	NAS setups
	•	Reverse proxy (Nginx) is optional but recommended for production

⸻

🧠 Future Improvements
	•	User authentication
	•	Remote peer discovery
	•	Subtitles support
	•	Multiple media libraries
	•	Mobile-friendly UI

⸻

📄 License

MIT License © 2026 BingeBox

⸻

🙌 Acknowledgements
	•	TMDB￼ for movie metadata
	•	Node.js & Docker communities

---

If you want, I can also:
- 🔥 Add **badges** (Docker, Node, License)
- 🧩 Tailor it for **GitHub sponsors / hackathons**
- 🧪 Add **API documentation section**
- 🖼️ Include screenshots section

Just tell me 👍











