# securesight

# Features

1. Incident Player – View the associated video or image from each camera

2. Incident List – Displays recent incidents with camera name, type, and time

3. Resolve Button – Mark an incident as resolved with optimistic UI

4. Seed API – /api/seed inserts sample incidents and cameras into the database

# REST API –

GET /api/incidents?resolved=false

PATCH /api/incidents/:id/resolve


# Tech Stack

Area	Tech Stack

Frontend	Next.js (App Router), Tailwind CSS
Backend	Express.js, Node.js, SQLite
Database	SQLite (file-based)
Deployment	Render (Backend), GitHub



---

# Sample Data

-- Cameras
Camera 1, Camera 2, Camera 3

-- Incidents
- Unauthorized Access
- Gun Threat
- Loitering


---

# Installation (Local)

# Clone the repo
git clone https://github.com/your-username/securesight.git
cd securesight-backend

# Install backend dependencies
npm install

# Run backend server
node backend/server.js

# In another terminal for frontend
cd securesight-frontend
npm install
npm run dev


---

# Environment Setup (Optional)

If you're using environment variables (like DB path or PORT):

.env

PORT=4000
DATABASE_PATH=./securesight.db

Then update server.js:

require('dotenv').config();
const PORT = process.env.PORT || 4000;


# Deployment Steps

Backend (Render)

1. Push code to GitHub
2. Go to Render
3. Create New Web Service → Connect GitHub
4. Set Build Command: npm install
5. Set Start Command: node backend/server.js
6. Set Environment:

PORT=4000 (if needed)

---

✅ Submission Checklist

[x] Deployed backend on Render

[x] /api/incidents and /api/seed tested

[x] Frontend connected and functional

[x] Video/Image player with resolve option

[x] Responsive and clean UI



---
