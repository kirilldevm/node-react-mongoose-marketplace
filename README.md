# Mongoose React Marketplace

A full-stack marketplace application built with React and Node.js that allows users to browse, create, edit, and delete products with secure user authentication.

## 🎯 About

Mongoose React Marketplace is a modern e-commerce platform that demonstrates a complete full-stack implementation. Users can authenticate their accounts, manage products, and interact with a persistent MongoDB database. It's an ideal project for learning how to build scalable web applications with the MERN stack.

## 🛠 Tech Stack

### Frontend

- **React** - UI library for building interactive user interfaces
- **React Router DOM** - Client-side routing for navigation
- **Axios** - HTTP client for API requests
- **CSS** - Custom styling for components

### Backend

- **Node.js & Express** - Server runtime and web framework
- **MongoDB** - NoSQL database for data persistence
- **JWT (jsonwebtoken)** - Token-based authentication
- **bcryptjs** - Password hashing and encryption
- **Body Parser** - Middleware for parsing request bodies

## ✨ Features

- **User Authentication**
  - Sign up and login functionality
  - Password encryption with bcryptjs
  - JWT-based token authentication
  - Session management

- **Product Management**
  - View all available products
  - Create new products with images and descriptions
  - Edit existing product information
  - Delete products
  - Browse product details

- **Responsive UI**
  - Modal components for user interactions
  - Backdrop overlays for focus management
  - Reusable components (Button, Input, Header)
  - Clean and intuitive interface

- **Database Integration**
  - Persistent data storage with MongoDB
  - Product catalog with images
  - User accounts and authentication records

## 📁 Project Structure

```
mongoose-react-marketplace/
├── backend/
│   ├── app.js                 # Express server setup
│   ├── db.js                  # MongoDB connection
│   ├── images/                # Product images
│   └── routes/
│       ├── auth.js            # Authentication endpoints
│       └── products.js        # Product CRUD endpoints
├── public/
│   ├── index.html
│   └── manifest.json
├── src/
│   ├── App.js                 # Main app component
│   ├── index.js               # React entry point
│   ├── index.css              # Global styles
│   ├── components/            # Reusable UI components
│   │   ├── Backdrop/
│   │   ├── Button/
│   │   ├── Header/
│   │   ├── Input/
│   │   ├── Modal/
│   │   └── Products/
│   └── pages/                 # Page components
│       └── Product/
│           ├── Auth.js        # Login/signup page
│           ├── Product.js     # Product details page
│           ├── Products.js    # Products list page
│           └── EditProduct.js # Product editor page
├── package.json
└── README.md
```

## 🚀 Getting Started

### Prerequisites

- Node.js (v10 or higher)
- MongoDB installed and running
- npm or yarn package manager

### Installation

1. **Clone the repository**

   ```bash
   git clone https://github.com/kirilldevm/node-react-mongoose-marketplace
   cd mongoose-react-marketplace
   ```

2. **Install dependencies**

   ```bash
   npm install
   ```

3. **Configure MongoDB**
   - Ensure MongoDB is running on your system
   - Update the database connection in `backend/db.js` if needed

### Running the Application

#### Development Mode (Both Frontend & Backend)

**Terminal 1 - Start the backend server:**

```bash
npm run start:server
```

The backend will run on `http://localhost:3100`

**Terminal 2 - Start the React development server:**

```bash
npm start
```

The frontend will open on `http://localhost:3000`

#### Production Build

```bash
npm run build
```

Creates an optimized production build in the `build/` directory.

## 📝 API Endpoints

### Authentication

- `POST /login` - User login
- `POST /signup` - User registration

### Products

- `GET /products` - Fetch all products
- `POST /products` - Create a new product
- `PUT /products/:id` - Update a product
- `DELETE /products/:id` - Delete a product

## 🔐 Security Features

- **Password Security** - All passwords are hashed using bcryptjs before storage
- **JWT Tokens** - Token-based authentication with 1-hour expiration
- **CORS Headers** - Cross-Origin Resource Sharing configured for frontend-backend communication
- **Input Validation** - Basic validation on email and password fields

## 💡 Key Components

- **Header** - Navigation and branding
- **Modal** - Dialog boxes for user interactions
- **Backdrop** - Semi-transparent overlay for modals
- **Input** - Reusable form input fields
- **Button** - Styled action buttons
- **Products** - Product display and management
- **ProductItem** - Individual product card component

## 📦 Available Scripts

- `npm start` - Run React development server
- `npm build` - Create production build
- `npm test` - Run tests
- `npm run start:server` - Start Node.js backend server

## 🤝 Contributing

Feel free to fork this project and submit pull requests for any improvements.

## 🎓 Learning Outcomes

This project demonstrates:

- Full-stack JavaScript/Node.js development
- React component composition and state management
- RESTful API design
- Database integration with MongoDB
- User authentication and security best practices
- Responsive UI/UX design patterns
