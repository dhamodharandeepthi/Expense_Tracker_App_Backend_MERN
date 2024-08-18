# Expense Tracker API

A simple RESTful API for managing expenses, built with Node.js, Express, and MongoDB.

### Features

- **CRUD Operations:** Create, Read, Update, and Delete expenses.

- **Data Persistence:** Stores expense data in a MongoDB database.

- **Cross-Origin Resource Sharing (CORS):** Supports requests from different origins.

### Technologies Used

- **Node.js:** JavaScript runtime for server-side programming.

- **Express:** Web framework for Node.js.

- **MongoDB:** NoSQL database for storing expense data.

- **Mongoose:** ODM (Object Data Modeling) library for MongoDB and Node.js.

- **Cors:** Middleware for enabling CORS.

### Usage

Interact with the API using tools like Postman

#### some example requests

- **Get all expenses**

```javascript
GET http://localhost:8000/api/expenses
```

- **Create a new expense:**

```javascript
POST http://localhost:8000/api/expenses
Content-Type: application/json

{
  "amount": 100,
  "category": "Food",
  "date": "2024-08-15",
  "description": "Lunch with friends"
}
```

- **Update an existing expense**

```javascript
PUT http://localhost:8000/api/expenses/:id
Content-Type: application/json

{
  "amount": 120,
  "category": "Food",
  "date": "2024-08-15",
  "description": "Dinner with family"
}
```

- **Delete an expense:**

```javascript
DELETE http://localhost:8000/api/expenses/:id
```

### API Endpoints

- **`GET /api/expenses:`** Retrieve all expenses.

- **`POST /api/expenses:`** Create a new expense.

- **`PUT /api/expenses/:id:`** Update an existing expense by ID.

- **`DELETE /api/expenses/:id:`** Delete an expense by ID