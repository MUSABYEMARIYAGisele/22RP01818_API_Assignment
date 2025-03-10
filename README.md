API Development Assignment - README
Overview
This project focuses on designing and implementing APIs to manage various data entities, including student records, product details, and category management for an online store. The development process involves both PHP and Laravel frameworks. Below is a structured breakdown of the tasks and implementation guidelines.

Task 1: Representing Student Data in XML and JSON
In this section, you will create XML and JSON formats to represent a student’s details, including:

Name
Age
Gender
List of enrolled subjects (each with a subject name and grade)
Additionally, you will write XQuery expressions to retrieve specific details, such as:

The student's name and age
The names of all subjects the student is taking
Task 2: Building a Simple Product API with PHP
This part involves developing a basic API in PHP to handle product management using RESTful endpoints. The following functionalities should be implemented:

GET /products → Fetch all products
GET /products/{id} → Retrieve a product by its ID
POST /products → Add a new product
PUT /products/{id} → Update an existing product’s details
DELETE /products/{id} → Remove a product by its ID
Each product should have an ID, name, description, and price. The product data will be stored in a PHP array for simplicity, and responses should be formatted in JSON.

Task 3: Category Management API Using Laravel
In this activity, you will develop an API using Laravel to manage product categories in an online store. The API will interact with a MySQL database named online_store, containing a categories table with the following columns:

id
name
lft
rgt
created_at
updated_at
The Nested Set Model will be used to handle hierarchical categories. The API should support the following operations:

GET /categories → Retrieve all categories in XML format
GET /categories/{id} → Fetch a specific category by ID in XML format
POST /categories → Add a new category (accepts XML input with name and parent_id)
PUT /categories/{id} → Modify an existing category (accepts XML input with name)
DELETE /categories/{id} → Remove a category and return a success response in XML
Error handling and validation should be implemented to ensure that invalid requests return appropriate XML-formatted error responses. The implementation will involve Laravel routing, controllers, models, and unit tests to validate the API's functionality.

Task 4: Banking System API with Laravel
This section requires the development of an API for a banking system using Laravel. The system will support essential banking operations, such as:

Account creation
Deposits
Withdrawals
Prerequisites
Ensure your development environment includes the following:

PHP (version 8.0 or later)
Composer
MySQL or another compatible database
Laravel (version 9 or newer)
Node.js & NPM (for managing frontend assets)
Installation Guide
Backend Setup
Clone the project repository.
Install required dependencies using:
sh
Copy
Edit
composer install
Copy .env.example to .env and configure database settings.
Generate an application key:
sh
Copy
Edit
php artisan key:generate
Run database migrations and seed initial data:
sh
Copy
Edit
php artisan migrate  
php artisan db:seed  
Start the Laravel development server:
sh
Copy
Edit
php artisan serve  
Frontend Setup
Install frontend dependencies:
sh
Copy
Edit
npm install  
Compile frontend assets:
sh
Copy
Edit
npm run dev  
API Testing and Documentation
APIs can be tested using tools like Postman or Swagger. The Swagger UI will automatically generate API documentation, which can be accessed through a designated URL.

Conclusion
This project provides practical experience in API development, covering XML/JSON data handling, RESTful API implementation in PHP, category management using Laravel’s Nested Set Model, and building a banking system API. Following these structured steps will help create a robust and maintainable API solution.
