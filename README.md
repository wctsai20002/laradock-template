# Laradock-Template

### Required
- PHP 7.2+
- Docker
- Docker-compose
- Composer
- Laravel
- Yarn

### Clone
```
   git clone https://github.com/wctsai20002/laradock-template.git --branch master
   cd laradock-template
```

### Init submodule
```
   git submodule update --init
   cd laradock/
   cp env-example .env
```

### Start laradock
```
   docker-compose up -d nginx mysql workspace redis mail-dev php-fpm
   docker-compose exec --user=laradock workspace bash
   composer install
   yarn
   cp .env.example .env
```

### Generate key
```
   php artisan key:generate
```

### Important
```
    you may need to modify .env file for your environment
```
