##  Intalation
composer install
npm install
npm run dev
php artisan migrate
php artisan serve


<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400"></a></p>

<p align="center">
<a href="https://travis-ci.org/laravel/framework"><img src="https://travis-ci.org/laravel/framework.svg" alt="Build Status"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/dt/laravel/framework" alt="Total Downloads"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/v/laravel/framework" alt="Latest Stable Version"></a>
<a href="https://packagist.org/packages/laravel/framework"><img src="https://img.shields.io/packagist/l/laravel/framework" alt="License"></a>
</p>

## About Laravel

Laravel is a web application framework with expressive, elegant syntax. We believe development must be an enjoyable and creative experience to be truly fulfilling. Laravel takes the pain out of development by easing common tasks used in many web projects, such as:

- [Simple, fast routing engine](https://laravel.com/docs/routing).
- [Powerful dependency injection container](https://laravel.com/docs/container).
- Multiple back-ends for [session](https://laravel.com/docs/session) and [cache](https://laravel.com/docs/cache) storage.
- Expressive, intuitive [database ORM](https://laravel.com/docs/eloquent).
- Database agnostic [schema migrations](https://laravel.com/docs/migrations).
- [Robust background job processing](https://laravel.com/docs/queues).
- [Real-time event broadcasting](https://laravel.com/docs/broadcasting).

Laravel is accessible, powerful, and provides tools required for large, robust applications.

## Learning Laravel

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains over 1500 video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the Laravel [Patreon page](https://patreon.com/taylorotwell).

### Premium Partners

- **[Vehikl](https://vehikl.com/)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Cubet Techno Labs](https://cubettech.com)**
- **[Cyber-Duck](https://cyber-duck.co.uk)**
- **[Many](https://www.many.co.uk)**
- **[Webdock, Fast VPS Hosting](https://www.webdock.io/en)**
- **[DevSquad](https://devsquad.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel/)**
- **[OP.GG](https://op.gg)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

## Desafio

Desaf??o 1:


Visualiza las siguientes estructuras de tablas.

    Invoice (id, date, user_id, seller_id, type)
    Product (id, invoice_id, name, quantity, price)

En base a esas estructuras, genera utilizando Eloquent, las consultas para obtener la siguiente informaci??n:

    Obtener precio total de la factura.
    Obtener todos id de las facturas que tengan productos con cantidad mayor a 100.
    Obtener todos los nombres de los productos cuyo valor final sea superior a $1.000.000 CLP.

Desaf??o 2:


Indica paso a paso los comandos para una instalaci??n b??sica de Laravel que me permita ver la p??gina principal (recuerda describir qu?? hace cada comando).


Desaf??o 3:


Respecto a la estructura de datos del desaf??o 1, agrega a "Invoice" un campo "total" y escribe un Observador (Observer) en el que cada vez que se inserter un registro en la tabla "Product", aumente el valor de "total" de la tabla "Invoice".


Desaf??o 4:


Expl??canos ??qu?? es "Laravel Jetstream"? y ??qu?? permite "Livewire" a los programadores?


Desaf??o 5:


Manos al c??digo! basado en las siguientes tablas, construye un peque??o software:


Tablas de la Base de Datos:

    users
    tasks
    logs


Los requerimientos para el software son:

Construir un CRUD, utilizar Bootstrap para el front y en las vistas el uso de Layouts en Blade.


Las funciones a desarrollar son las siguientes:

    El sistema debe permitir que los usuarios se registren y puedan iniciar sesi??n, el software no debe permitir que el correo email@hack.net se pueda registrar.
    S??lo los usuarios con sesi??n iniciada deber??an poder ver el listado de tareas (tasks)  de la plataforma en la primera pantalla luego de iniciar sesi??n.
    El sistema deber??a permitir que cualquier usuario cree una nueva tarea (tasks), esta debe contener como m??nimo la descripci??n de la tarea, el usuario asignado, la fecha m??xima de ejecuci??n.
    Cuando un usuario logueado entre a una tarea asignada a ??l, el sistema debe permitir que este agregue registros (logs) asociados a la tarea, los registros contienen como m??nimo el comentario y la fecha de este. Los usuarios no asignados a la tarea, no pueden acceder a ella, solo verla en el listado.
    Al momento de que se genere un nuevo registro (logs), es necesario que se env??e un correo electr??nico al autor de la tarea (Puedes utilizar Mailtrap para Testing, aunque lo importante no es la evidencia del env??o, sino el c??digo).
    En el listado de tareas, el sistema deber??a mostrar en rojo las tareas cuya "fecha m??xima de ejecuci??n" haya expirado respecto a hoy. 
    Recuerda usar bootstrap en el dise??o, y que puedes ingresar todas las tareas que quieras, insertando campos en la tabla tasks.
