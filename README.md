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

	
```
Ahora vamos con cofigemail 


![cofigmail](https://user-images.githubusercontent.com/53823068/110571152-83391600-812d-11eb-8eec-19693402051b.JPG)

Cabe destacar que se tiene que configurar el correo de Gmail para usarse con aplicaciones menos “seguras” donde se nos proporciona una clave que necesitaremos luego 
```
   'driver' => env('MAIL_DRIVER', 'smtp'),
   'host' => env('MAIL_HOST', 'smtp.mailgun.org'),
   'port' => env('MAIL_PORT', 587),

   'from' => [
      'address' => env('MAIL_FROM_ADDRESS', 'hello@example.com'),
      'name' => env('MAIL_FROM_NAME', 'Example'),
      ],
   'encryption' => env('MAIL_ENCRYPTION', 'tls'),

   'username' => env('MAIL_USERNAME'),
   'password' => env('MAIL_PASSWORD'),
   //// modificaremos estos valores de nuenvo en el archivo env/// 
   MAIL_DRIVER=smtp
   MAIL_HOST=smtp.gmail.com
   MAIL_PORT=587
   MAIL_USERNAME=ejemplo@gmail.com
   MAIL_PASSWORD=claveindescifrable
   MAIL_ENCRYPTION=tls
   
```

