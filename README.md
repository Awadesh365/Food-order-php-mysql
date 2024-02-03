# Food Order Website


This is a simple Food Order website built using PHP and MySQL. It provides an online platform for users to browse a menu and place orders for their favorite food items. Restaurant owners can manage their menu items and orders efficiently through the admin dashboard.

## Features

- **User Registration and Login**: Users can create accounts and log in securely to place orders and track their order history.

- **Browse Menu**: Users can view the restaurant's menu, which displays a list of available food items with descriptions and prices.

- **Order Placement**: Users can add items to their cart, specify the quantity, and place orders. They can also remove items from the cart if needed.

- **Order History**: Users can view their order history and check the status of their current orders.

- **Admin Dashboard**: Restaurant owners have access to an admin dashboard where they can manage menu items, view and process orders, and update order statuses.

- **Database Integration**: The website uses MySQL to store user data, menu items, and order information, ensuring data consistency and reliability.

## Usage

1. **User Registration and Login**:
   - Register as a new user by clicking the "Register" link on the login page.
   - Log in using your credentials on the login page.

2. **Browsing Menu**:
   - After logging in, you can browse the restaurant's menu by clicking the "Menu" link in the navigation menu.

3. **Placing Orders**:
   - Add food items to your cart by clicking the "Add to Cart" button on the menu page.
   - Review your cart by clicking the "Cart" link in the navigation menu.
   - Place your order and receive an order confirmation.

4. **Admin Dashboard**:
   - To access the admin dashboard, log in as an admin using the provided admin credentials (or create an admin account).
   - From the admin dashboard, you can manage menu items and process orders.

## Contributing

Contributions are welcome! If you'd like to contribute to this project, please follow these steps:

1. Fork the repository.

2. Create a new branch for your feature or bug fix.

3. Make your changes and commit them.

4. . Push your changes to your forked repository.

5. Submit a pull request to the original repository.

## 📖  How to Download the Project and Run on your PC?

### Pre-Requisites:

1. Download and Install XAMPP

[Click Here to Download](https://www.apachefriends.org/index.html)

2. Install any Text Editor (Sublime Text or Visual Studio Code or Atom or Brackets)

### Installation

1. Download as as Zip or Clone this project
2. Move this project to Root Directory
```
Local Disc C: -> xampp -> htdocs -> 'this project'
```
*Local Disk C is the location where xampp was installed*

3. Open XAMPP Control Panel and Start 'Apache' and 'MySQL'

4. Import Database

a. Open 'phpmyadmin' in your browser
b. Create a Database
c. Import the SQL file provided with this project

5. Make Changes to settings

Go to 'config' folder and Open 'constants.php' file. Then make changes on following constants
```php
<?php 
//Start Session
session_start();

//Create Constants to Store Non Repeating Values
define('SITEURL', 'http://localhost/food-order/'); //Update the home URL of the project if you have changed port number or it's live on server
define('LOCALHOST', 'localhost');
define('DB_USERNAME', 'root');
define('DB_PASSWORD', '');
define('DB_NAME', 'food-order');
    
$conn = mysqli_connect(LOCALHOST, DB_USERNAME, DB_PASSWORD) or die(mysqli_error()); //Database Connection
$db_select = mysqli_select_db($conn, DB_NAME) or die(mysqli_error()); //SElecting Database 

?>
```


