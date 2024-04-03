## Run the application
**Note**: Make sure you install composer and PHP on your device. If you haven't, follow the instructions below:
- [Composer](https://www.geeksforgeeks.org/how-to-install-php-composer-on-windows/).
- [PHP](https://www.geeksforgeeks.org/how-to-install-php-in-windows-10/).

If you have composer and php installed on your device, follow the instructions below.
1. Clone the repository

2. Import voguish_online_shop database to phpmyadmin

3. Install composer to your project repository

```bash
composer install
```

4. Copy the `.env` file:

```bash
copy .env.example .env
```

5. Update the `.env` database section with your voguish_online_shop database credentials:

```bash
DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=voguish_online_shop
DB_USERNAME=root
DB_PASSWORD=
```

6. Generate Application Key

```bash
php artisan key:generate
```

7. Run the migrations:

```bash
php artisan migrate
```

8. Start the server:

```bash
php artisan serve
```

9. Go to [http://localhost:8000](http://localhost:8000)
