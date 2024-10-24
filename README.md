# NodeJS - User Management API

This project implements a User Management API using Node.js, Express, and MongoDB. It provides a simple RESTful API for managing user data including basic CRUD operations (Create, Read, Update, Delete). The user details stored in MongoDB include the user's name, email, and age. The API was developed and tested using Postman, and MongoDB was used as the NoSQL database solution.

## Table of Contents

- [Features](#features)
- [Technologies Used](#technologies-used)
- [API Endpoints](#api-endpoints)
- [Installation](#installation)
- [Usage](#usage)
- [License](#license)
- [Author](#author)

## Features

- **Get All Users:** Retrieve a list of all users from the database.
- **Get User by ID:** Fetch details of a specific user using their unique ID.
- **Create User:** Add a new user with name, email, and age details.
- **Update User:** Modify existing user details using their unique ID.
- **Delete User:** Remove a user from the database using their unique ID.

## Technologies Used

- **Programming Language:** JavaScript (Node.js)
- **Framework:** Express.js
- **Database:** MongoDB (NoSQL)
- **API Testing:** Postman
- **Others:**
  - Visual Studio Code for development
  - Git for version control

## API Endpoints

Below is a list of the main API endpoints provided in this User Management system:

| HTTP Method | Endpoint   |   Description     |
| ----------- | ---------- | ----------------- |
|   GET       | /users     | Get all users     |
| ----------- | ---------- | ----------------- |
|   GET       | /users/:id | Get user by id    |
| ----------- | ---------- | ----------------- |
|   POST      | /users     | Create user       |
| ----------- | ---------- | ----------------- |
|   PUT       | /users/:id | Update user by id |
| ----------- | ---------- | ----------------- |
|   DELETE    | /users/:id | Delete user by id |

## User Schema

The schema for the user collection in MongoDB includes the following fields:

- **name** (String): The name of the user.
- **email** (String): The email address of the user.
- **age** (Number): The age of the user.

## Installation

To run this project locally, follow the steps below:

```bash
# Clone the repository
git clone https://github.com/Packiyalakshmi-M/User-Management-API.git

# Navigate into the project directory
cd sample_app

# Install dependencies
npm install

# Set up your environment variables for MongoDB connection in a .env file:
MONGODB_URI=mongodb://localhost:27017/userdb

# Start the serve
npm start

```

## Usage

To interact with the API, you can use tools like Postman or cURL.

Here’s an example of how to test the API using Postman:

1. **Get All Users**
   **Method:** GET
   **URL:** http://localhost:3000/users

2. **Get User by ID**
   **Method:** GET
   **URL:** http://localhost:3000/users/:id

3. **Create User**
   **Method:** POST

   **URL:** http://localhost:3000/users

   **Body:**

   json
   {
   "name": "John Doe",
   "email": "john@example.com",
   "age": 25
   }

4. **Update User**
   **Method:** PUT

   **URL:** http://localhost:3000/users/:id

   **Body:**

   json
   {
   "name": "Jane Doe",
   "email": "jane@example.com",
   "age": 30
   }

5. **Delete User**
   **Method:** DELETE
   **URL:** http://localhost:3000/users/:id

## License

This project is open source and available under the MIT License.

## Author

- Packiyalakshmi Murugan
- [LinkedIn Link](https://www.linkedin.com/in/packiyalakshmi-m-7a9844210/)
- [Github link](https://github.com/Packiyalakshmi-M/)
