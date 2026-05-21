# 🎓 StudyNotion

<div align="center">

![StudyNotion Logo](./assets/logo.png)

**A Modern EdTech Platform for Students and Educators**

StudyNotion is a full-stack educational platform that provides an interactive and seamless learning experience where students can enroll in courses and instructors can create, manage, and monetize educational content.

[Features](#-features) •
[Tech Stack](#-tech-stack) •
[Architecture](#-architecture) •
[API Routes](#-api-routes) •
[Installation](#-installation--setup) •
[Contributing](#-contributing)

</div>

---

# 📖 Overview

StudyNotion is designed to simplify and improve online learning through an intuitive and scalable system.

The platform enables:

- 📚 Course creation and management
- 👨‍🏫 Instructor dashboards
- 👨‍🎓 Student enrollment
- 💳 Payment integration
- ⭐ Ratings and reviews
- ☁️ Media management
- 🔐 Authentication and authorization
- 📊 Learning analytics

The application follows a **Monolithic Architecture** and uses modern web technologies to deliver a responsive and smooth user experience.

---

# ✨ Features

## Student Features

- User Registration/Login
- OTP Verification
- Forgot Password functionality
- Browse all courses
- Wishlist management
- Add courses to cart
- Purchase courses
- Course progress tracking
- Course reviews and ratings
- Update profile settings

---

## Instructor Features

- Create courses
- Update courses
- Delete courses
- Add sections and subsections
- Upload videos and media
- View dashboard analytics
- View enrolled students
- Monitor course performance

---

## Future Admin Features

- Manage users
- Manage instructors
- Platform analytics
- Revenue insights
- Content moderation
- System management

---

# 🛠 Tech Stack

## Frontend Technologies

| Technology | Purpose |
|------------|----------|
| React.js | Frontend UI Development |
| Redux | State Management |
| Tailwind CSS | Styling |
| CSS | Additional Styling |
| Chart.js | Data Visualization |
| Figma | UI/UX Design |

---

## Backend Technologies

| Technology | Purpose |
|------------|----------|
| Node.js | Runtime Environment |
| Express.js | Backend Framework |
| MongoDB | Database |
| Cloudinary | Media Storage |
| JWT | Authentication |
| Razorpay | Payment Processing |

---

# 🏗 Architecture

StudyNotion uses a **Monolithic Architecture** where all services are managed within a unified application structure.

### Architecture Flow

```text
User
   ↓
Frontend (React)
   ↓
Backend API (Node + Express)
   ↓
Authentication Middleware
   ↓
Database (MongoDB)
   ↓
Cloudinary Storage
```

---

# 📂 Project Structure

```bash
StudyNotion/
│
├── client/
│   ├── src/
│   ├── components/
│   ├── pages/
│   ├── services/
│   └── redux/
│
├── server/
│   ├── controllers/
│   ├── routes/
│   ├── models/
│   ├── middleware/
│   ├── config/
│   └── utils/
│
├── assets/
├── README.md
└── package.json
```

---

# 🔐 Authentication Features

StudyNotion implements secure authentication with:

- JWT Authentication
- OTP Verification
- Password Reset
- Protected Routes
- Role-Based Access Control

Roles include:

- Student
- Instructor
- Admin (Future Scope)

---

# 📡 API Routes

## Authentication APIs

| Endpoint | Route |
|-----------|--------|
| Send OTP | `/api/v1/auth/sendotp` |
| Signup | `/api/v1/auth/signup` |
| Login | `/api/v1/auth/login` |
| Reset Password Token | `/api/v1/auth/reset-password-token` |
| Reset Password | `/api/v1/auth/reset-password` |

---

## Profile APIs

| Endpoint | Route |
|-----------|--------|
| Get User Details | `/api/v1/profile/getUserDetails` |
| Get Enrolled Courses | `/api/v1/profile/getEnrolledCourses` |
| Instructor Dashboard | `/api/v1/profile/instructorDashboard` |

---

## Course APIs

| Endpoint | Route |
|-----------|--------|
| Get All Courses | `/api/v1/course/getAllCourses` |
| Create Course | `/api/v1/course/createCourse` |
| Edit Course | `/api/v1/course/editCourse` |
| Delete Course | `/api/v1/course/deleteCourse` |
| Add Section | `/api/v1/course/addSection` |
| Add Subsection | `/api/v1/course/addSubSection` |
| Update Progress | `/api/v1/course/updateCourseProgress` |
| Create Rating | `/api/v1/course/createRating` |

---

## Payment APIs

| Endpoint | Route |
|-----------|--------|
| Capture Payment | `/api/v1/payment/capturePayment` |
| Verify Payment | `/api/v1/payment/verifyPayment` |
| Success Email | `/api/v1/payment/sendPaymentSuccessEmail` |

---

# 💳 Payment Integration

StudyNotion integrates **Razorpay** for secure payment handling.

Features:

- Course checkout
- Payment verification
- Purchase history
- Payment success emails

---

# ☁️ Media Management

Cloudinary is used for:

- Video uploads
- Course thumbnails
- Image optimization
- Document storage
- Media delivery

---

# 🚀 Installation & Setup

## Clone Repository

```bash
git clone https://github.com/yourusername/studynotion.git
```

Move into directory:

```bash
cd studynotion
```

Install dependencies:

### Frontend

```bash
cd client
npm install
```

### Backend

```bash
cd server
npm install
```

---

## Environment Variables

Create `.env` files.

### Backend .env

```env
PORT=5000

MONGODB_URL=

JWT_SECRET=

CLOUDINARY_NAME=
CLOUDINARY_API_KEY=
CLOUDINARY_API_SECRET=

RAZORPAY_KEY=
RAZORPAY_SECRET=

MAIL_HOST=
MAIL_USER=
MAIL_PASS=
```

---

## Start Application

### Start Backend

```bash
npm run dev
```

### Start Frontend

```bash
npm start
```

---

# 📷 Screenshots

Add screenshots here:

| Homepage | Dashboard |
|-----------|------------|
| Screenshot | Screenshot |

---

# 🔮 Future Enhancements

- AI-powered course recommendations
- Live classes
- Video conferencing
- Discussion forums
- Certificate generation
- Dark mode
- Mobile application
- Admin dashboard

---

# 🤝 Contributing

Contributions are welcome.

Steps:

1. Fork repository
2. Create feature branch

```bash
git checkout -b feature/NewFeature
```

3. Commit changes

```bash
git commit -m "Added new feature"
```

4. Push changes

```bash
git push origin feature/NewFeature
```

5. Create Pull Request

---

<div align="center">

Made with ❤️ by StudyNotion Team

</div>
