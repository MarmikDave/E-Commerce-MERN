# E-Commerce Full Stack Application

This project is a full-stack E-Commerce website built using the MERN stack (MongoDB, Express.js, React.js, Node.js). The application includes an **Admin Panel** for managing products and an **E-Commerce Client Panel** for browsing, adding products to the cart, and checking out using multiple payment gateways.

## Features

### Admin Panel
- Add, delete, and update products.
- Manage product shipping status (e.g., shipped, out for delivery, delivered).
- Update product information.

### Client Panel
- Browse a collection of products.
- Add products to the cart.
- Checkout using Razorpay, Stripe, or Cash on Delivery (COD).
- View images of products, stored on Cloudinary.
- Payments are securely processed using Stripe or Razorpay.

### Backend
- All routes and controllers are implemented to handle product management, user actions, and payment processing.
- MongoDB is used as the database for storing product and order information.
- Product images are stored and retrieved from Cloudinary.

---

## Installation

### Prerequisites
- Node.js
- MongoDB
- Cloudinary Account
- Stripe and Razorpay Accounts

### Clone the Repository
```bash
git clone https://github.com/MarmikDave/E-Commerce-MERN
cd E-Commerce-MERN
```

### Install Dependencies

#### Server
```bash
cd server
npm install
```

#### Client
```bash
cd client
npm install
```

#### Admin
```bash
cd admin
npm install
```

### Environment Variables

#### Server Environment Variables (`server/.env`)
```plaintext
MONGODB_URI = "your_mongodb_uri"
CLOUDINARY_NAME = 'your_cloudinary_name'
CLOUDINARY_API_KEY = 'your_cloudinary_api_key'
CLOUDINARY_SECRET_KEY = 'your_cloudinary_secret_key'
JWT_SECRET = 'your_jwt_secret'
ADMIN_EMAIL = 'admin@gmail.com'
ADMIN_PASSWORD = 'admin_password'
STRIPE_SECRET_KEY = "your_stripe_secret_key"
RAZORPAY_KEY_ID = "your_razorpay_key_id"
RAZORPAY_KEY_SECRET = "your_razorpay_key_secret"
```

#### Client Environment Variables (`client/.env`)
```plaintext
VITE_BACKEND_URL = 'http://localhost:4000'
VITE_RAZORPAY_KEY_ID = "your_razorpay_key_id"
```

#### Admin Environment Variables (`admin/.env`)
```plaintext
VITE_BACKEND_URL = 'http://localhost:4000'
```

## Running the Project

### Run the Server
```bash
cd server
npm run server
```

### Run the Client
```bash
cd client
npm run dev
```

### Run the Admin Panel
```bash
cd admin
npm run dev
```

## Technologies Used
- **Frontend (Client/Admin)**: React.js, Vite
- **Backend**: Node.js, Express.js
- **Database**: MongoDB, Mongoose
- **Payment Gateways**: Razorpay, Stripe
- **Image Storage**: Cloudinary
- **Authentication**: JWT, Bcrypt
