# Parts — Laravel Online Store

An online store on Laravel 8: catalog with product variants, cart and checkout, user accounts and an admin panel.

## Live Preview

Not deployed — the store needs PHP and MySQL, so run it locally (see Getting Started).

## Technologies Used

- PHP 8, Laravel 8
- MySQL
- Blade templates, Bootstrap 5
- Laravel Mix

## Getting Started

You need PHP 8, Composer, MySQL, Node.js and npm installed.

```bash
git clone https://github.com/nester02/Parts02.git
cd Parts02
composer install
cp .env.example .env
php artisan key:generate
```

Set the database name, user and password in `.env`, then:

```bash
php artisan migrate --seed
npm install
npm run dev
php artisan serve
```

The store opens at http://localhost:8000.

## Features

- Catalog: categories, products and product variants (SKUs) built from properties and their options
- Cart and checkout, discount coupons
- Two languages (English, Russian) and several currencies, switched from the header
- "Notify me" subscription when an out-of-stock variant is back
- Registration and login, order history in the user account
- Admin panel: orders, and create/edit/delete for categories, products, variants, properties, coupons and merchants
- API for merchants with access tokens
