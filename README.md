# README

## how to reproduce the bug

- `composer install --ignore-platform-reqs`
- `docker compose up`
- open a shell inside the PHP container
- `XDEBUG_MODE=off bin/console doctrine:database:create`
- `XDEBUG_MODE=off bin/console make:migration`
- `XDEBUG_MODE=off bin/console doctrine:migrations:migrate`
- `XDEBUG_MODE=off bin/console doctrine:fixtures:load`
- see the hell of reserved keywords in action
