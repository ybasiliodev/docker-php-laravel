## Deploy

Para inicar o projeto, basta rodar os comandos abaixo em um ambiente com docker instalado:

```bash
  cp nome-do-projeto/.env.example nome-do-projeto/.env
  docker compose build
  docker compose up -d
  docker exec php-server composer install
  docker exec php-server php artisan config:cache
```