# Express Reviews API

This project is a Node.js Express server that provides an API for managing product reviews. It includes endpoints for retrieving, adding, deleting, and editing reviews associated with products.

## Project Structure

```
express-reviews-api
├── src
│   ├── app.js                # Entry point of the application
│   ├── routes
│   │   └── productRoutes.js  # Routes for product-related requests
│   ├── controllers
│   │   └── reviewController.js # Logic for handling review-related requests
│   ├── models
│   │   ├── Product.js        # Model representing a product
│   │   ├── Review.js         # Model representing a review
│   │   └── User.js           # Model representing a user
│   └── middleware
│       └── errorHandler.js    # Middleware for handling errors
├── package.json               # NPM configuration file
└── README.md                  # Documentation for the project
```

## Endpoints

- **GET /product/:ID/reviews/**: Retrieve all reviews for a specific product.
- **POST /product/:ID/reviews/**: Publish a new review for a specific product.
- **DELETE /product/:ID/review/:reviewID**: Delete an existing review from a specific product.
- **PUT /product/:ID/review/:reviewID**: Edit an existing review for a specific product.
- **404 Error**: Returns a 404 error for routes not found.

## Installation

1. Clone the repository:
   ```
   git clone <repository-url>
   ```

2. Navigate to the project directory:
   ```
   cd express-reviews-api
   ```

3. Install the dependencies:
   ```
   npm install
   ```

## Usage

To start the server, run:
```
npm start
```

The server will be running on `http://localhost:3000`. You can use tools like Postman or curl to interact with the API endpoints.

## License

This project is licensed under the MIT License.