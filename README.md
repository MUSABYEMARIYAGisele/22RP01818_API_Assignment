# API Development Assignment - README

## Introduction
This assignment involves creating APIs to manage various data entities, including student information, products, and categories for an online store. The implementation will utilize both PHP and Laravel frameworks. Below is a structured breakdown of the activities and implementation steps.

## Activity 1: Student Information Representation (XML and JSON)
In this activity, you will create XML and JSON structures to represent a student. The student’s details should include their name, age, gender, and a list of subjects they are enrolled in. Each subject must have a subject name and a grade.

Additionally, you will write XQuery expressions to retrieve specific data. The queries should fetch the student’s name and age, as well as retrieve the names of all subjects the student is enrolled in.

## Activity 2: Simple API for Managing Products (PHP)
This activity focuses on developing a simple API in PHP to manage products. You will implement the following RESTful API endpoints:

- `GET /products` - Retrieve all products.
- `GET /products/{id}` - Retrieve a specific product by ID.
- `POST /products` - Add a new product.
- `PUT /products/{id}` - Update an existing product by ID.
- `DELETE /products/{id}` - Remove a product by ID.

Each product should include an ID, name, description, and price. The product data will be stored in an array within PHP for simplicity. All API responses should be returned in JSON format.

## Activity 3: Online Store Category Management API (Laravel)
This activity involves setting up a Laravel-based API to manage product categories in an online store. You will create a MySQL database named `online_store` and define a `categories` table with the following fields: `id`, `name`, `lft`, `rgt`, `created_at`, and `updated_at`.

To manage hierarchical categories efficiently, you will implement the **Nested Set Model** using Laravel’s Eloquent ORM. The API should support the following routes:

- `GET /categories` - Retrieve all categories in XML format.
- `GET /categories/{id}` - Retrieve a specific category by ID in XML format.
- `POST /categories` - Create a new category (accept XML with `name` and `parent_id` fields).
- `PUT /categories/{id}` - Update an existing category (accept XML with `name`).
- `DELETE /categories/{id}` - Delete a category and return a success message in XML format.

Proper error handling and validation should be implemented to return error responses in XML format for invalid requests. You will use Laravel’s routing, controllers, and models to implement this functionality. Additionally, unit tests should be written to ensure each endpoint functions correctly.

## Activity 4: Develop APIs for Your Project - Laravel Bank System
This activity involves building a banking system using Laravel. The system will support fundamental banking operations such as creating accounts, making deposits, and processing withdrawals.

To set up the project, ensure that the following dependencies are installed on your system:
- PHP (version 8.0 or higher)
- Composer
- MySQL (or any preferred database system)
- Laravel (version 9 or higher)
- Node.js and NPM (for frontend asset management)

### Installation Instructions
1. Clone the repository containing the project files.
2. Install backend dependencies by running:
   ```bash
   composer install
   ```
3. Configure the environment file by copying `.env.example` to `.env` and setting up the database connection.
4. Generate the application key by executing:
   ```bash
   php artisan key:generate
   ```
5. Run database migrations and seed data with:
   ```bash
   php artisan migrate
   php artisan db:seed
   ```
6. Start the Laravel development server using:
   ```bash
   php artisan serve
   ```

### Frontend Setup
For the frontend, install dependencies using:
```bash
npm install
```
Then compile frontend assets with:
```bash
npm run dev
```

## API Documentation
The API can be tested using **Postman** or **Swagger**. The **Swagger UI** will automatically generate API documentation, which can be accessed through a specified URL.

## Conclusion
This assignment provides hands-on experience in API development, covering XML/JSON data handling, RESTful API creation with PHP, hierarchical category management with Laravel, and building a banking system API. By following these structured guidelines, you will develop a well-functioning and maintainable API system.

