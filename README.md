## Inventory Management System

## Features
- POS
- Orders
  - Pending Orders
  - Complete Orders
  - Pending Due
- Purchases
  - All Purchases
  - Approval Purchases
  - Purchase Report
- Products
- Customers
- Suppliers


## Instalation

1.  **Clone Repository or Download**

1. **Setup**
    ```bash
    # Go into the repository
    $ cd inventory-management-system

    # Install dependencies
    $ composer install

    # Open with your text editor
    $ code .
    ```
1. **.ENV**

    Rename or copy the `.env.example` file to `.env`
    ```bash
    # Generate app key
    $ php artisan key:generate
    ```
1. **Custom Faker Locale**

    To set Faker Locale, add this line of code to the end `.env` file.
    ```bash
    # In this case, the locale is set to Indonesian

    FAKER_LOCALE="id_ID"
    ```

1. **Setup Database**

    Setup your database credentials in your `.env` file.

1. **Seed Database**
    ```bash
    $ php artisan:migrate:fresh --seed

    # Note: If showing an error, please try to rerun this command.
    ```
1. **Create Storage Link**

    ```bash
    $ php artisan storage:link
    ```
1. **Run Server**

    ```bash
    $ php artisan serve
    ```
1. **Login**

    Try login with username: `admin` and password: `password`

## Config
1. **Config Chart**

    Open file `./config/cart.php`. You can set a tax, format number, etc.
    > For More details, visit this link [hardevine/shoppingcart](https://packagist.org/packages/hardevine/shoppingcart).