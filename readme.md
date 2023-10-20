initier le projet
composer create-project symfony/website-skeleton agence
iunclure Docker

modifier .env avec adresse db et mailtrap DSN
php bin/console d:d:c

git init

symfony start:server

make:controller home
make:user

php bin/console make:entity User