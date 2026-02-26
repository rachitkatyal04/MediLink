# MediLink 🏥

A full-stack doctor appointment booking platform built with the MERN stack. MediLink connects patients with healthcare professionals, enabling seamless appointment scheduling, management, and online payments.

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Prerequisites](#prerequisites)
- [Installation](#installation)
- [Environment Variables](#environment-variables)
- [Running the Application](#running-the-application)
- [License](#license)

## ✨ Features

### Patient Portal (Frontend)

- User registration and authentication
- Browse doctors by specialty
- Book appointments with preferred doctors
- View and manage appointments
- Online payment integration (Razorpay & Stripe)
- User profile management
- Responsive design

### Admin & Doctor Dashboard

- Admin authentication
- Doctor management (add, edit, remove)
- Appointment management
- Dashboard analytics
- Doctor profile management

### Backend API

- RESTful API architecture
- JWT-based authentication
- Secure password hashing with bcrypt
- Image upload with Cloudinary
- MongoDB database integration

## 🛠️ Tech Stack

**Frontend & Admin:**

- React 18/19
- Vite
- Tailwind CSS
- React Router DOM
- Axios
- React Toastify

**Backend:**

- Node.js
- Express.js
- MongoDB with Mongoose
- JWT Authentication
- Cloudinary (Image Storage)
- Razorpay & Stripe (Payments)

## 📁 Project Structure

```
MediLink/
├── frontend/          # Patient-facing web application
├── admin/             # Admin & Doctor dashboard
└── backend/           # REST API server
    ├── models/        # MongoDB schemas
    ├── routes/        # API routes
    ├── controllers/   # Route handlers
    ├── middlewares/   # Auth & other middlewares
    └── config/        # Database & cloud config
```

## 📋 Prerequisites

- Node.js (v18 or higher)
- MongoDB Atlas account or local MongoDB
- Cloudinary account
- Razorpay/Stripe account (for payments)

## 🚀 Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/rachitkatyal04/MediLink.git
   cd MediLink
   ```

2. **Install Backend Dependencies**

   ```bash
   cd backend
   npm install
   ```

3. **Install Frontend Dependencies**

   ```bash
   cd frontend
   npm install
   ```

4. **Install Admin Dependencies**
   ```bash
   cd admin
   npm install
   ```

## 🔐 Environment Variables

Create a `.env` file in the `backend` folder with the following variables:

```env
# App Config
CURRENCY=INR
JWT_SECRET=your_jwt_secret_key

# Admin Credentials
ADMIN_EMAIL=admin@example.com
ADMIN_PASSWORD=your_admin_password

# MongoDB (Required)
MONGODB_URI=your_mongodb_connection_string

# Cloudinary (Required)
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_cloudinary_api_key
CLOUDINARY_SECRET_KEY=your_cloudinary_secret_key

# Razorpay (Optional)
RAZORPAY_KEY_ID=your_razorpay_key_id
RAZORPAY_KEY_SECRET=your_razorpay_key_secret

# Stripe (Optional)
STRIPE_SECRET_KEY=your_stripe_secret_key
```

## ▶️ Running the Application

1. **Start the Backend Server**

   ```bash
   cd backend
   npm run dev
   ```

   Server runs on `http://localhost:4000`

2. **Start the Frontend**

   ```bash
   cd frontend
   npm run dev
   ```

   Frontend runs on `http://localhost:5173`

3. **Start the Admin Panel**
   ```bash
   cd admin
   npm run dev
   ```
   Admin panel runs on `http://localhost:5174`

## 📄 License

This project is licensed under the ISC License.
