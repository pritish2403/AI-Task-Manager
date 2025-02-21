AI Task Manager
A simple task manager with authentication, built using:

Backend: Golang (Fiber)
Frontend: Next.js (TypeScript)
Database: In-Memory (NoSQL for demo)

Features
User Registration & Login (JWT Authentication)
Task Management (Create, Read, Update, Delete)
Secure API Routes (Protected with JWT)
Minimal UI

How to Run This Project
Clone the Repository
git clone https://github.com/your-username/your-repository.git
cd your-repository

Start the Backend (Golang + Fiber)
cd backend
go run main.go

Start the Frontend (Next.js + TypeScript)
cd frontend
npm install
npm run dev
Visit http://localhost:3000 in your browser.

Test API (Using Postman or cURL)
Register a User
curl -X POST http://localhost:3001/register -H "Content-Type: application/json" -d '{"username": "testuser", "password": "mypassword"}'

Login to Get Token
curl -X POST http://localhost:3001/login -H "Content-Type: application/json" -d '{"username": "testuser", "password": "mypassword"}'

Access Protected Task Routes
curl -X GET http://localhost:3001/tasks -H "Authorization: Bearer YOUR_TOKEN_HERE"
Demo Video
Click here to watch the demo

Contact & Support
If you have any issues, feel free to open an issue on GitHub.

Save & Push README to GitHub
git add README.md
git commit -m "Added README"
git push origin main
