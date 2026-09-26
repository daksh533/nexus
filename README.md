Nexus 💬

A real-time chat application built on the MERN stack, with live messaging, authentication, and presence tracking.

🔗 Live Demo: nexus-lhu2.onrender.com

✨ Features
Real-time messaging — instant message delivery powered by Socket.io
Secure authentication — JWT-based login and session handling
Online status — see which users are currently active
Read receipts — know when your messages have been seen
Responsive UI — built with React for a smooth experience across devices
🛠️ Tech Stack

Frontend

React (Vite)
Socket.io Client

Backend

Node.js
Express.js
Socket.io
JWT (JSON Web Tokens) for authentication

Database

MongoDB

Deployment

Render
📂 Project Structure
nexus/
├── client/          # React frontend (Vite)
│   ├── src/
│   └── ...
├── server/          # Express backend
│   ├── controllers/
│   ├── models/
│   ├── routes/
│   ├── socket/
│   └── ...
└── README.md

Adjust this structure to match your actual repo layout.

🚀 Getting Started
Prerequisites
Node.js (v18 or higher recommended)
MongoDB (local instance or MongoDB Atlas)
Installation
Clone the repository
bash
   git clone https://github.com/<your-username>/nexus.git
   cd nexus
Install dependencies
bash
   # Backend
   cd server
   npm install

   # Frontend
   cd ../client
   npm install
Set up environment variables Create a .env file in the server directory:
env
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   CLIENT_URL=http://localhost:5173
Run the app
bash
   # Start the backend (from /server)
   npm run dev

   # Start the frontend (from /client)
   npm run dev
Open http://localhost:5173 in your browser 🎉
🔐 Authentication Flow
User signs up / logs in via the auth API
Server issues a JWT on successful login
Token is stored client-side and sent with subsequent requests
Socket.io connection is authenticated using the same token, enabling real-time features per user
📸 Screenshots




🗺️ Roadmap
 Group chats
 Media/file sharing
 Message reactions
 Push notifications
🤝 Contributing

👤 Author

Daksh

GitHub: daksh533

⭐️ If you like this project, consider giving it a star on GitHub!
