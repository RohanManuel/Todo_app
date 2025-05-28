# 📝 Todo Task Management Web Application

This is a full-stack Todo Task Management Web Application developed for the Katomaran Full Stack Hackathon. It enables users to log in via Google, GitHub and manage their personal tasks with full CRUD functionality.

## 🔧 Features

- Social media login (Google, GitHub)
- Add, view, update, delete tasks
- Mark tasks as complete or open
- Responsive UI for both mobile and desktop
- Secure user authentication and task management

## 🧱 Tech Stack

- **Frontend:** React, TailwindCSS
- **Backend:** Node.js, Express.js
- **Database:** Supabase
- **Authentication:** Supabase Auth (for social logins)
- **Deployment:**
  - Frontend: Vercel
  - Database: Supabase

## 🚀 How to Setup Locally

### 1. Clone the repository

git clone https://github.com/your-username/Todo_app.git

cd Todo_app

### 2. Set up environment variables

Create a .env file in the folder:

NEXT_PUBLIC_SUPABASE_URL=Your_Url

NEXT_PUBLIC_SUPABASE_ANON_KEY=Your_Key

KV_REST_API_URL=Your_Url

KV_REST_API_TOKEN=Your_Key

### 3. Install dependencies

npm install

npm run dev

### 4. Visit the app

http://localhost:3000

## 🌐 Live Demo  
You can check out the live deployed version here:  
👉 [Live App](https://todo-app-one-red.vercel.app/)

## 📹 Loom Video  
A walkthrough and demo of the application can be found here:  
👉 [Watch on Loom](https://www.loom.com/share/04cb7ee77d284d24be3e8af89390eaf7?sid=1ba4131a-4086-413f-9606-6eee0a305e32)

### 4. Architecture Diagram

```plaintext
                   +-----------------------------+
                   |    User (Browser/Mobile)    |
                   +-------------+---------------+
                                 |
                                 v
                   +-----------------------------+
                   |      Frontend (React.js)     |
                   | - Login (OAuth: Google, Git) |
                   | - Dashboard & Task UI        |
                   | - REST API Calls             |
                   +-------------+----------------+
                                 |
                                 v
                   +-----------------------------+
                   |      Backend (Node.js +      |
                   |     Express/Nest.js)         |
                   | - RESTful APIs               |
                   | - Auth (JWT/session)         |
                   | - Input Validation           |
                   | - Task CRUD operations       |
                   +-------------+----------------+
                                 |
            +--------------------+--------------------+
            |                                         |
            v                                         v
+--------------------------+             +-----------------------------+
|  OAuth Provider (Google, |             | Database (MongoDB / SQL)     |
|  GitHub, Facebook, etc)  |             | - Users Collection/Table     |
| - Auth token exchange    |             | - Tasks Collection/Table     |
+--------------------------+             +-----------------------------+

                                |
                                v
                    +---------------------------+
                    |     Deployment Platforms   |
                    |---------------------------|
                    | Frontend: Vercel/Firebase  |
                    | Backend: Railway/Render    |
                    | DB: MongoDB Atlas / Supabase|
                    +---------------------------+

```plaintext



🚀 This project was developed as part of a hackathon organized by [Katomaran](https://www.katomaran.com).
