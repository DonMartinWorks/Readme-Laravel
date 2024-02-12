<a name="readme-top"></a>

# Presentación

Este proyecto es una aplicación de punto de ventas (POS [Point of Sale]).

## Funcionalidades

-   Autenticación de usuarios.
-   Roles y permisos.
-   Subida de imágenes.
-   Cambio de contraseña y sus datos.
-   Generación de PDF.
-   Inventario de productos.
-   Generación de ID y códigos de barras.
-   Exportación de datos en Excel.
-   Respaldo de datos DB (Backup).

#### Programas utlizados

-   [Laragon](https://laragon.org/)
-   [Node](https://nodejs.org/en)
-   [VS Code](https://code.visualstudio.com/)

#### Paquetes utlizados

-   [Laravel](https://laravel.com/)
-   [Breeze](https://laravel.com/docs/10.x/starter-kits)

<br />

# Instalación de manera local

## Archivo .env

#### Que es este archivo

_El archivo `.env` en Laravel es un archivo de configuración que almacena variables de entorno para una aplicación. Estas variables se utilizan para configurar la aplicación en diferentes entornos, como desarrollo, pruebas y producción. El archivo `.env` se utiliza para almacenar información confidencial, como contraseñas de bases de datos, claves de API y credenciales de correo electrónico, que no deben ser compartidas en el código fuente de la aplicación. En su lugar, se almacenan en el archivo `.env` y se acceden a través de la función env en Laravel._

### Credenciales

_Al clonar este proyecto ve al archivo *.env.example* copia este archivo con el nombre de: `.env` y coloca tus credenciales, que coincidan con tu DB, Email_

-   Ejemplo de credenciales para la DB, asegurate que coincidan con tu tipo de conexión para tu DB.

```bash
  DB_CONNECTION=mysql
  DB_HOST=
  DB_PORT=
  DB_DATABASE=dbname
  DB_USERNAME=username
  DB_PASSWORD=password
```

#### Mailtrap

_Puedes utlizar cualquier paquete de envio de emails por api, pero te recomiendo el uso de <a href="https://mailtrap.io/">`Mailtrap`</a>_

1- _Primero debes crear una cuenta, después crea un inbox, en la sección SMTP Settings > SMTP / POP3 > en Integrations pon Laravel 9+_
2- _Coloca estas credenciales en tu archivo `.env` reemplazando desde la linea `31 a la 35`._

```bash
    MAIL_MAILER=smtp
    MAIL_HOST=sandbox.smtp.mailtrap.io
    MAIL_PORT=2525
    MAIL_USERNAME=
    MAIL_PASSWORD=
```

# Comandos

## Comandos de Instalación

-   _La instalación de este proyecto necesita que se ejecuten de manera cronológica y ordenada._

Instalación de los paquetes _Composer_

```bash
  composer install
```

Instalación de los paquetes _Node_

```bash
  npm install
```

Construcción de los paquetes _Node_

```bash
  npm run build
```

Generación de la _llave_ del proyecto

```bash
  php artisan key:generate
```

Generación de la _DB_

```bash
  php artisan migrate
```

Utilización del _Seeder_

```bash
  php artisan db:seed
```

<br />

_Listado de comandos que podrian ser necesarios_

-   Limpieza de caché (events/views/cache/route/config/compiled)

    ```
     php artisan optimize:clear
    ```

-   Creacion de los links de los archivos estaticos

    ```
    php artisan storage:link
    ```

-   Actualización de la información del cargador automático de clases.

    ```
    composer dump-autoload
    ```

## Comandos DB/(SQL)

_Listado de comandos DB_

-   Reinicia desde cero la DB y crea los seeders

    ```
     php artisan migrate:fresh --seed
    ```

-   Revierte la/s última/s migración/es

    ```
     php artisan migrate:rollback
    ```

<br />

# Servidor local

_El funcionamiento de esta aplicacion requiere que este levantado de manera simultanea._

## Servidores

_Para levantar este servicio debes estar en la carpeta donde esta este proyecto, debe ser ejecutado con CMD y de manera simultanea el servidor backend y frontend._

```bash
  cd NewsWorld
```

### Backend

```bash
  php artisan serve
```

### Frontend

```bash
  npm run dev
```

<br />

# Contacto

Mi Cuenta GitHub: [https://github.com/DonMartinWorks](https://github.com/DonMartinWorks)

<a href="#readme-top">Subir a las instrucciones</a>