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
git clone https://github.com/SauravF023/Movie-Booking-System-MernStack.git
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
# 🌐 Database
MONGODB_URI=mongodb://localhost:27017/quickshow
 
# 🔐 Clerk Authentication
CLERK_PUBLISHABLE_KEY=your-clerk-publishable-key
CLERK_SECRET_KEY=your-clerk-secret-key
 
# ⚙️ Inngest Event Scheduling
INNGEST_EVENT_KEY=your-inngest-event-key
INNGEST_SIGNING_KEY=your-inngest-signing-key
 
# 🎬 TMDB API (for movie data)
TMDB_API_KEY=your-tmdb-api-key
 
# 💳 Stripe Payment Integration
STRIPE_PUBLISHABLE_KEY=your-stripe-publishable-key
STRIPE_SECRET_KEY=your-stripe-secret-key
STRIPE_WEBHOOK_SECRET=your-stripe-webhook-secret
 
# 📧 Email Notifications (Nodemailer or similar SMTP setup)
SENDER_EMAIL=your-sender@example.com
SMTP_USER=your-smtp-username
SMTP_PASS=your-smtp-password

```

### Client (.env)

```env
# 💱 Currency Symbol
VITE_CURRENCY=$

# 🔐 Clerk Authentication (Public Key for Frontend)
VITE_CLERK_PUBLISHABLE_KEY=your-clerk-publishable-key

# 🌐 Base API URL (Proxy to Backend)
VITE_BASE_URL=http://localhost:3000

# 🎞️ TMDB Image Base URL
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
  
## Deployment
The application is configured for deployment on Vercel with the included vercel.json files.

Deploy to Vercel:

# Install Vercel CLI
npm i -g vercel

# Deploy
vercel --prod
Contributing
Fork the repository
Create a feature branch (git checkout -b feature/amazing-feature)
Commit your changes (git commit -m 'Add some amazing feature')
Push to the branch (git push origin feature/amazing-feature)
Open a Pull Request
Development Guidelines
Follow the existing code style and conventions
Write meaningful commit messages
Add tests for new features
Update documentation as needed
Ensure all tests pass before submitting PR

---

## 👨‍💻 Author

**Saurav Mishra**

If you found this project helpful, consider giving it a ⭐ on GitHub!
