# 🕒 SlotSwapper — ServiceHive SDE Assignment

## 📘 Overview
SlotSwapper is a **peer-to-peer time-slot scheduling application** that allows users to mark their calendar events as *swappable* and exchange them with other users.  
Built as part of the **ServiceHive Full-Stack Intern Technical Challenge**, this project demonstrates full-stack skills including authentication, database design, RESTful APIs, and dynamic frontend state management.

---

## 🚀 Features

### 🔐 Authentication
- Sign-up and Login using Name, Email, and Password.
- JWT-based session management.
- Protected API routes.

### 📅 Calendar / Events
- Users can create, view, update, and delete their own events.
- Each event has a status: `BUSY`, `SWAPPABLE`, or `SWAP_PENDING`.
- “Make Swappable” toggle to offer an event for swap.

### 🔁 Slot Swapping Logic
- View other users’ *swappable* slots (`GET /api/swappable-slots`).
- Send swap requests (`POST /api/swap-request`).
- Accept or reject incoming swap requests (`POST /api/swap-response/:id`).
- On acceptance, events are exchanged between users.

### 💬 Notifications / Requests
- Dashboard displays **incoming** and **outgoing** swap requests.
- Status updates happen dynamically without a manual refresh.

---

## 🧰 Tech Stack

| Layer | Technology |
|-------|-------------|
| Frontend | React (Vite) |
| State Management | React Context API |
| Backend | Node.js + Express |
| Database | SQLite (can be replaced with Postgre
