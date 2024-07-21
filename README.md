# Study Gymon Express API

Welcome to the **Study Gymon Express API**! This project is an API for a study buddy application designed specifically for South African matriculants. Built using Node.js and Express, this API provides various endpoints to facilitate functionalities required for managing study sessions, users, and related activities.

## Table of Contents

- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [API Documentation](#api-documentation)
- [Project Structure](#project-structure)
- [Dependencies](#dependencies)
- [Contributing](#contributing)
- [License](#license)

## Features

- User authentication and authorization
- Study session management
- User profile management
- Secure data handling with bcrypt and JWT
- Rate limiting and security enhancements
- Comprehensive API documentation with Swagger

## Installation

To get started with the Study Gymon Express API, follow these steps:

1. **Clone the repository:**

    ```bash
    git clone https://github.com/7irelo/study-gymon-express-api.git
    cd study-gymon-express-api
    ```

2. **Install dependencies:**

    ```bash
    npm install
    ```

3. **Set up environment variables:**

    Create a `.env` file in the root directory and add your environment variables. You can use the `.env.example` file as a template.

4. **Run the application:**

    ```bash
    npm start
    ```

    The server will start on the port specified in your `.env` file.

## Usage

The API provides various endpoints for interacting with the study buddy application. You can use tools like Postman or cURL to make requests to the API.

## API Documentation

API documentation is available through Swagger UI. After starting the server, you can access the documentation at:

```
http://localhost:3000/api-docs
```

## Project Structure

Here’s an overview of the project structure:

```
study-gymon-express-api/
│
├── config/                  # Configuration files
│   └── config.js            # Application configuration
│
├── controllers/             # API request handlers
│   ├── authController.js    # Authentication related operations
│   ├── sessionController.js # Study session management
│   └── userController.js    # User profile management
│
├── models/                  # Database models
│   ├── index.js             # Sequelize instance and model imports
│   ├── user.js              # User model
│   └── session.js           # Study session model
│
├── routes/                  # API route definitions
│   ├── authRoutes.js        # Routes for authentication
│   ├── sessionRoutes.js     # Routes for study sessions
│   └── userRoutes.js        # Routes for user profiles
│
├── middleware/              # Custom middleware
│   ├── authMiddleware.js    # Authentication and authorization middleware
│   └── rateLimitMiddleware.js # Rate limiting middleware
│
├── utils/                   # Utility functions
│   ├── logger.js            # Winston logger configuration
│   └── swagger.js           # Swagger documentation setup
│
├── .env                     # Environment variables
├── .env.example             # Example environment variables
├── app.js                   # Main application file
├── package.json             # Project metadata and dependencies
└── README.md                # This file
```

## Dependencies

The project uses the following dependencies:

- `bcryptjs`: Password hashing
- `body-parser`: Middleware to parse request bodies
- `compression`: Middleware for gzip compression
- `cors`: Middleware for handling CORS
- `dotenv`: Loads environment variables
- `express`: Web framework
- `express-rate-limit`: Rate limiting middleware
- `helmet`: Security headers middleware
- `jsonwebtoken`: JWT for authentication
- `morgan`: HTTP request logger middleware
- `mysql2`: MySQL client for Node.js
- `sequelize`: ORM for MySQL
- `swagger-jsdoc`: Generates Swagger documentation from JSDoc comments
- `swagger-ui-express`: Serves Swagger UI
- `winston`: Logging library

## Contributing

We welcome contributions to improve the Study Gymon Express API! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch for your changes
3. Make your changes and commit them
4. Open a pull request with a description of your changes

## License

This project is licensed under the [MIT License](LICENSE).

---

Feel free to modify or add more details as needed!
