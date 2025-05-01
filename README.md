# 💼 MERN Finance Dashboard App

A modern finance analytics and reporting web application built using the MERN stack, providing dynamic dashboards, predictive financial modeling, and RESTful APIs. Designed with scalability and developer productivity in mind.

---

## 📚 Table of Contents

- [Overview](#-overview)
- [Architecture](#-architecture)
- [Tech Stack](#-tech-stack)
- [Project Structure](#-project-structure)
- [Installation](#-installation)
- [Environment Variables](#-environment-variables)
- [Running the App](#-running-the-app)
- [API Documentation](#-api-documentation)
- [Machine Learning Integration](#-machine-learning-integration)
- [Frontend Features](#-frontend-features)
- [Deployment](#-deployment)
- [Security Notes](#-security-notes)
- [Screenshots](#-screenshots)
- [Contributing](#-contributing)
- [License](#-license)

---

## 🧩 Overview

This full-stack finance dashboard helps visualize, analyze, and predict financial performance using:

- RESTful API (Node.js + Express)
- MongoDB for persistent storage
- Regression-js for simple ML-based trend forecasting
- Vite + React + TypeScript for a blazing-fast UI
- Redux Toolkit & RTK Query for state and async data management

---

## 🏗 Architecture

![Image](https://github.com/user-attachments/assets/2adf0d6d-be00-45ab-a593-9ac198375430)*


---

## 🧰 Tech Stack

### 🔹 Frontend

| Tech            | Purpose                                     |
|-----------------|---------------------------------------------|
| Vite            | Fast development/build tool                 |
| React + TypeScript | Type-safe UI logic                      |
| Redux Toolkit   | State management (RTK + RTK Query)          |
| React Router    | SPA navigation                              |
| Material UI     | Component library                           |
| Recharts        | Data visualization                          |
| Heroicons       | Icon set                                    |

### 🔸 Backend

| Tech          | Purpose                                        |
|---------------|------------------------------------------------|
| Node.js       | JS Runtime                                     |
| Express.js    | Web framework                                  |
| Mongoose      | ODM for MongoDB                                |
| Regression-js | Simple linear regression (forecasting)         |
| MongoDB Atlas | Cloud database                                 |

---

## 🗂 Project Structure


📦 mern-finance-dashboard ├── client/ # Frontend source │ ├── src/ │ │ ├── assets/ # Static files & images │ │ ├── components/ # Shared components (charts, tables, UI) │ │ ├── scenes/ # Pages/views │ │ ├── state/ # Redux slices & API service │ │ └── App.tsx, main.tsx │ └── index.html ├── server/ # Backend source │ ├── data/ # Static dataset for seed/mocking │ ├── models/ # Mongoose models │ ├── routes/ # API routes (modular) │ ├── app.js, index.js # Entry points ├── .env.local # Environment variables ├── Dockerfile / fly.toml # Deployment configuration └── README.md


---

## 🧱 Installation

```bash
git clone https://github.com/yourusername/mern-finance-dashboard.git
cd mern-finance-dashboard


# Install client dependencies

cd client
npm install

# Install server dependencies

cd ../server
npm install


🔐 Environment Variables
Create .env.local in the server folder:

MONGO_URL=mongodb+srv://<username>:<password>@cluster0.brjd0da.mongodb.net/
PORT=5000

▶️ Running the App
Start Backend

cd server
npm run dev

Start Frontend

cd client
npm run dev

The app will be accessible at: http://localhost:5173


## 🧠 Machine Learning Integration
The backend uses regression-js to compute linear regression forecasts.

Model is trained on numerical transaction data (e.g., time vs. revenue).

Results are returned via /api/forecast.

import regression from 'regression';
const result = regression.linear([[0, 10], [1, 20], [2, 30]]);


🖼 Frontend Features
📊 Recharts-based financial graphs (Line, Bar, Pie)

💻 SPA with protected routes and scene-based UI

🔄 Asynchronous API integration with RTK Query

💡 Dark/Light MUI theming

📁 Modular Redux slice structure

🚀 Deployment
Frontend on Fly.io

flyctl launch
flyctl deploy

📫 Contact
Asma Laaribi
📧 Email: asmalaaribi@outlook.com
🌍 Portfolio: https://asmalaaribii.wixsite.com/portfolio






