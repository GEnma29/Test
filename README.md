# Test
prueba de desarollo en PHP 
Desafio 1 para esto devemos ir al archivo config 

![configdatabase](https://user-images.githubusercontent.com/53823068/110564471-41a36d80-8123-11eb-861f-224537842474.JPG)

Ahora laravel nos da una guía donde definimos el tipo de motor con el cual trabajaremos, en nuestro caso Mysql para configurar nuestra base de datos nos vamos al archivo env este archivo obviamente será ignorado por git para mantener los datos sensibles privados 
```php
    'default' => env('DB_CONNECTION', 'mysql'),
    /////////////////////////////////////////////////////////////////////////////////
        'mysql' => [
            'driver' => 'mysql',
            'url' => env('DATABASE_URL'),
            'host' => env('DB_HOST', '127.0.0.1'),
            'port' => env('DB_PORT', '3306'),
            'database' => env('DB_DATABASE', 'forge'),
            'username' => env('DB_USERNAME', 'forge'),
            'password' => env('DB_PASSWORD', ''),
            'unix_socket' => env('DB_SOCKET', ''),
            'charset' => 'utf8mb4',
            'collation' => 'utf8mb4_unicode_ci',
            'prefix' => '',
            'prefix_indexes' => true,
            'strict' => true,
            'engine' => null,
            'options' => extension_loaded('pdo_mysql') ? array_filter([
                PDO::MYSQL_ATTR_SSL_CA => env('MYSQL_ATTR_SSL_CA'),
            ]) : [],
        ],
        
        //////////////// archivo env/////////////////////////////////////
        
        APP_NAME=Laravel
        APP_ENV=local
        APP_KEY=base64:QYo9eXwlyhHHMzhxEcDI3eQW5Ae0GKsVtoHCjoe2JGo=
        APP_DEBUG=true
        APP_URL=http://j-livewire-8.test

        LOG_CHANNEL=stack
        LOG_LEVEL=debug

        DB_CONNECTION=mysql
        DB_HOST=127.0.0.1
        DB_PORT=3306
        DB_DATABASE=j_livewire_8
        DB_USERNAME=root
        DB_PASSWORD=

       BROADCAST_DRIVER=log
       CACHE_DRIVER=file
       QUEUE_CONNECTION=sync
       SESSION_DRIVER=database
       SESSION_LIFETIME=120

       MEMCACHED_HOST=127.0.0.1

       REDIS_HOST=127.0.0.1
       REDIS_PASSWORD=null
       REDIS_PORT=6379

       MAIL_MAILER=smtp
       MAIL_HOST=mailhog
       MAIL_PORT=1025
       MAIL_USERNAME=null
       MAIL_PASSWORD=null
       MAIL_ENCRYPTION=null
       MAIL_FROM_ADDRESS=null
       MAIL_FROM_NAME="${APP_NAME}"

       AWS_ACCESS_KEY_ID=
       AWS_SECRET_ACCESS_KEY=
       AWS_DEFAULT_REGION=us-east-1
       AWS_BUCKET=

       PUSHER_APP_ID=
       PUSHER_APP_KEY=
       PUSHER_APP_SECRET=
       PUSHER_APP_CLUSTER=mt1

       MIX_PUSHER_APP_KEY="${PUSHER_APP_KEY}"
       MIX_PUSHER_APP_CLUSTER="${PUSHER_APP_CLUSTER}"

		
		```
