# MERN Stack CRUD Application

This project is a MERN (MongoDB, Express, React, Node.js) stack application designed to perform CRUD (Create, Read, Update, Delete) operations for managing products. The frontend uses Chakra UI for styling, and the backend leverages MongoDB for data persistence.

## Features

- Create a product with a name, price, and image.
- View a list of products.
- Update product details.
- Delete products.

## File Structure

### Backend
```
backend/
├── config/
│   └── db.js          # MongoDB connection configuration
├── controllers/
│   └── product.controller.js  # Handles product-related logic
├── models/
│   └── products.model.js      # Mongoose schema and model for products
├── routes/
│   └── product.route.js       # Product-related API routes
├── server.js       # Main backend entry point
├── package.json    # Backend dependencies
├── package-lock.json
├── .env            # Environment variables
└── .gitignore      # Ignored files and directories
```

### Frontend
```
frontend/
├── node_modules/    # Node.js modules
├── public/
│   └── index.html   # HTML template
├── src/
│   ├── components/
│   │   ├── Navbar.jsx       # Navigation bar component
│   │   └── Product.jsx      # Product display component
│   ├── pages/
│   │   ├── CreatePage.jsx   # Page for creating and editing products
│   │   └── HomePage.jsx     # Home page displaying the product list
│   ├── store/
│   │   └── product.js       # State management for products
│   ├── App.jsx      # Main application component
│   └── main.jsx     # Entry point for React application
├── .eslintrc.cjs    # ESLint configuration
├── index.html       # Base HTML file
├── package.json     # Frontend dependencies
├── package-lock.json
├── vite.config.js   # Vite configuration
└── .gitignore       # Ignored files and directories
```

### Root Directory
```
├── backend/
├── frontend/
├── package.json      # Root package.json for both frontend and backend
├── package-lock.json
├── .env              # Root environment variables
├── .gitignore        # Root ignored files and directories
└── README.md         # Project documentation
```

## Installation and Setup

### Prerequisites
- Node.js installed on your machine
- MongoDB instance running locally or in the cloud

### Backend Setup
1. Navigate to the `backend` directory:
   ```bash
   cd backend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Configure the `.env` file:
   ```env
   MONGO_URI=your_mongo_connection_string
    
   ```
4. Start the server:
   ```bash
   npm start
   ```

### Frontend Setup
1. Navigate to the `frontend` directory:
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

### Root Setup
If you are managing both frontend and backend simultaneously, install the root dependencies (if applicable) and run both parts concurrently using tools like `concurrently`.

## Usage

1. Open the frontend in your browser at `http://localhost:5173` (default Vite dev server port).
2. Interact with the CRUD operations:
   - Add a new product by providing a name, price, and image.
   - View the list of products.
   - Edit product details.
   - Delete a product.
3. Data is stored and managed in the MongoDB database.

## Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB (via Mongoose)

### Frontend
- React.js
- Chakra UI (for styling)

### Others
- Vite (for frontend build tool)
- ESLint (for code linting)

## API Endpoints

### Base URL: `/api/products`

- **GET /api/products**: Fetch all products.
- **POST /api/products**: Create a new product.
- **PUT /api/products/:id**: Update a product by ID.
- **DELETE /api/products/:id**: Delete a product by ID.

## Environment Variables
Ensure the following environment variables are configured in the `.env` file:

- `MONGO_URI`: MongoDB connection string
- `PORT`: Port for the backend server

## Contributing
1. Fork the repository.
2. Create a new branch for your feature/bugfix.
3. Commit your changes and push them to your fork.
4. Open a pull request to the main branch.

## License
This project is open-source and available under the [MIT License](LICENSE).

## Screenshots
Include relevant screenshots of your application for better understanding.
 
---
Feel free to reach out for any queries or feedback!

