# Product Management Dashboard

This is a simple product management system where users can add products with the following fields:
- Product Name
- Quantity in Stock
- Price per Item

Once the data is submitted, it is displayed in a table with the following columns:
- Product Name
- Quantity in Stock
- Price per Item
- Datetime Submitted
- Total Value (calculated as Quantity in Stock * Price per Item)

Users can edit the entries, and the total value of all products is shown at the bottom of the table.

The system uses Laravel for backend functionality, AJAX for real-time updates, and Bootstrap for responsive front-end design.

## Setup Instructions

1. **Install Dependencies**  
   ```bash
   composer install
   
2. **Configure Database**
   - In .env, set:
   ```bash
   DB_CONNECTION=mysql
   DB_HOST=localhost
   DB_PORT=3306
   DB_DATABASE=Product-Management-Dashboard
   DB_USERNAME=root
   DB_PASSWORD=yourpassword

3. **Generate Application Key**
   ```bash
   php artisan key:generate

4. **Create Storage Link**
   ```bash
   php artisan storage:link

5. **Run Migrations**
   ```bash
   php artisan migrate

6. **Start Development Server**
   ```bash
   php artisan serve
   ```
   - Access the app at http://127.0.0.1:8000
