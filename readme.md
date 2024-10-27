# Natours Application

Built using modern technologies: node.js, express, mongoDB, mongoose and friends 😁

## Table of Contents
- [Introduction](#introduction)
- [Features](#features)
- [Technologies](#technologies)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contributing](#contributing)
- [License](#license)

## Introduction
Natours is a tour booking application that allows users to book tours, view tour details, and manage their bookings. It is built using modern web technologies to ensure a seamless and efficient user experience.

## Features
- User authentication and authorization
- Tour booking and management
- Tour reviews and ratings
- User profile management
- Admin panel for managing tours and users
- Strong error handling and data modeling
- Fast, scalable, feature-rich RESTful API (includes filters, sorts, pagination, and much more)
- Server-side website rendering with Pug templates
- Credit card payments with Stripe
- Sending emails & uploading files
- Advanced authentication and authorization (including password reset)
- Security: encryption, sanitization, rate limiting
- CRUD operations with MongoDB and Mongoose
- Handling geospatial data in NoSQL databases

## Technologies
- **Node.js**
- **Express**
- **MongoDB**
- **Mongoose**
- **JWT**
- **Bcrypt**
- **Pug**

## Installation
To get started with the Natours application, follow these steps:

1. Clone the repository:
    ```sh
    git clone https://github.com/yourusername/natours.git
    cd natours
    ```

2. Install the dependencies:
    ```sh
    npm install
    ```

3. Set up environment variables:
   Create a `.env` file in the root directory and add the following:
    ```env
    NODE_ENV=development
    PORT=3000
    DATABASE=mongodb+srv://<username>:<password>@cluster0.mongodb.net/natours
    DATABASE_PASSWORD=<your-database-password>
    JWT_SECRET=<your-jwt-secret>
    JWT_EXPIRES_IN=90d
    JWT_COOKIE_EXPIRES_IN=90
    ```

4. Start the development server:
    ```sh
    npm run start:dev
    ```

## Usage
Once the server is running, you can access the application at `http://localhost:3000`.

## API Endpoints
Here are some of the main API endpoints available in the Natours application:

- **Tours**
    - `GET /api/v1/tours`: Get all tours
    - `GET /api/v1/tours/:id`: Get a single tour by ID
    - `POST /api/v1/tours`: Create a new tour (Admin only)
    - `PATCH /api/v1/tours/:id`: Update a tour by ID (Admin only)
    - `DELETE /api/v1/tours/:id`: Delete a tour by ID (Admin only)

- **Users**
    - `POST /api/v1/users/signup`: Sign up a new user
    - `POST /api/v1/users/login`: Log in a user
    - `GET /api/v1/users/me`: Get the logged-in user's profile
    - `PATCH /api/v1/users/updateMe`: Update the logged-in user's profile
    - `DELETE /api/v1/users/deleteMe`: Delete the logged-in user's profile

- **Bookings**
    - `GET /api/v1/bookings`: Get all bookings (Admin only)
    - `POST /api/v1/bookings`: Create a new booking
    - `GET /api/v1/bookings/:id`: Get a single booking by ID
    - `DELETE /api/v1/bookings/:id`: Delete a booking by ID

## Contributing
Contributions are welcome! Please follow these steps to contribute:

1. Fork the repository
2. Create a new branch (`git checkout -b feature/your-feature`)
3. Commit your changes (`git commit -m 'Add some feature'`)
4. Push to the branch (`git push origin feature/your-feature`)
5. Open a pull request

## License
This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.