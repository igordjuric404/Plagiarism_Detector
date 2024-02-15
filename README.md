## Project Record - ITEH project

## Initial settings before starting the project

## 1. Cloning the repository

git clone https://github.com/elab-development/internet-tehnologije-projekat-evidencijaradova_2020_0180

## 2. Entering the project directory

cd internet-tehnologije-projekat-evidencijaradova_2020_0180

## 3. Installing Composer

cd laravel
composer install

## 3.1 In case of an error, allow the extension in the php.ini file, delete the ; in front of the extension

;extension=sodium => extension=sodium

## 4. Copying the .env configuration file

cp .env.example .env

## 5. Generating encryption keys

php artisan key:generate

## 9. Creating an empty database for the application

Create an empty database for the project on the phpmyadmin page with the name from the .env file

## 6. Migrating and populating the database

php artisan migrate
php artisan db:seed

## 7. Installation of laravel/passport dependencies needed for authentication

php artisan passport:install

## 8. Installing NPM dependencies

cd ../react-frontend
npm install

## Additional settings for launching the project

## 1. Start the laravel server from the laravel folder

php artisan serve

## 2. Start the react server from the rect folder

npm run start
