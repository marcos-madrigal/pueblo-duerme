# Pueblo Duerme Online (Multiplayer Social Deduction Game)

A real-time multiplayer browser game inspired by the classic social deduction party game *Werewolf* (*Pueblo Duerme*). Built with **Node.js**, **Express**, and **Socket.IO** for low-latency bidirectional communication between players.

🔗 **Live Beta Demo:** [Play Pueblo Duerme Online](https://pueblo-duerme-9hx1.onrender.com/)

> **Status:** Active Beta — Core real-time gameplay loop, WebSocket event handling, and role mechanics are live. Custom room creation & lobby management are currently in progress.

---

### Key Features
- **Real-Time WebSocket Architecture:** Powered by Socket.IO to synchronize player connections, game states, and votes instantaneously across clients.
- **Server-Authoritative Game Loop:** Centralized state machine in `server.js` handling day/night phases, role assignments, and win conditions to prevent client-side tampering.
- **Zero-Install Browser Client:** Lightweight frontend (`public/index.html`) accessible directly from any web browser via Render.

---

### Tech Stack
- **Backend:** Node.js, Express
- **Real-Time Communication:** Socket.IO (WebSockets)
- **Frontend:** HTML5, CSS3, Vanilla JavaScript
- **Deployment:** Render

---

### Project Structure
```text
pueblo-duerme/
├── public/
│   └── index.html      # Client UI, styles, and Socket.IO client logic
├── server.js           # Express server, Socket.IO event handlers, and game state engine
├── package.json        # Dependencies and start scripts
└── .gitignore
```

---

### Running Locally

1. Clone the repository:
```bash
git clone [https://github.com/marcos-madrigal/pueblo-duerme.git](https://github.com/marcos-madrigal/pueblo-duerme.git)
cd pueblo-duerme
```

2. Install dependencies:
```bash
npm install
```

3. Start the server:
```bash
node server.js
```

4. Open `http://localhost:3000` in multiple browser tabs to simulate a local multiplayer lobby (or jump straight into the hosted version at [pueblo-duerme.onrender.com](https://pueblo-duerme.onrender.com/)).

---

### Roadmap
- [x] Real-time Socket.IO connection and player synchronization
- [x] Core day/night cycle and role mechanics
- [x] Cloud deployment on Render
- [ ] Custom room creation with shareable room codes
- [ ] Reconnection handling and mobile UI enhancements
