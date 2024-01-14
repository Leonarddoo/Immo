
# Slim 4 API with MySQL and Optional S3 Storage

This is a simple API built with Slim 4 framework, utilizing MySQL for data storage and providing an optional integration with Amazon S3 for file storage.

## Getting Started
### Prerequisites
Before you begin, ensure you have the following installed:

- PHP
- Composer
- MySQL
- (Optional) Amazon S3 account for storage

### Installation
1. Clone the repository:
```bash
git clone https://github.com/Leonarddoo/Immo/tree/main/immo-api-php-main
```
2. Install dependencies:
```bash
composer install
```
3. Create a copy of the .env.example file:
```bash
cp .env.example .env
```
4. Update the .env file with your database and S3 credentials.

### Database Setup

1. Create a MySQL database for the application.

2. Update the .env file with your database credentials:

````
MYSQL_HOST=
MYSQL_DATABASE=
MYSQL_USER=
MYSQL_PASSWORD=
MYSQL_ROOT_PASSWORD=
````

### S3 Setup (Optional)

If you want to use S3 storage, update the .env file with your S3 credentials:

```
S3_KEY=
S3_SECRET=
S3_REGION=
S3_BUCKET=
```

### Run the Application
Start the PHP built-in server:

```
php -S localhost:<PORT> -t ./public
```
Replace PORT with your desired port number.

Visit http://localhost:PORT in your browser to access the API.

## API Endpoints
#### Options Routes
- POST /option: Create a new option.
- GET /option: Retrieve the list of options.
- GET /option/{id}: Retrieve a specific option by ID.
- POST /option/{id}: Update a specific option by ID.
- DELETE /option/{id}: Delete a specific option by ID.

#### Property Routes
- POST /property: Create a new property

- GET /property: Retrieve the list of properties.

- GET /property/{id}: Retrieve a specific property by ID.

- PUT /property/{id}/sell: Sell a specific property by ID.

- PUT /property/{id}/unsell: Unsell a specific property by ID.

- POST /property/{id}: Update a specific property by ID.

- DELETE /property/{id}: Delete a specific property by ID.

- POST /property/{id}/image: Add an image to a specific property.

- DELETE /property/{id}/image/{image_id}: Delete an image from a specific property.


