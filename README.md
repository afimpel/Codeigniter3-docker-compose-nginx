[TOCM]

# Dockerize Codeigniter3 App With docker-compose

## Contents
+ nginx
    + latest official version
+ php:7.4.26-fpm (official)
    + curl
    + soap
    + mysqli
    + pdo
    + pdo_mysql
+ mysql
    + latest official version
+ phpmyadmin
    + latest official version

## Test Running Application

```bash
## runing with docker compose
docker-compose -f docker-compose.yml up --build
# or run in background process 
docker-compose -f docker-compose.yml up --build -d
```

### WEBSITE
```
app running in port 8181 ---> open in browser
http://localhost:8181/
http://localhost:8181/phpinfo.php
```

### Database Admin
```
phpmyadmin running in port 8282 ---> open in browser
http://localhost:8282/
```
```php
login with username `ci` and password `ci`
```
