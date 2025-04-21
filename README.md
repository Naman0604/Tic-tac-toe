# 🧠 TIC-TAC-TOE

A classic two-player Tic-Tac-Toe game built with modern web technologies using Vite for the frontend and Node.js for the backend.

## 📦 Project Structure

```
TIC-TAC-TOE/
├── src/                     # Frontend source code (React/Vite)
├── public/                  # Static assets
├── index.html               # HTML entry point
├── tic-tac-toe_server/      # Backend server (Node.js + Express)
│   ├── server.js            # Server entry point
│   └── package.json         # Backend dependencies
├── package.json             # Root manifest
├── vite.config.js           # Vite configuration
└── README.md                # You're here!
```

---

## 🚀 Features

- 🎮 Interactive Tic-Tac-Toe UI with player switching
- ⚙️ Backend server to handle game logic or state (extendable for multiplayer)
- 🛠 Powered by [Vite](https://vitejs.dev/) for ultra-fast dev experience
- 🌐 Deployable as full-stack or split frontend/backend

---

## 🧰 Getting Started

### 🔧 Prerequisites

- Node.js (v16+ recommended)
- npm

### 🖥️ Frontend Setup

```bash
cd TIC-TAC-TOE
npm install
npm run dev
```

### 🖧 Backend Setup

```bash
cd TIC-TAC-TOE/tic-tac-toe_server
npm install
node server.js
```

By default, the frontend runs on [http://localhost:5173](http://localhost:5173) and the backend on [http://localhost:3000](http://localhost:3000).

---

## 🧪 Scripts

From the root directory:

| Command             | Description                     |
|---------------------|---------------------------------|
| `npm run dev`       | Start Vite development server   |
| `npm run build`     | Build frontend for production   |
| `npm start`         | Start backend server            |

---

## 🌍 Deployment Guide

### Option A: Combined Full-Stack (Render, Railway)

1. Push to GitHub
2. Ensure `server.js` serves the `dist` folder (after `vite build`)
3. Add scripts in root `package.json`:
   ```json
   "scripts": {
     "build": "vite build",
     "start": "node tic-tac-toe_server/server.js"
   }
   ```
4. Use platform build command: `npm run build`
5. Start command: `npm start`

### Option B: Separate

- Deploy frontend (e.g., Vercel, Netlify) after `npm run build`
- Deploy backend (e.g., Render) pointing to `server.js`
- Update API URLs in frontend accordingly

---

## 📄 License

MIT License. Feel free to use and extend!

---

## 🙌 Acknowledgements

Built using:
- [Vite](https://vitejs.dev/)
- [Node.js](https://nodejs.org/)
- [Express](https://expressjs.com/)
