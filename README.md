# 🛒 Full-Stack E-Commerce Website (MERN)

A complete **E-Commerce web application** built using the **MERN stack (MongoDB, Express.js, React.js, Node.js)**.  
This project offers a seamless shopping experience for users and a powerful admin dashboard for managing products, orders, and customers.  

It integrates **Stripe** and **Razorpay** for secure online payments, supports **Cash on Delivery (COD)**, and uses **Cloudinary** for optimized image storage.  
Both **frontend** and **admin panels** are built with **React.js** and **Tailwind CSS**, deployed on **Vercel** for high performance.

---

## ✨ Features

### 👤 User Features
- 🔐 **JWT Authentication & Authorization**
- 🛍️ **Browse, Search & Filter Products**
- 🛒 **Shopping Cart & Checkout**
- 💳 **Secure Payments** (Stripe & Razorpay)
- 💵 **Cash on Delivery (COD)** option
- 📦 **Order History & Tracking**
- 📱 **Responsive UI** with React.js & Tailwind CSS

### 🧑‍💼 Admin Features
The **Admin Dashboard** is designed for efficient store management:
- 📦 **Add Products:** Create new items with images, name, pricing, descriptions, category,  sizes and bestseller 
- 📑 **List Products:** View, edit, or delete existing products
- 🧾 **Manage Orders:** View all orders, update order statuses (Pending, Shipped, Delivered, etc.)  
- 📊 **Dashboard Overview** – Key metrics at a glance

---

## 🛠️ Tech Stack

| Layer | Technologies |
|--------|---------------|
| **Frontend** | React.js (Hooks, Context API), Tailwind CSS, Axios, React Router |
| **Admin Panel** | React.js, Tailwind CSS |
| **Backend** | Node.js, Express.js, Mongoose |
| **Database** | MongoDB Atlas |
| **Authentication** | JWT (JSON Web Token) |
| **Payments** | Stripe, Razorpay, Cash on Delivery |
| **Media Storage** | Cloudinary |

---

## 📂 Project Directory Structure

```bash
mern-ecommerce/
│
├── admin/
│   ├── public/
│   │   └── favicon.png
│   │
│   ├── src/
│   │   ├── assets/             # Images, icons, etc.
│   │   ├── components/         # Reusable UI components
│   │   ├── pages/              # Main pages (Add Product, Product List, Orders)
│   │   ├── App.jsx             # Main React App component
│   │   ├── index.css           # Global styles
│   │   └── main.jsx            # Entry point
│   │
│   ├── .env                    # Environment variables
│   ├── index.html              # Root HTML file
│   ├── tailwind.config.js      # Tailwind CSS configuration
│   └── package.json
│
├── backend/
│   ├── config/
│   │   ├── mongodb.js          # MongoDB connection setup
│   │   └── cloudinary.js       # Cloudinary configuration
│   │
│   ├── controllers/
│   │   ├── cartController.js   # Shopping cart operations
│   │   ├── orderController.js  # Order management logic
│   │   ├── productController.js # Product CRUD operations
│   │   └── userController.js   # User registration, login & profile
│   │
│   ├── middlewares/
│   │   ├── adminAuth.js        # Middleware for admin route protection
│   │   ├── auth.js             # Middleware for user authentication (JWT)
│   │   └── multer.js           # Middleware for image upload handling
│   │
│   ├── models/
│   │   ├── userModel.js        # User schema
│   │   ├── productModel.js     # Product schema
│   │   └── orderModel.js       # Order schema
│   │
│   ├── routes/
│   │   ├── cartRoute.js        # /api/cart routes
│   │   ├── orderRoute.js       # /api/order routes
│   │   ├── productRoute.js     # /api/product routes
│   │   └── userRoute.js        # /api/user routes
│   │
│   ├── .env                    # Environment variables
│   ├── server.js               # Main Express server file
│   └── package.json
│
├── frontend/
│   ├── public/
│   │   └── favicon.png
│   │
│   ├── src/
│   │   ├── assets/             # Images, icons, etc.
│   │   ├── components/         # Reusable UI components
│   │   ├── context/            # Context API for global state management
│   │   ├── pages/              # Main pages (Home, Product, Cart, Checkout, etc.)
│   │   ├── App.jsx             # Main React App component
│   │   ├── index.css           # Global styles
│   │   └── main.jsx            # Entry point
│   │
│   ├── .env                    # Environment variables
│   ├── index.html              # Root HTML file
│   ├── tailwind.config.js      # Tailwind CSS configuration
│   └── package.json
│
├── README.md                   # Project documentation
└── .gitignore                  # Ignored files and folders
````

---

## ⚙️ Installation & Setup (Local)

```bash
# 1️⃣ Clone the repository
git clone https://github.com/Chetnatupat/E-Commerce-Website

# 2️⃣ Navigate into the project folder
cd mern-ecommerce
```

### 🧩 Install Dependencies

#### Backend

```bash
cd backend
npm install
```

#### Frontend

```bash
cd ../frontend
npm install
```

#### Admin Panel

```bash
cd ../admin
npm install
```

---

### 🔧 Environment Configuration

Create a `.env` file in **backend**, **frontend**, and **admin** directories.

#### 🗄️ Backend `.env`

```
PORT = 4000
MONGODB_URL = your_mongodb_atlas_connection_string
CLOUDINARY_API_KEY = your_api_key
CLOUDINARY_SECRET_KEY = your_api_secret
CLOUDINARY_NAME = your_cloud_name
JWT_SECRET = your_jwt_secret_key
ADMIN_EMAIL = your_admin_email
ADMIN_PASSWORD = your_admin_password
STRIPE_SECRET_KEY = your_stripe_secret
RAZORPAY_KEY_ID = your_razorpay_key_id
RAZORPAY_KEY_SECRET = your_razorpay_secret
```

#### 🌐 Frontend `.env`

```
VITE_BACKEND_URL = https://your-backend-api-link.com/api
VITE_RAZORPAY_KEY_ID = your_razorpay_key_id
```

#### 🧑‍💼 Admin `.env`

```
VITE_BACKEND_URL = https://your-backend-api-link.com/api
```

---

## 🧪 Run Locally

### Backend

```bash
cd backend
npm run start
```

### Frontend

```bash
cd frontend
npm run dev
```

### Admin

```bash
cd admin
npm run dev
```

Then visit:

* **Frontend:** [http://localhost:5173](http://localhost:5173)
* **Admin Panel:** [http://localhost:5174](http://localhost:5174)
* **Backend:** [http://localhost:4000](http://localhost:4000)

---

## 📚 Future Enhancements

* 🧾 PDF Invoice Generation
* 💌 Email Notifications
* 📱 Progressive Web App (PWA) Support
* 🌍 Multi-language Support

---

## 👨‍💻 Author

**Developed by:** Chetna Tupat

🐙 [GitHub](https://github.com/Chetnatupat)

💼 [LinkedIn](https://linkedin.com/in/chetna-tupat)

---
