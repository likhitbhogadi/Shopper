# SHOPPER - E-Commerce Platform for IIIT Community

A full-stack e-commerce platform built specifically for the IIIT community that enables users to buy and sell products within the campus network.

## Features

- **User Authentication**
  - Email-based registration (restricted to IIIT domain)
  - Secure login with reCAPTCHA verification
  - JWT-based authentication
  - Password hashing for security

- **Product Management**
  - Upload products with details (name, price, category, description)
  - Browse available products
  - Filter products by category
  - Search products by name

- **Shopping Features**
  - Add products to cart
  - View product details
  - Secure checkout process
  - OTP-based delivery verification

- **Order Management**
  - View order history (bought/sold items)
  - Track pending deliveries
  - Verify deliveries using OTP

- **User Profile**
  - View and edit personal details
  - Manage product listings
  - Track order history

- **Support System**
  - AI-powered chat support
  - Persistent chat history
  - Quick responses for common queries

## Tech Stack

### Frontend
- React + Vite
- React Router for navigation
- Axios for API requests
- React-Toastify for notifications
- CSS for styling

### Backend
- Node.js + Express
- MongoDB for database
- JWT for authentication
- bcrypt for password hashing
- Google reCAPTCHA integration
- Gemini AI for chat support

## Getting Started - how to run locally

### Environment Setup

1. Create a `.env` file in the backend directory with the following variables:
```
PORT=3001
MONGO_STRING=your_mongodb_connection_string
FRONTEND_URL=http://localhost:5173
SESSION_SECRET=your_session_secret
RECAPTCHA_SECRET_KEY=your_recaptcha_secret_key
GEMINI_API_KEY=your_gemini_api_key
```

2. Create a `.env` file in the frontend directory with:
```
VITE_RECAPTCHA_SITE_KEY=your_recaptcha_site_key
```

3. Replace the placeholder values with your actual credentials:
  - Get reCAPTCHA keys from [Google reCAPTCHA](https://www.google.com/recaptcha/admin)
  - Get a Gemini API key from [Google AI Studio](https://ai.google.dev/)
  - Set up a MongoDB database (local or Atlas)

### Backend Setup

1. Navigate to the backend directory:
```bash
cd backend
```

2. Install dependencies:
```bash
npm install
```

3. Start the backend server:
```bash
npm start
```
The server should start running on port 3001.

### Frontend Setup

1. Open a new terminal and navigate to the frontend directory:
```bash
cd frontend
```

2. Install dependencies:
```bash
npm install
```

3. Start the development server:
```bash
npm run dev
```
The frontend application should start running on port 5173.

### Access the Application

1. Open your browser and navigate to:
```
http://localhost:5173
```

2. Register a new account using an email with the IIIT domain (e.g., example@iiit.ac.in)
3. Log in with your credentials
4. Start exploring the platform!

### Prerequisites
- Node.js
- MongoDB
- npm or yarn

### Installation

1. Clone the repository
```bash
git clone [repository-url]