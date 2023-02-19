# docker-lemp-local

- PHP 8.1
- NGINX Latest
- MariaDB 10.6
- Redis Latest
- PhpMyAdmin Latest

- nginx (80): http://site1.localhost, http://site2.localhost, http://site#.localhost
- PhpMyAdmin (8001): http://site1.localhost:8001 ou http://localhost:8001
- Redis (6379): http://site1.localhost:6379

   
# Definir variáveis MariaDB:
    MYSQL_USER=root
    MYSQL_ROOT_PASSWORD=sua_senha_root
    MYSQL_DATABASE=seu_banco_de_dados

# Renomear pastas para o seu respectivo domínio:

- sites/html/site1.localhost
- sites/html/site2.localhost

- vhosts/sites-available/site1.localhost.conf
- vhosts/sites-available/site2.localhost.conf

# Comando para criar e subir a infraestrutura docker:
docker-compose -f docker-compose.yml up -d --build

# Comando para recriar a infraestrutura docker:
docker-compose -f docker-compose.yml up -d --build --force-recreate
