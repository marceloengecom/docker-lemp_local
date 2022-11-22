# docker-lemp-local

- PHP 8.1
- NGINX Latest
- MariaDB 10.6
- Redis Latest
- PhpMyAdmin Latest


nginx (80) : http://localhost
PhpMyAdmin (8000) : http://localhost:8001
Redis (6379) : http://localhost:6379
site1.localhost: http://site1.localhost


MySql & PhpMyAdmin Credential
user : root
password : root_password


# Comando para criar e subir a infraestrutura docker:
docker-compose -f docker-compose.yml up -d --build

# Comando para recriar a infraestrutura docker:
docker-compose -f docker-compose.yml up -d --build --force-recreate