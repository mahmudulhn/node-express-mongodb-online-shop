# Node.js Express MongoDB Online Shop

## Project Overview
The Node.js Express MongoDB Online Shop is a web application designed to facilitate online shopping. It allows users to browse products, add items to their cart, place orders, and manage their accounts. The application includes both customer and admin functionalities, where admins can manage the product catalog and view orders.

## Features
- **User Authentication**: Sign up, log in, and log out functionalities.
- **Product Management**: Admins can add, edit, and delete products.
- **Shopping Cart**: Customers can add products to their cart and proceed to checkout.
- **Order Management**: Customers can place orders, and admins can view all orders.
- **Responsive Design**: The application is designed to work well on both desktop and mobile devices.

## Technologies Used
- **Node.js**: A JavaScript runtime for building server-side applications.
- **Express.js**: A web application framework for Node.js, used to build the application's server.
- **MongoDB**: A NoSQL database used to store user data, products, and orders.
- **Mongoose**: An ODM (Object Data Modeling) library for MongoDB and Node.js.
- **EJS (Embedded JavaScript)**: A templating engine used to generate HTML markup with plain JavaScript.
- **CSS**: For styling the application.
- **JavaScript**: For client-side scripting and interactivity.
- **HTML**: For structuring the web pages.
- **Nodemon**: A tool for automatically restarting the Node.js server during development.

## Project Structure

```
node-express-mongodb-online-shop/
├── controllers/
│ ├── admin.controller.js
│ ├── auth.controller.js
│ ├── customer.controller.js
├── middlewares/
│ ├── auth.middleware.js
│ ├── error-handler.middleware.js
├── models/
│ ├── cart.model.js
│ ├── order.model.js
│ ├── product.model.js
│ ├── user.model.js
├── public/
│ ├── css/
│ ├── images/
│ ├── js/
├── routes/
│ ├── admin.routes.js
│ ├── auth.routes.js
│ ├── customer.routes.js
├── views/
│ ├── admin/
│ ├── auth/
│ ├── customer/
│ ├── shared/
├── app.js
├── package.json
├── README.md
└── .gitignore

```


## Detailed Documentation

### 1. Controllers
- **admin.controller.js**: Manages admin-specific actions like adding, editing, and deleting products.
- **auth.controller.js**: Handles user authentication including login, signup, and logout.
- **customer.controller.js**: Manages customer actions such as viewing products, adding products to the cart, and placing orders.

### 2. Middlewares
- **auth.middleware.js**: Checks if a user is authenticated before allowing access to certain routes.
- **error-handler.middleware.js**: Manages error handling across the application.

### 3. Models
- **cart.model.js**: Schema and model for user shopping carts.
- **order.model.js**: Schema and model for orders.
- **product.model.js**: Schema and model for products.
- **user.model.js**: Schema and model for users.

### 4. Public
Contains static files like CSS, JavaScript, and images.

### 5. Routes
Defines the routes and associates them with corresponding controller functions.
- **admin.routes.js**: Routes for admin actions.
- **auth.routes.js**: Routes for authentication actions.
- **customer.routes.js**: Routes for customer actions.

### 6. Views
Contains the EJS templates for rendering HTML pages.
- **admin/**: Views related to admin functionalities.
- **auth/**: Views for authentication pages (login, signup).
- **customer/**: Views for customer-facing pages (product listings, cart, orders).
- **shared/**: Shared views like header, footer, and error pages.

### 7. app.js
The main entry point of the application. It sets up the Express server, connects to MongoDB, and initializes routes and middleware.

### 8. package.json
Lists the project dependencies and scripts for running the application.

### 9. README.md
Contains an overview of the project, setup instructions, and usage guidelines.

### 10. .gitignore
Specifies files and directories to be ignored by Git.

## Additional Information
- **Database**: The application uses MongoDB for storing data. Ensure MongoDB is running and properly configured in the `.env` file.
- **Authentication**: The application uses sessions and cookies for managing user authentication.
