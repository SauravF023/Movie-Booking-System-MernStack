# Movie-Booking-System-MernStack
A full-stack Movie Booking System built using the MERN stack (MongoDB, Express.js, React, Node.js) with seat selection, snack &amp; parking add-ons, QR-based ticket verification, and production deployment on Vercel &amp; Render.

🌟 Overview

QuickShow is a production-ready, full-stack movie ticket booking application built on the MERN stack. It lets users browse real-time movie catalogs powered by the TMDB API, pick seats interactively, pay securely via Stripe, and receive booking confirmations by email — all within a fast, mobile-first interface.

Administrators get a dedicated dashboard to manage shows, monitor bookings, handle movie listings, and view revenue analytics — no separate backend tool needed.

Why QuickShow?

ProblemQuickShow's SolutionFinding movies + booking in one placeUnified discovery-to-checkout flowReal-time seat availabilityLive seat-map with lock mechanismSecure paymentsStripe with webhook verificationAsync notificationsInngest background jobs for emailMedia management at scaleCloudinary for posters & thumbnailsAuth without the boilerplateClerk handles sign-up, login, sessions.

🛠 Tech Stack

Frontend (/client)

TechnologyVersionPurposeReact19UI libraryViteLatestBuild tool & dev serverTailwind CSSv4Utility-first stylingClerkLatestAuthentication & user managementStripe.jsLatestClient-side payment elementsReact Router DOMv6+Client-side routingAxios / Fetch-HTTP requests to backend

Backend (/server)

TechnologyVersionPurposeNode.jsv18+JavaScript runtimeExpressv4REST API frameworkMongoDBAtlasNoSQL databaseMongooseLatestODM for MongoDBClerk SDKLatestServer-side auth verificationStripeLatestPayment intent & webhooksInngestLatestBackground job schedulingNodemailerLatestTransactional email via SMTPTMDB APIv3Movie metadata & postersCloudinaryLatestImage/media managementNodemonLatestDev auto-restart


✨ Features

🎟️ User Features


Authentication — Sign up, log in, and manage sessions via Clerk (supports OAuth)
Movie Discovery — Browse trending, upcoming, and now-playing movies via TMDB API
Search & Filter — Filter movies by genre, rating, and release date
Movie Detail Pages — Full details: synopsis, cast, ratings, trailers
Interactive Seat Selection — Visual theater seat map with live availability
Secure Checkout — Stripe-powered payment flow with 3D Secure support
Booking Confirmation — Automated email confirmation after successful payment
My Bookings — Dashboard to view and manage personal booking history
Favorites — Save and revisit favourite movies


👨‍💼 Admin Features


Admin Dashboard — At-a-glance revenue, booking counts, and trends
Show Management — Create, update, and delete movie shows
Movie Management — Add movies with metadata, posters, and media
Booking Overview — View and update all user bookings system-wide
Theater Configuration — Set up theater layouts and seat arrangements
Analytics — Revenue reporting and occupancy insights


⚙️ Technical Features


Background Jobs — Inngest handles async tasks like email dispatch and seat release on payment timeout
Webhook Handling — Stripe webhook signature verification for secure payment confirmation
Image Optimization — Cloudinary transforms and delivers optimized movie poster images
Responsive Design — Mobile-first Tailwind CSS layout that works on all devices
Input Validation — Server-side schema validation via Mongoose
Error Handling — Centralized error middleware with meaningful HTTP responses
CORS & Security — Proper CORS configuration and environment-based secrets
Vercel Deployment — Both client and server configured for zero-config Vercel deploys


