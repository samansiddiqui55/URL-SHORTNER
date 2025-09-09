# 🔗 URL Shortener

A **System Design Project** that implements a full-stack URL shortening service.  
Users can input long URLs and generate short, shareable links.  
The project is split into **Backend** (Node.js, Express, MongoDB) and **Frontend** (React + Vite), demonstrating modular design and scalable architecture.  

Live demo: [Netlify Deployment](https://resonant-pika-fa18cb.netlify.app/)  

---

## ✨ Features

- Shortens long URLs into unique, compact links.  
- Redirects users seamlessly from the short link to the original URL.  
- Backend built with **Node.js + Express + MongoDB**.  
- Frontend built with **React + Vite**.  
- Modular separation of concerns between backend and frontend.  
- Scalable design principles suitable for system design projects.  

---

## 🗂 Project Structure

URL-SHORTNER/
│
├── BACKEND/ # Node.js + Express + MongoDB backend
│ ├── src/ # Routes, models, controllers
│ ├── app.js # Main server file
│ ├── .env # Environment variables
│ ├── package.json
│
├── FRONTEND/ # React + Vite frontend
│ ├── src/ # React components
│ ├── index.html
│ ├── vite.config.js
│ ├── package.json
│
### 1. Clone the repository
```bash
git clone https://github.com/samansiddiqui55/URL-SHORTNER.git
cd URL-SHORTNER
## ⚙️ Backend Setup

1. Go to the backend folder:
   ```bash
   cd BACKEND
Install the required dependencies:
npm install
Create a .env file inside the BACKEND directory and add:
MONGO_URI=<your-mongodb-connection-string>
PORT=5000
BASE_URL=http://localhost:5000
Start the backend server:
npm start

## ⚙️ Frontend Setup

1. Go to the frontend folder:
   ```bash
   cd FRONTEND
Install the required dependencies:
npm install
Start the frontend development server:
npm run dev
Open the app in your browser at:
http://localhost:5173

System Design Overview
Frontend (React + Vite) → User inputs a long URL.
Backend (Express + MongoDB) → Generates a unique short code, stores mapping in MongoDB.
Database (MongoDB) → Persists original URL and short code.
Redirection → When the short link is visited, backend retrieves original URL from DB and redirects.
