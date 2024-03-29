# E-commerce-App-backend

This is the backend for an E-commerce application that allows users to view available products and add them to their cart for purchase. The backend is built with Node.js and Express.js, and utilizes MongoDB for data storage. 

## Features

- API endpoints for retrieving products and adding/removing products to/from cart
- User authentication and authorization with JSON Web Tokens (JWT)
- Secure password storage with bcrypt hashing
- Integration with MongoDB for persistent data storage
- Error handling middleware to ensure smooth user experience

## Getting Started

### Prerequisites

- Node.js installed on your machine
- MongoDB installed on your machine
- A tool such as Postman for testing API endpoints

### Installing

1. Clone the repository to your local machine
2. Install dependencies by running `npm install` in your terminal
3. Create a `.env` file in the root directory of the project and add the following variables:

```
MONGODB_URI=<your MongoDB URI>
JWT_SECRET=<your JWT secret>
```

4. Start the server by running `npm start` in your terminal

## API Endpoints

### Products

- GET /products - retrieve all available products
- GET /products/:id - retrieve a specific product by its ID

### Cart

- GET /cart - retrieve the current user's cart
- POST /cart - add a product to the current user's cart
- DELETE /cart/:id - remove a product from the current user's cart

## Authentication

- POST /register - register a new user
- POST /login - log in an existing user and receive a JWT

## Built With

- Node.js
- Express.js
- MongoDB
