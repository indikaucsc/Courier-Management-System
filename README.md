# Instalation in 5 steps 

git clone https://github.com/taboritis/coreui-laravel.git
cd coreui-laravel
composer install
cp .env.example .env
php artisan key:generate


You have to register and login to app (database needed)
If you are user MySQL you can paste this to your .env file:

DB_CONNECTION=mysql
DB_HOST=127.0.0.1
DB_PORT=3306
DB_DATABASE=coreui
DB_USERNAME=root
DB_PASSWORD=


To create table in database
	php artisan migrate
(or to create table with exemplary user 'John Doe')

	php artisan migrate:fresh --seed
That's all. Enjoy.
Change log
v 1.0.6a
v 1.0.6

Update to CoreUI 1.0.6
In gulpfile.js prepared scripts to import libraries and app files to /public directory
