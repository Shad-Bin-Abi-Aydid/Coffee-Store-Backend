# Coffee Store Server

A RESTful backend API for the Coffee Store application, built with Node.js, Express, and MongoDB.

## Live Demo

- **Frontend Live Site:** [coffee-store-2c760.web.app](https://coffee-store-2c760.web.app/)
- **Frontend Repository:** [github.com/Shad-Bin-Abi-Aydid/Coffee-Store](https://github.com/Shad-Bin-Abi-Aydid/Coffee-Store)

## Features

- Full CRUD operations for coffee items
- User management (create, read, delete, update sign-in time)
- MongoDB Atlas integration
- Environment variable configuration for secure credentials

## Tech Stack

- **Runtime:** Node.js
- **Framework:** Express.js v5
- **Database:** MongoDB Atlas
- **Packages:** `cors`, `dotenv`, `mongodb`

## API Endpoints

### Coffee

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/coffee` | Get all coffees |
| `POST` | `/coffee` | Add a new coffee |
| `GET` | `/coffee/:id` | Get a single coffee by ID |
| `PUT` | `/coffee/:id` | Update a coffee by ID |
| `DELETE` | `/coffee/:id` | Delete a coffee by ID |

### Users

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/allusers` | Get all users |
| `POST` | `/users` | Create a new user |
| `DELETE` | `/users/:id` | Delete a user by ID |
| `PATCH` | `/users` | Update user's last sign-in time |

## Getting Started

### Prerequisites

- Node.js (v18 or higher)
- A [MongoDB Atlas](https://www.mongodb.com/cloud/atlas) account and cluster

### Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/Shad-Bin-Abi-Aydid/coffee-store-server.git
   cd coffee-store-server
   ```

2. Install dependencies:
   ```bash
   npm install
   ```

3. Create a `.env` file in the root directory:
   ```env
   DB_User=your_mongodb_username
   DB_Pass=your_mongodb_password
   ```

4. Start the server:
   ```bash
   npm start
   ```

The server will run on `http://localhost:5000` by default.

## Environment Variables

| Variable | Description |
|----------|-------------|
| `DB_User` | MongoDB Atlas database username |
| `DB_Pass` | MongoDB Atlas database password |
| `PORT` | Server port (defaults to `5000`) |
