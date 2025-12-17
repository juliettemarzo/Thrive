# Thrive App

A full-stack web application built with **Node.js**, **Express**, and **MongoDB (Mongoose)** that allows users to sign up, log in, and manage personal goals. This project was built as part of a full-stack development course and is designed to be easy to run locally.

---

## Features

* User authentication (sign up & login)
* Create, view, update, and delete goals
* MongoDB Atlas database with Mongoose
* RESTful API structure
* Static frontend served from the `public` folder

---

## Tech Stack

* **Backend:** Node.js, Express
* **Database:** MongoDB Atlas, Mongoose
* **Frontend:** HTML, CSS, JavaScript
* **Tools:** npm, dotenv, Git

---

## Prerequisites

Before running this project, make sure you have:

* Node.js (v18+ recommended)
* npm (comes with Node.js)
* A MongoDB Atlas account (free tier works)

---

## Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/juliettemarzo/Thrive.git
cd Thrive/backend
```

---

### 2. Install dependencies

```bash
npm install
```

---

### 3. Set up environment variables

Create a `.env` file in the `backend` folder:

```bash
touch .env
```

Add the following:

```env
MONGO_URI=your_mongodb_atlas_connection_string
PORT=8080
```

⚠️ Make sure your IP address is whitelisted in MongoDB Atlas under **Network Access**.

---

### 4. Run the server

```bash
node server.js
```

You should see:

```text
Server running on http://localhost:8080
Connected to MongoDB
```

---

## Using the App

Open your browser and navigate to one of the following:

* Signup page: `http://localhost:8080/signup.html`
* Login page: `http://localhost:8080/login.html`

The frontend is served statically from the `public` folder.

---

## Project Structure

```text
Thrive/
├── backend/
│   ├── models/
│   ├── routes/
│   ├── services/
│   ├── server.js
│   ├── package.json
│   └── .env (not committed)
├── public/
│   ├── signup.html
│   ├── login.html
│   └── css/
└── README.md
```

---

## Notes

* The `.env` file is intentionally excluded from version control.
* Anyone cloning this repo must create their own `.env` file.
* If MongoDB connection fails, check your Atlas IP whitelist and connection string.
