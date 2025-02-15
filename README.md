# Product API

A simple REST API built with Node.js, Express, and MongoDB to manage product data.

## Features

- Add a product
- Retrieve all products
- Delete a product

## Technologies Used

- Node.js
- Express.js
- MongoDB (Mongoose)
- dotenv (for environment variables)
- cors (for handling cross-origin requests)
- Postman

## Installation

Clone the repository: 

   ```sh
   git clone https://github.com/0Sa-ad0/product-api.git
   cd product-api
   ```

Install dependencies: \
    ```
    npm install express mongoose dotenv body-parser cors 
    npm install --save-dev nodemon
    ```

Create a .env file in the root directory and add: \
    ```
    PORT=5000
    MONGO_URI=mongodb://localhost:27017/productdb
    ```

Start the server: \
    ```
    npm run dev
    ```

# API Endpoints

## Add a Product

- Endpoint: `POST` `/api/products/add`
- Request Body:

    ```json
    {
        "name": "Laptop",
        "price": 1200,
        "description": "High-end laptop"
    }

    Response:

    {
        "_id": "65df2...",
        "name": "Laptop",
        "price": 1200,
        "description": "High-end laptop",
        "createdAt": "2025-01-30T10:00:00.000Z"
    }
    ```
![](https://github.com/0Sa-ad0/product-api/blob/main/screenshot/add.png)

## Retrieve All Products

- Endpoint: `GET` `/api/products/list`
- Response:

    ```json
    [
        {
            "_id": "65df2...",
            "name": "Laptop",
            "price": 1200,
            "description": "High-end laptop",
            "createdAt": "2025-01-30T10:00:00.000Z"
        }
    ]
    ```
![](https://github.com/0Sa-ad0/product-api/blob/main/screenshot/list.png)

## Delete a Product

- Endpoint: `DELETE` `/api/products/delete/:id`
- Response:

    ```json
    {
        "message": "Product deleted"
    }
    ```
![](https://github.com/0Sa-ad0/product-api/blob/main/screenshot/delete.png)

# VIDEO

https://github.com/user-attachments/assets/68db8677-a31e-4aa3-a171-b8995c16ef1e

