# AI Quiz Generator 

An intelligent web application that generates **MCQs**, **Fill-in-the-Blank**, and **True/False** questions from any given paragraph or topic using **Google Gemini AI**.

Built with a **Flask backend**, **Tailwind CSS frontend**, and a **secure login system with SQLite3**.  
Designed as a B.Tech final-year project integrating **AI + Web Development + Databases**.

---

## 🚀 Features

✅ **AI-Powered Quiz Generation** – Automatically generates 10 questions using Gemini (`gemini-pro` model).  
✅ **Multiple Question Types** – MCQ, Fill-in-the-Blank, and True/False modes.  
✅ **User Authentication System** – Secure Signup/Login using `bcrypt` password hashing.  
✅ **Quiz History** – Every quiz generated is saved in the user’s history.  
✅ **Responsive UI** – Clean, modern frontend built with Tailwind CSS.  
✅ **Theme Toggle** – Light and dark themes with persistent state.  
✅ **Modular Codebase** – Clean separation between frontend and backend.  

---

## 🏗️ System Architecture

           ┌──────────────────────────────┐
           │          Frontend            │
           │  (HTML + Tailwind + JS)      │
           ├──────────────────────────────┤
           │  index.html / quiz.html      │
           │  script.js                   │
           │  - Handles signup/login UI   │
           │  - Sends API requests        │
           │  - Displays quizzes          │
           └────────────┬─────────────────┘
                        │  REST API (JSON)
                        ▼
           ┌──────────────────────────────┐
           │          Backend             │
           │     (Flask + Python)         │
           ├──────────────────────────────┤
           │  app.py                      │
           │  - /api/signup               │
           │  - /api/login                │
           │  - /api/generate (Gemini)    │
           │  - /api/save-history         │
           │  - /api/history              │
           └────────────┬─────────────────┘
                        │  SQLite3
                        ▼
           ┌──────────────────────────────┐
           │          Database            │
           │        (app.db file)         │
           ├──────────────────────────────┤
           │ users table                  │
           │ history table                │
           └──────────────────────────────┘



