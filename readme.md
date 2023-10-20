initier le projet
composer create-project symfony/website-skeleton agence
iunclure Docker

modifier .env avec adresse db et mailtrap DSN
php bin/console d:d:c

git init
git add .
git commit -m message

symfony start:server

make:controller home
make:user

php bin/console make:entity User
make:auth

make:registration 
composer require symfonycasts/verify-email-bundle    

make:migration
d:m:m doctrine:migration:migration

composer require symfony/messenger

php bin/console messenger:consume async

composer require symfonycasts/reset-password-bundle

php bin/console make:reset-password

composer require symfony/mailer

symfony console make:user Admin

composer require easycorp/easyadmin-bundle

php bin/console make:admin:dashboard

php bin/console make:admin:crud 