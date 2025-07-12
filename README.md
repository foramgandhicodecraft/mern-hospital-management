#  MERN Hospital Management System

A full-stack hospital management web app built using the **MERN stack (MongoDB, Express, React, Node.js)**. This system allows users to book appointments, doctors to manage their schedules, and admins to handle doctor listings and appointments securely.

---


##  Features

### 👤 User
- Sign up / Login using secure JWT-based auth
- Browse and filter doctors by specialty
- Book and cancel appointments
- View profile and appointment history

### 🩺 Doctor
- Secure login
- View appointments
- Cancel or complete appointments
- Update profile
- Dashboard showing earnings and patient count

### 🛠️ Admin
- Admin login (secured via env credentials)
- Add doctors with image upload (via Cloudinary)
- View, manage, and cancel any appointment
- Toggle doctor availability
- Dashboard analytics

---

##  Tech Stack

| Technology | Usage |
|------------|--------|
| **MongoDB** + **Mongoose** | Database and schema definitions |
| **Express.js** | Backend API routing |
| **React.js** + **Vite** | Frontend interfaces |
| **Node.js** | Server runtime |
| **JWT** | Secure authentication |
| **bcrypt** | Password hashing |
| **Cloudinary** | Doctor image upload |
| **Axios** | Frontend-backend communication |

---

## 🛠 Getting Started

### 1. Clone the Repository
git bash:<br>
git clone https://github.com/foramgandhicodecraft/mern-hospital-management.git <br>
cd mern-hospital-management

### 2. Setup Environment Variables

Create a .env file in /backend with:<br>
PORT=5000 <br>
JWT_SECRET=your_jwt_secret <br>
MONGO_URL=your_mongodb_connection_string <br>
ADMIN_EMAIL=admin@example.com <br>
ADMIN_PASSWORD=admin123 <br>

Frontend & Admin (/frontend/.env and /admin/.env)<br>
VITE_BACKEND_URL=http://localhost:4000<br>

CLOUDINARY_CLOUD_NAME=your_cloud_name<br>
CLOUDINARY_API_KEY=your_api_key<br>
CLOUDINARY_API_SECRET=your_api_secret<br>

### 3. Install Dependencies
npm install

###  4. Start the Project
Backend:<br>
cd backend<br>
npm run server<br>
Frontend:<br>
cd frontend<br>
npm run dev<br>
Admin:<br>
cd admin<br>
npm run dev<br>

##  Authentication
- JWT Token is generated on login
- Stored in localStorage
- Sent in headers for protected routes
- Backend validates token before allowing access

 ##  Author
Foram Gandhi

##  License
This project is licensed under the MIT License.
