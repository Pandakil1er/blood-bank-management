# Blood Bank Management System

## Overview
The **Blood Bank Management System** is a full-stack web application designed to streamline the process of blood donation and distribution. It enables hospitals, blood banks, donors, and administrators to efficiently manage blood inventory, track availability, and handle requests in real-time.

## Features
- **Role-Based Access Control (RBAC)**: Secure authentication with JWT for admins, hospitals, donors, and blood banks.
- **Real-Time Inventory Management**: Tracks availability across **8 blood groups** (A+, A-, B+, B-, AB+, AB-, O+, O-).
- **Donor Registration & Management**: Allows users to register as donors and track their donation history.
- **Hospital Request System**: Hospitals can request blood based on availability.
- **Admin Dashboard**: Provides an overview of system statistics and operations.
- **Responsive UI**: Built using React.js, ensuring a seamless experience across devices.
- **RESTful API**: Secure and efficient API endpoints for all operations.

## Tech Stack
- **Frontend**: React.js, Redux Toolkit, React Router, Axios, React Toastify
- **Backend**: Node.js, Express.js
- **Database**: MongoDB, Mongoose
- **Security**: JWT Authentication, bcrypt for password hashing

## Installation & Setup
### Prerequisites
Ensure you have the following installed:
- Node.js (v16+)
- MongoDB

### Steps
1. Clone the repository:
   ```sh
   git clone https://github.com/AnkurDhattarwal/blood-bank-management.git
   cd blood-bank-management
   ```
2. Install dependencies:
   ```sh
   npm install
   ```
3. Set up environment variables:
   - Create a `.env` file in the root directory and add:
     ```sh
     MONGO_URI=your_mongodb_connection_string
     JWT_SECRET=your_secret_key
     ```
4. Start the backend server:
   ```sh
   npm run server
   ```
5. Navigate to the `client` folder and start the frontend:
   ```sh
   cd client
   npm start
   ```
6. Open `http://localhost:3000` in your browser.

## API Endpoints
- **User Authentication**
  - `POST /api/auth/register` - Register a new user
  - `POST /api/auth/login` - Login user
- **Blood Inventory**
  - `GET /api/blood` - Get blood availability
  - `POST /api/blood/donate` - Record a blood donation
  - `POST /api/blood/request` - Request blood
- **Admin Controls**
  - `GET /api/admin/stats` - Get system analytics

## Future Enhancements
- SMS & Email notifications for donation camps.
- AI-powered blood demand prediction.
- Blockchain-based donor verification.



