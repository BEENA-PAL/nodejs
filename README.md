# Worko API

## Description

This project contains REST api code for assignment given by Worko.ai for role of Backend Developer Intern.

All assignment tasks are completed in this project, including:

1. Setting up the backend API with Node.js using the MVC architecture.
2. Implementing the controller, service, and DAO layers.
3. Creating models for CRUD operations and DTOs for request and response.
4. Adding validation framework for specific fields.
5. Persisting user information in a NoSQL database.
6. Writing unit tests with at least 60% coverage.
7. Implementing basic authentication using JWT.

## Table of Contents

- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Contact](#contact)

## Installation

### Prerequisites

- Node.js
- npm
- A NoSQL database (e.g., MongoDB)

### Steps

1. Clone the repository:

   ```bash
   git clone https://github.com/BEENA-PAL/nodejs.git
   ```

2. Navigate to the project directory:

   ```bash
   cd workai-assignment
   ```

3. Install dependencies:

   ```bash
   npm install
   ```

4. Set up environment variables. Create a `.env` file in the root directory with the following content:

   ```plaintext
   URI=your_mongodb_database_uri
   PORT=your_port
   JWT_SECRET_KEY=your_jwt_secret_key
   JWT_TOKEN_EXPIRATION_TIME=your_token_expiration_time
   ```

5. Start the server:

   ```bash
   node index.js
   ```

## Usage

Once the server is running, you can use tools like Postman or cURL to interact with the API.

## API Endpoints

### User Resource: `/worko/user`

- **GET** - List all users

  ```bash
  GET /worko/user
  ```

- **GET** - Get user details by ID

  ```bash
  GET /worko/user/:userId
  ```

- **POST** - Create a new user

  ```bash
  POST /worko/user
  ```

- **PUT** - Update user

  ```bash
  PUT /worko/user
  ```

- **PATCH** - Partially update user

  ```bash
  PATCH /worko/user
  ```

- **DELETE** - Soft delete user in the database

  ```bash
  DELETE /worko/user/:userId
  ```

### User Payload

The required fields for creating or updating a user are:

- Id (Generated)
- email
- name
- age
- city
- zipcode

## Contact

Narendra Mali - mailto:beenapal570@gmail.com
