This project is an E-commerce API built with Flask. It allows customers to place orders, manage their accounts, and interact with products. This README provides clear instructions on how to set up and run the application, as well as explanations of its features.
The required downloads for running the project are as follows. Please create a virtual environment before downloading.
Flask
Flask-SQLAlchemy
Flask-Marshmallow
marshmallow
MySQL
MySQL-connector-python

The project encompasses different Features to create, read, update, and delete information. Listed below are the features you can access with this API.
Customer Management: Add, update, delete, and retrieve customer information.
Customer Account Management: Create and manage customer accounts.
Product Management: Add, update, delete, and retrieve product information.
Order Management: Place, update, delete, and retrieve orders. Each order captures the order date and the associated customer.
Order Status: Manage and update order statuses (e.g., Pending, Shipped, Delivered, Cancelled).

After downloading the specified requirements run the flask api.
The application will be running on your local server at http://127.0.0.1:5000/

The API endpoints are listed below, along with a brief discription of each endpoints purpose.

Customers
GET /customers: Retrieve all customers.
POST /customers: Add a new customer.
PUT /customers/int:id: Update a customer by ID.
DELETE /customers/int:id: Delete a customer by ID.

Customer Accounts
GET /accounts: Retrieve all customer accounts.
POST /accounts: Add a new customer account.
PUT /accounts/int:id: Update a customer account by ID.
DELETE /accounts/int:id: Delete a customer account by ID.

Products
GET /products: Retrieve all products.
POST /products: Add a new product.
PUT /products/int:id: Update a product by ID.
DELETE /products/int:id: Delete a product by ID.

Orders
GET /orders: Retrieve all orders.
POST /orders: Place a new order.
PUT /orders/int:id: Update an order by ID.
DELETE /orders/int:id: Delete an order by ID.

Order Statuses
GET /order_statuses: Retrieve all order statuses.

Customer Orders
GET /customers/int:customer_id/orders: Retrieve all orders for a customer.
PUT /customers/int:customer_id/orders/int:order_id: Update an order status for a customer.
