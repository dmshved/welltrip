<p align="center">
<img src="https://thumbs2.imgbox.com/ab/30/vdZyHVFO_t.png" alt="">
</p>

<h1 align="center">Welltrip API</h1>

<h2 align="center">
    Welltrip is an implementation of task from a real job interview
</h2>

The full version of this task: [Laravel hiring test](https://docs.google.com/document/d/1IqsnOB6sjoSEcgmjqHPhb58Ym-82x5jKDDxvTWeQsL0/edit?pli=1&tab=t.0)

### The short version of the goals

- DB structure (image at the end of this list)
- Get the list of public & paginated travels: /travels
- Get the list of paginated tours: /travels/{travel-slug}/tours
- Tours filtering and ordering by: priceFrom, priceTo, dateFrom, dateTo
- Roles (admin & editor)
- Create users artisan command
- Admin endpoint: create new travels, with middleware role:xxxxx
- Admin endpoint: create new tours for travels
- Editor endpoint: update travel
- Automated Tests with [Pest](https://pestphp.com/)
- API Documentation with [Scribe](https://scribe.knuckles.wtf/laravel/)


<p align="center">
    <img src="https://images2.imgbox.com/af/7c/XMJcYKdQ_o.png" alt="welltrip_db">
</p>

### Installation

- Clone the repository

```
https://github.com/dmshved/welltrip.git
```

- Copy `.env.example` file to `.env` and edit database credentials there

```
copy .env.example .env
```

- Install dependencies

```
composer install
npm install
```

- Generate key

```
php artisan key:generate
```

- Run migrations

```
php artisan migrate
```

- Seed the database with test data (runs the roles seeding)

```
php artisan db:seed
```

- Run the application

```
php artisan serve 
```

- Create a user using artisan command

```
php artisan users:create 
```
