<h2>Step 1: Install Laravel</h2>
 <i>composer create-project laravel/laravel example-app</i>

<h2>Step 2: Setup Database Configuration</h2>
<i>
.env

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=Enter_Your_Database_Name
DB_USERNAME=Enter_Your_Database_Username
DB_PASSWORD=Enter_Your_Database_Password
</i>

<h2>Step 3: Install Auth Scaffold</h2>
Laravel's laravel/ui package provides a quick way to scaffold all of the routes and views you need for authentication using a few simple commands: <br>
<i>
composer require laravel/ui
</i>
<br>

Next, we need to generate auth scaffold with bootstrap, so let's run the below command: <br>
<i>
php artisan ui bootstrap --auth
</i>
<br>
Then, install npm packages using the below command: <br>
<i>
npm install
</i>
<br>
At last, built bootstrap CSS using the below command: <br>
<i>
npm run build
</i>


<h2>Step 4: Install Cashier Package</h2>
Laravel's laravel/ui package provides a quick way to scaffold all of the routes and views you need for authentication using a few simple commands: <br>
<i>
composer require laravel/cashier
</i>
<br>
Next, we need to publish cashier migration for creating tables, so let's run the below command: <br>
<i>
php artisan vendor:publish --tag="cashier-migrations"
</i>

<br>
Then, run the migration command to create a table using the below command:<br>
<i>
php artisan migrate
</i>


<h2>Step 5: Create Stripe Account & Get Stripe API Key and SECRET</h2>
This step is a very important step, if you don't have a stripe account then you need to create and if you have then proceeded to get Stripe Key and Secret. So, Let's open below stripe official website using the below link:

1) Open <a href="https://stripe.com/en-in">Stripe official website</a>

⚠ Strip supports 47 different countries and 2 are coming soon, but unfortunately Stripe doesn't support Morroco, so my example stopped here
<br>


