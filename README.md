# 📦 Express.js Products API

## 📄 Project Overview

A simple RESTful API for managing products built with Express.js. Supports CRUD operations, filtering, pagination, search, statistics, authentication, and middleware.

## ⚙️ Setup Instructions

1. Clone the repository.
2. Install dependencies:

```bash
npm install
```

3. Create a `.env` file based on `.env.example`:

```env
PORT=3000
API_KEY=supersecretapikey123
```

4. Start the server:

```bash
node server.js
```

## 📖 API Documentation

| Method | Endpoint                          | Description                          |
|--------|----------------------------------|--------------------------------------|
| GET    | /api/products                    | List all products (supports filtering, pagination, search) |
| GET    | /api/products/:id                | Get a specific product               |
| POST   | /api/products                    | Add a new product (requires API key) |
| PUT    | /api/products/:id                | Update product (requires API key)    |
| DELETE | /api/products/:id                | Delete product (requires API key)    |
| GET    | /api/products/stats/count-by-category | Get product count by category        |

## 🔐 Authentication

For POST, PUT, and DELETE requests, include an API key in the request header:

```
api-key: supersecretapikey123
```

## 🧪 Testing

Use tools like **Postman** or **curl** to test API endpoints.

## 📂 Environment Variables

| Variable | Description              |
|----------|--------------------------|
| PORT     | Port number for server     |
| API_KEY  | API key for authentication |

Check `.env.example` for reference.
