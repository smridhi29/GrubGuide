
# GrubGuide

Welcome to the GrubGuide Food Ordering web application, a comprehensive MERN stack project designed to showcase the integration of MongoDB, Express.js, React, and Node.js. This application provides a practical guide for building a food ordering system, covering frontend and backend development aspects.







## Features

- User Authentication: 
User authentication is implemented using a combination of React Context API and backend Express middleware.
User details (username and password) are securely stored in MongoDB.
The app uses JSON Web Tokens (JWT) for token-based authentication.
Protected routes are created on the backend to ensure authentication before accessing certain endpoints.

- Dynamic Food Catalog:
Food items are fetched from the MongoDB database and dynamically rendered on the frontend.
Each food item is displayed with relevant details, such as name, description, price, and an associated image.
Categorization of food items is achieved through proper data organization in the database.

- Shopping Cart Functionality:
The shopping cart is managed using the React Context API to provide a centralized state.
Users can add items to the cart, adjust quantities, and remove items in real-time.
The cart state is efficiently updated, ensuring a responsive user experience.

-  Context API Integration:
React Context API is utilized to manage global state for the shopping cart.
The context provider and consumer components are implemented to share and access cart data across different parts of the application.
Centralized state management eliminates the need for prop drilling.

- Backend API with Express:
Express.js is used to set up a RESTful API for handling backend operations.
API routes are defined for CRUD functionality related to food items and user orders.
Middleware is implemented to handle CORS, authentication, and error responses.

- MongoDB Integration:
MongoDB is chosen as the NoSQL database for its flexibility in handling large volumes of data.
Mongoose is used to define schemas and models for interacting with MongoDB.
Connection to MongoDB Atlas allows for cloud-based data storage.

- Express Middleware:
Middleware functions in Express handle various tasks, including authentication and error responses.
Custom middleware is implemented to ensure that routes are protected and errors are appropriately handled.

- Order Placement:
Users can place orders through the frontend, providing necessary details such as user information and selected food items.
Orders are stored in the MongoDB database, linking each order to a specific user through their email.

- User Order History:
The app retrieves user order history by querying the MongoDB database for orders associated with the user's email.
Historical order data is displayed on the frontend, providing users with a personalized order history.


## Tech Stack

**Frontend:** 
- React: A JavaScript library for building user interfaces.
- React Router Dom: For handling client-side routing in React applications.
  
**Backend:** 
- Node.js: A JavaScript runtime for server-side development.
- Express.js: A web application framework for Node.js, simplifying the creation of robust APIs.
  
**Database (MongoDB):** 
- MongoDB: A NoSQL database, providing a flexible and scalable data storage solution.
  
**Server-Side Framework (Express):** 
- Express.js: A minimalist and flexible Node.js web application framework used for building APIs and web applications.
  
**Database ORM (Mongoose):** 
- Mongoose: An ODM (Object Data Modeling) library for MongoDB and Node.js, providing a schema-based solution for modeling application data.
  
**Version Control:** 
- Git: A distributed version control system for tracking changes in source code during software development.
  
**Package Manager:** 
- npm (Node Package Manager): A package manager for Node.js packages and modules.
  
**Code Editor:**
- Visual Studio Code (VS Code): A lightweight and powerful code editor.



## Getting Started
Follow these steps to set up and run the GrubGuide Food Ordering App:

Clone the repository:

```bash
  git clone https://github.com/smridhi29/GrubGuide.git
  cd mernapp

  ```
For front-end
```bash
  npm install
  npm start
  ```

  For back-end (To start using nodemon for automatic server restarts)
```bash
  nodemon ./index.js
  ```
The Express server will be running at http://localhost:5000  


Ensure that MongoDB is installed on your machine. You can download it from the [official MongoDB website](https://www.mongodb.com/docs/manual/installation/).


 Run the following command to start the MongoDB server:
```bash
  mongod
  ```

Open your web browser and go to http://localhost:3000 to access the GrubGuide Food Ordering App.
