# Stayly - Modern Listing & Booking Platform

🚀 Live Demo: https://stayly.onrender.com

Stayly is a full-stack web application that enables users to discover, create, and manage property listings with integrated maps, image uploads, and user-generated reviews. The platform focuses on clean UI/UX, scalable backend architecture, and real-world application features.

---

## ✨ Features

### 🔐 Authentication & Authorization
- Secure user signup & signin using Passport.js
- Session-based authentication with MongoDB store
- Protected routes with ownership-based access control
- Redirect-after-login functionality

### 🏡 Listings
- Full CRUD operations (Create, Read, Update, Delete)
- Image upload with Cloudinary (cloud storage)
- Location-based listings with geocoding
- Server-side validation using Joi

### 🗺️ Map Integration
- Interactive maps using Mapbox GL JS
- Location-based geocoding for listing coordinates
- Custom markers with popup details
- Map display on listing pages

### ⭐ Reviews System
- Add and delete reviews with ratings
- User-specific permissions
- Star-based rating UI
- Cascade delete when listing is removed

### 🎯 UI & UX Features
- Scrollable category navigation with arrow controls
- Advanced filter modal
- Flash messages with auto-dismiss
- Responsive mobile-first design
- Custom form validation UI

---

## 🛠️ Tech Stack

### Frontend
- EJS (with ejs-mate layouts)
- Bootstrap 5
- Font Awesome, Bootstrap Icons, Boxicons
- CSS
- Vanilla JavaScript

### Backend
- Node.js
- Express.js (MVC architecture)

### Database
- MongoDB (Mongoose)

### Authentication
- Passport.js
- passport-local-mongoose

### Cloud & APIs
- Cloudinary (Image Upload & Storage)
- Mapbox (Maps & Geocoding)

---

## 📂 Project Structure

```text
stayly/
├── controllers/        # Route logic
├── models/             # Mongoose schemas
├── routes/             # Express routers
├── views/              # EJS templates
│   ├── layouts/        # Main boilerplate layout
│   ├── includes/       # Navbar, footer, flash messages
│   ├── listings/       # Index, show, new, edit views
│   └── user/           # Signup, signin views
├── public/             # Static assets
│   ├── css/            # Stylesheets
│   └── js/             # Client-side scripts
├── utils/              # Helper utilities
├── middleware.js       # Custom middleware
├── schema.js           # Joi validation schemas
├── cloudConfig.js      # Cloudinary storage setup
├── init/               # Seed data
└── app.js              # Main server file
```

---

## ⚙️ Installation & Setup

### 1️⃣ Clone repository

```bash
git clone https://github.com/your-username/stayly.git
cd stayly
```

### 2️⃣ Install dependencies

```bash
npm install
```

### 3️⃣ Create `.env`

```
ATLASDB_URL=your_mongodb_atlas_url
SESSION_SECRET=your_session_secret

CLOUD_NAME=your_cloudinary_cloud_name
CLOUD_API_KEY=your_cloudinary_api_key
CLOUD_API_SECRET=your_cloudinary_api_secret

MAP_TOKEN=your_mapbox_access_token
```

### 4️⃣ Run locally

```bash
node app.js
```

Visit:

```
http://localhost:8080
```

---

## 🧠 Key Concepts Used

* MVC Architecture
* RESTful Routing
* Middleware for authentication and validation
* GeoJSON and geospatial data
* File upload handling with Multer and Cloudinary
* Session management with MongoStore
* Error handling with Express middleware
* Responsive UI design

---

## 📸 Screenshots

![alt text](image.png)

---

## 🚀 Planned Improvements

* 🔍 Search and filtering functionality (backend integration)
* 🛎️ Booking system with availability management
* 👤 User dashboard (bookings, listings, and activity)
* ❤️ Wishlist / favorites system
* 📍 Nearby listings using MongoDB geospatial queries
* 🌍 Country-based listing pages with map view
* 💳 Payment integration

---

## 👨‍💻 Author

**Nur Hasin Ahammad** </br>
Full Stack Developer | CSE Undergraduate

---

## ⭐ Acknowledgements

* Bootstrap
* MongoDB
* Cloudinary
* Mapbox
* Passport.js

---

## 📜 License

This project is licensed under the MIT License.