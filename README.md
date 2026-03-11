# StudyNotion – Full Stack Learning Management System

StudyNotion is a **full-stack Learning Management System (LMS)** that allows instructors to create and manage courses while enabling students to browse, purchase, and learn online courses seamlessly.

The platform provides **secure authentication, course management, video learning, progress tracking, and online payments** with a modern responsive UI.

---

# 🚀 Features

## 👨‍🎓 Student Features

### Authentication

* Sign up / Login with email verification
* JWT based authentication
* Password reset via email
* Secure password encryption

### Course Discovery

* Browse courses by category
* Search and filter courses
* View course details, ratings, and reviews
* Add courses to shopping cart

### Learning Experience

* Watch course lectures using video player
* Track lecture completion progress
* Course progress dashboard
* Download course completion certificate

### User Profile

* Update profile information
* Change password
* View enrolled courses
* Track purchase history

---

## 👨‍🏫 Instructor Features

### Course Management

* Create and publish courses
* Upload videos and documents
* Organize course sections and lectures
* Manage course status (Draft / Published)

### Dashboard & Analytics

* View student enrollments
* Track course revenue
* Monitor course performance
* Recent enrollment activity

### Content Management

* Upload course thumbnails
* Store media files using Cloudinary
* Categorize courses

---

# 🛠️ Tech Stack

## Frontend

* React.js
* Redux Toolkit
* React Router
* Tailwind CSS
* Axios
* React Hot Toast
* React Icons

## Backend

* Node.js
* Express.js
* MongoDB
* Mongoose
* JWT Authentication
* Bcrypt
* Nodemailer
* Cloudinary

## Payment Integration

* Razorpay

---

# 📁 Project Structure

```
studyNotion/
│
├── public/                 # Static public assets
│
├── src/                    # Frontend source code
│   ├── assets/             # Images and static files
│   ├── components/         # Reusable React components
│   ├── pages/              # Page components
│   ├── hooks/              # Custom React hooks
│   ├── services/           # API service functions
│   ├── slices/             # Redux slices
│   ├── reducer/            # Redux reducers
│   ├── utils/              # Utility functions
│   └── data/               # Static data files
│
├── server/                 # Backend source code
│   ├── config/             # Configuration files
│   ├── controllers/        # Request handlers
│   ├── middleware/         # Custom middleware
│   ├── models/             # Mongoose database models
│   ├── routes/             # API routes
│   ├── mail/               # Email templates & services
│   └── utils/              # Utility functions
│
├── .env.example            # Environment variables template
├── index.js                # Backend entry point
├── package.json            # Project dependencies
└── README.md
```

---

# ⚙️ Installation

## Prerequisites

* Node.js (v18+)
* MongoDB
* npm or yarn

---

## Clone the Repository

```bash
git clone <repository-url>
cd studyNotion
```

---

## Install Dependencies

Frontend:

```bash
npm install
```

Backend:

```bash
cd server
npm install
```

---

# 🔧 Environment Variables

Create a **.env** file inside the `server` folder.

### Backend `.env`

```
# Database
MONGODB_URL=your_mongodb_connection_string

# JWT
JWT_SECRET=your_jwt_secret

# Email Configuration
MAIL_HOST=smtp.gmail.com
MAIL_USER=your_email@gmail.com
MAIL_PASS=your_app_password

# Cloudinary
CLOUDINARY_NAME=your_cloudinary_name
CLOUDINARY_API_KEY=your_api_key
CLOUDINARY_API_SECRET=your_api_secret
FOLDER=studynotion

# Razorpay
RAZORPAY_KEY=your_key
RAZORPAY_SECRET=your_secret

# Server
PORT=5000
NODE_ENV=development
```

### Frontend `.env`

```
VITE_BACKEND_URL=http://localhost:5000/api/v1
VITE_RAZORPAY_KEY=your_razorpay_key
```

---

# ▶️ Running the Project

Run both frontend and backend:

```bash
npm run dev
```

Or run separately:

Frontend

```bash
npm run client
```

Backend

```bash
npm run server
```

---

# 📡 API Endpoints

## Authentication

```
POST /api/v1/auth/signup
POST /api/v1/auth/login
POST /api/v1/auth/forgot-password
```

## Courses

```
GET  /api/v1/course/showAllCategories
POST /api/v1/course/createCourse
GET  /api/v1/course/getCourseDetails
POST /api/v1/course/createRating
```

## Payments

```
POST /api/v1/payment/capturePayment
POST /api/v1/payment/verifySignature
```

---

# 🔒 Security Features

* JWT based authentication
* Password hashing using bcrypt
* Input validation and sanitization
* CORS protection
* Secure payment verification
* Protected API routes

---

# 🚀 Deployment

## Frontend

Deploy using:

* Vercel
* Netlify

Steps:

```
npm run build
Deploy the dist folder
```

## Backend

Deploy using:

* Render
* Railway

Steps:

1. Deploy `server` folder
2. Set environment variables
3. Update frontend API URL

---

# 🤝 Contributing

1. Fork the repository
2. Create a feature branch
3. Commit your changes
4. Push to the branch
5. Create a Pull Request

---

# 📄 License

This project is licensed under the MIT License.

---

# 🙏 Acknowledgements

* React Team
* Tailwind CSS
* MongoDB
* Razorpay
* Cloudinary
