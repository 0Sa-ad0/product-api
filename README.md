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

## Delete a Product

- Endpoint: `DELETE` `/api/products/delete/:id`
- Response:

    ```json
    {
    "message": "Product deleted"
    }
    ```
