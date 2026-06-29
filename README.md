# 🎬 QuickShow – MERN Movie Ticket Booking System

A modern **full-stack movie ticket booking platform** built using the **MERN Stack**, enabling users to discover movies, book tickets with interactive seat selection, make secure online payments, and manage bookings through an intuitive interface. The platform also includes a powerful **Admin Dashboard** for managing movies, shows, and bookings.

---

## 🚀 Features

### 👤 User Features

* 🔐 Secure authentication using **Clerk**
* 🎬 Browse trending and upcoming movies (TMDB API)
* 🔍 Search movies with detailed information
* 🎟️ Interactive seat selection
* 🍿 Snack add-ons during booking
* 💳 Secure online payments using **Stripe**
* 📄 QR code ticket generation with PDF download
* 📧 Email booking confirmations
* 📱 Fully responsive design

### 👨‍💼 Admin Features

* 📊 Admin dashboard
* 🎥 Manage movies and shows
* 🎫 View and manage bookings
* 💰 Monitor booking analytics
* ✔️ Ticket verification system

---

## 🛠️ Tech Stack

| Category        | Technologies                 |
| --------------- | ---------------------------- |
| Frontend        | React.js, Tailwind CSS, Vite |
| Backend         | Node.js, Express.js          |
| Database        | MongoDB Atlas                |
| Authentication  | Clerk                        |
| Payments        | Stripe                       |
| Movie Data      | TMDB API                     |
| Background Jobs | Inngest                      |
| Deployment      | Vercel, Render               |
| Others          | JWT, QR Code, jsPDF          |

---

## 📂 Project Structure

```text
QuickShow
├── client
│   ├── src
│   ├── public
│   └── package.json
│
├── server
│   ├── controllers
│   ├── routes
│   ├── models
│   ├── middleware
│   ├── configs
│   ├── inngest
│   └── package.json
│
└── README.md
```

---

## ⚙️ Installation

### 1️⃣ Clone Repository

```bash
git clone https://github.com/elyse502/QuickShow.git
cd QuickShow
```

### 2️⃣ Install Dependencies

Server

```bash
cd server
npm install
```

Client

```bash
cd ../client
npm install
```

---

## 🔑 Environment Variables

### Server (.env)

```env
MONGODB_URI=

CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

INNGEST_EVENT_KEY=
INNGEST_SIGNING_KEY=

TMDB_API_KEY=

STRIPE_PUBLISHABLE_KEY=
STRIPE_SECRET_KEY=
STRIPE_WEBHOOK_SECRET=

SENDER_EMAIL=
SMTP_USER=
SMTP_PASS=
```

### Client (.env)

```env
VITE_CURRENCY=$

VITE_CLERK_PUBLISHABLE_KEY=

VITE_BASE_URL=http://localhost:3000

VITE_TMDB_IMAGE_BASE_URL=https://image.tmdb.org/t/p/original
```

---

## ▶️ Running the Project

### Backend

```bash
cd server
npm run dev
```

### Frontend

```bash
cd client
npm run dev
```

---

## 🌐 Application URLs

| Service  | URL                   |
| -------- | --------------------- |
| Frontend | http://localhost:5173 |
| Backend  | http://localhost:5000 |

---

## 📡 REST API

### Authentication

```
POST /api/users/register
POST /api/users/login
GET  /api/users/profile
PUT  /api/users/profile
```

### Movies & Shows

```
GET    /api/shows
GET    /api/shows/:id
POST   /api/admin/shows
PUT    /api/admin/shows/:id
DELETE /api/admin/shows/:id
```

### Bookings

```
POST /api/bookings
GET  /api/bookings/user
GET  /api/admin/bookings
PUT  /api/bookings/:id
```

### Payments

```
POST /api/bookings/create-payment-intent
POST /api/webhooks/stripe
```

---

## ✨ Highlights

* 🎬 Movie discovery powered by TMDB
* 🎟️ Interactive seat booking system
* 💳 Stripe payment integration
* 📄 QR code & PDF ticket generation
* 📧 Automated email notifications
* 🔐 Clerk authentication
* 📱 Fully responsive UI
* ☁️ Cloud deployment using Vercel & Render
* ⚡ Fast development with Vite
* 🛡️ Secure and scalable MERN architecture

---

## 👨‍💻 Author

**Saurav Mishra**

If you found this project helpful, consider giving it a ⭐ on GitHub!
