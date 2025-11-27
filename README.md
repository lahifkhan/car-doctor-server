# Car Doctor Backend (Node.js + Express + MongoDB)

This is the backend server for the **Car Doctor** application.  
It provides RESTful APIs for **Users**, **Services**, and **Products**, using **Express.js** and **MongoDB Atlas**.

---

## Features

- User registration and lookup
- Add and fetch car services
- Add, fetch, and delete products
- Filter products by user email
- REST-based clean API design
- MongoDB Atlas connection

---

## Tech Stack

- Node.js
- Express.js
- MongoDB Atlas
- CORS
- Dotenv

---

## Live Server

`https://car-doctor-client-85y1.vercel.app/`

---

## CLIENT Repository

`https://github.com/lahifkhan/car-doctor-client`

---

## Installation

### 1\. Clone the Repository

`git clone https://github.com/lahifkhan/car-doctor-server.git cd car-doctor-server`

---

### 2\. Install Dependencies

`npm install`

---

### 3\. Create .env File

Create a `.env` file in the project root:

`DB_USER=your_mongodb_username DB_PASS=your_mongodb_password PORT=4000`

Replace the values with your actual credentials.

---

### 4\. Run the Server

`npm start`

Server will run at:

`http://localhost:4000`

---

## API Endpoints

### User Routes

| Route   | Method | Description                     |
| ------- | ------ | ------------------------------- |
| `/user` | GET    | Get a user by email (`?email=`) |
| `/user` | POST   | Create a new user               |

---

### Service Routes

| Route          | Method | Description                |
| -------------- | ------ | -------------------------- |
| `/service`     | POST   | Add a new service          |
| `/service`     | GET    | Get all services           |
| `/service/:id` | GET    | Get a single service by ID |

---

### Product Routes

| Route           | Method | Description                                 |
| --------------- | ------ | ------------------------------------------- |
| `/products`     | POST   | Add a new product                           |
| `/products`     | GET    | Get all products or filter by `?userEmail=` |
| `/products/:id` | GET    | Get product details                         |
| `/products/:id` | DELETE | Delete a product by ID                      |

---

## Project Structure

`src/ ├── index.js ├── services └── products`

---

## Database

MongoDB Collections:

- `user`
- `services`
- `products`
