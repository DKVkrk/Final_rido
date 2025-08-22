# 🚗 Rido - Ride-Sharing Platform

<div align="center">
  <img src="rido/public/logo rido.png" alt="Rido Logo" width="200"/>
  
  [![React](https://img.shields.io/badge/React-18.2.0-blue.svg)](https://reactjs.org/)
  [![Node.js](https://img.shields.io/badge/Node.js-Express-green.svg)](https://nodejs.org/)
  [![MongoDB](https://img.shields.io/badge/MongoDB-Mongoose-orange.svg)](https://mongodb.com/)
  [![Socket.io](https://img.shields.io/badge/Socket.io-Real--time-red.svg)](https://socket.io/)
  [![License](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE)
</div>

## 📖 Overview

**Rido** is a modern, full-stack ride-sharing platform that connects riders with drivers in real-time. Built with cutting-edge technologies, it provides a seamless experience for both passengers and drivers with features like real-time tracking, secure payments, and intelligent ride matching.

## ✨ Features

### 🚀 For Riders
- **Real-time Ride Booking**: Request rides with instant driver matching
- **Live Tracking**: Track your driver's location in real-time
- **Multiple Payment Options**: Secure payment processing with multiple gateways
- **Ride History**: View and manage your past rides
- **Rating System**: Rate your driver after each ride

### 🚗 For Drivers
- **Flexible Schedule**: Drive when you want, earn what you need
- **Route Optimization**: Smart navigation and route suggestions
- **Ride Requests**: Accept or decline ride requests
- **Profile Management**: Manage your vehicle and personal information


### 🔧 Platform Features
- **Real-time Communication**: WebSocket-based live updates
- **Geolocation Services**: Leaflet maps integration for accurate navigation
- **Authentication System**: Secure JWT-based authentication
- **Email Verification**: Complete email verification workflow
- **Responsive Design**: Mobile-first responsive UI
- **Business Solutions**: Corporate ride-sharing options

## 🛠️ Tech Stack

### Frontend
- **React 18** - Modern UI framework
- **Vite** - Fast build tool and dev server
- **React Router DOM** - Client-side routing
- **Socket.io Client** - Real-time communication
- **React Leaflet** - Interactive maps
- **Axios** - HTTP client
- **React Hot Toast** - User notifications
- **React Icons** - Icon library

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - MongoDB ODM
- **Socket.io** - Real-time bidirectional communication
- **JWT** - Authentication tokens
- **Bcryptjs** - Password hashing
- **Multer** - File upload handling
- **Nodemailer** - Email services
- **Cloudinary** - Image storage

### External Services
- **Leaflet Maps** - Geolocation and navigation
- **Google OAuth** - Social authentication
- **Stripe/Payment Gateway** - Payment processing

## 🚀 Quick Start

### Prerequisites
- Node.js (v16 or higher)
- MongoDB
- npm or yarn

### Installation

1. **Clone the repository**
   ```bash
   git clone https://github.com/yourusername/rido.git
   cd rido
   ```

2. **Install Frontend Dependencies**
   ```bash
   cd rido
   npm install
   ```

3. **Install Backend Dependencies**
   ```bash
   cd ../ridoBackend
   npm install
   ```

4. **Environment Setup**
   
   Create `.env` files in both frontend and backend directories:
   
   **Frontend (.env)**
   ```env
   VITE_API_URL=http://localhost:5000/api
   VITE_GOOGLE_MAPS_API_KEY=your_google_maps_api_key
   ```
   
   **Backend (.env)**
   ```env
   PORT=5000
   MONGODB_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   JWT_REFRESH_SECRET=your_refresh_token_secret
   GOOGLE_CLIENT_ID=your_google_client_id
   GOOGLE_CLIENT_SECRET=your_google_client_secret
   CLOUDINARY_CLOUD_NAME=your_cloudinary_name
   CLOUDINARY_API_KEY=your_cloudinary_key
   CLOUDINARY_API_SECRET=your_cloudinary_secret
   EMAIL_USER=your_email
   EMAIL_PASS=your_email_password
   FRONTEND_URL=http://localhost:5173
   ```

5. **Start the Development Servers**

   **Backend (Terminal 1)**
   ```bash
   cd ridoBackend
   npm run dev
   ```

   **Frontend (Terminal 2)**
   ```bash
   cd rido
   npm run dev
   ```

6. **Access the Application**
   - Frontend: http://localhost:5173
   - Backend API: http://localhost:5000

## 📁 Project Structure

```
final_rido/
├── rido/                    # Frontend React Application
│   ├── src/
│   │   ├── components/      # Reusable UI components
│   │   ├── pages/          # Page components
│   │   ├── styles/         # CSS stylesheets
│   │   ├── utils/          # Utility functions
│   │   └── common/         # Shared configurations
│   ├── public/             # Static assets
│   └── package.json
├── ridoBackend/            # Backend Node.js Application
│   ├── controllers/        # Route controllers
│   ├── models/            # Database models
│   ├── routes/            # API routes
│   ├── middleware/        # Custom middleware
│   ├── config/            # Configuration files
│   ├── utils/             # Utility functions
│   └── server.js          # Main server file
└── README.md
```

## 🔧 API Endpoints

### Authentication
- `POST /api/auth/register` - User registration
- `POST /api/auth/login` - User login
- `POST /api/auth/forgot-password` - Password reset
- `POST /api/auth/verify-email` - Email verification

### Rides
- `POST /api/rides/request` - Request a new ride
- `GET /api/rides/history` - Get ride history
- `PUT /api/rides/:id/status` - Update ride status
- `POST /api/rides/:id/rate` - Rate a ride

### Drivers
- `POST /api/drivers/register` - Driver registration
- `PUT /api/drivers/location` - Update driver location
- `GET /api/drivers/nearby` - Find nearby drivers

## 🎯 Key Features Implementation

### Real-time Ride Tracking
- WebSocket connections for live location updates
- Google Maps integration for route visualization
- Real-time driver-rider communication
- Real time sending images of live location between rider and driver

### Secure Authentication
- JWT-based authentication with refresh tokens
- Google OAuth integration
- Email verification system
- Password reset functionality

### Payment Integration
- Multiple payment gateway support
- Secure transaction processing
- Payment history tracking

## 🤝 Contributing

We welcome contributions! Please follow these steps:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 🆘 Support

If you encounter any issues or have questions:

- 📧 Email: support@rido.com
- 💬 Chat: Use the built-in chatbot in the application
- 📖 Documentation: Check the Help section in the app

## 🙏 Acknowledgments

- Google Maps API for location services
- Socket.io for real-time communication
- React community for excellent documentation
- All contributors who helped build Rido

---

<div align="center">
  <p>Made with ❤️ by the Rido Team</p>
  <p>🚗 Connecting people, one ride at a time 🚗</p>
</div> 