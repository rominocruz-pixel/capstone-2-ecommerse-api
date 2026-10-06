# Capstone 2 - E-Commerce REST API
## Description
A REST API for managing e-commerce products using Node.js, Express, MongoDB, and Mongoose.
## Technologies
- Node.js
- Express.js
- MongoDB
- Mongoose
- Postman - API Testing
## 📂 Project Structure
capstone-2-ecommers-api/
├── src/
│ ├── config/
│ │ └── db.js
│ ├── controllers/
│ │ └── productController.js
│ ├── middleware/
│ │ └── errorHandler.js
│ ├── models/
│ │ └── Product.js
│ ├── routes/
│ │ └── productRoutes.js
│ └── server.js
├── .env
├── .gitignore
├── package.json
└── README.md

## Installation
1. Clone the repository
    bash 
    git clone https://github.com/USERNAME/REPOSITORY.git
2. Run: npm install
3. Create .env:
PORT=5000
MONGO_URI=your_connection_string
4. Run: npm run dev
## Base URL
http://localhost:5000
## Product Endpoints
- POST /api/products
- GET /api/products
- GET /api/products/:id
- PATCH /api/products/:id
- DELETE /api/products/:id
## Search / Filter
GET /api/products?category=Accessories
GET /api/products?search=mouse

## Example Create Product
POST http://localhost:5000/api/products

Request body:

json

{
"name": "Mechanical Keyboard",
"description": "RGB mechanical keyboard",
"price": 1850,
"category": "Accessories",
"stock": 12
}

## Testing
Import/use the Postman collection: MSTCONNECT Capstone 2 API

## 📋 Environment Variables

| Variable    | Description               |
| ----------- | ------------------------- |
| `PORT`      | Port used by the server   |
| `MONGO_URI` | MongoDB connection string |

## 🔒 Security

Sensitive information should not be committed to the repository.

Make sure `.gitignore` contains:

node_modules/ 
.env