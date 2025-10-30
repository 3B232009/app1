<p align="center"><a href="https://laravel.com" target="_blank"><img src="https://raw.githubusercontent.com/laravel/art/master/logo-lockup/5%20SVG/2%20CMYK/1%20Full%20Color/laravel-logolockup-cmyk-red.svg" width="400" alt="Laravel Logo"></a></p>

<p align="center">
<a href="https://github.com/laravel/framework/actions"><img src="https://github.com/laravel/framework/workflows/tests/badge.svg" alt="Build Status"></a>
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

Laravel has the most extensive and thorough [documentation](https://laravel.com/docs) and video tutorial library of all modern web application frameworks, making it a breeze to get started with the framework. You can also check out [Laravel Learn](https://laravel.com/learn), where you will be guided through building a modern Laravel application.

If you don't feel like reading, [Laracasts](https://laracasts.com) can help. Laracasts contains thousands of video tutorials on a range of topics including Laravel, modern PHP, unit testing, and JavaScript. Boost your skills by digging into our comprehensive video library.

## Laravel Sponsors

We would like to extend our thanks to the following sponsors for funding Laravel development. If you are interested in becoming a sponsor, please visit the [Laravel Partners program](https://partners.laravel.com).

### Premium Partners

- **[Vehikl](https://vehikl.com)**
- **[Tighten Co.](https://tighten.co)**
- **[Kirschbaum Development Group](https://kirschbaumdevelopment.com)**
- **[64 Robots](https://64robots.com)**
- **[Curotec](https://www.curotec.com/services/technologies/laravel)**
- **[DevSquad](https://devsquad.com/hire-laravel-developers)**
- **[Redberry](https://redberry.international/laravel-development)**
- **[Active Logic](https://activelogic.com)**

## Contributing

Thank you for considering contributing to the Laravel framework! The contribution guide can be found in the [Laravel documentation](https://laravel.com/docs/contributions).

## Code of Conduct

In order to ensure that the Laravel community is welcoming to all, please review and abide by the [Code of Conduct](https://laravel.com/docs/contributions#code-of-conduct).

## Security Vulnerabilities

If you discover a security vulnerability within Laravel, please send an e-mail to Taylor Otwell via [taylor@laravel.com](mailto:taylor@laravel.com). All security vulnerabilities will be promptly addressed.

## License

The Laravel framework is open-sourced software licensed under the [MIT license](https://opensource.org/licenses/MIT).

a.  app1 專案定義了哪些命名空間(name space)，命名空間的基底目錄各為何？
    A:命名空間:App\                基底目錄:app/
      命名空間:Database\Factories\ 基底目錄:database/factories/
      命名空間:Database\Seeders\   基底目錄:database/seeders/

b.  app1 專案預定安裝那些必需(require)的套件&版本，
    以及app1 專案開發過程必需(require-dev)的套件&版本。      
    A:預定安裝必須:   php ^8.2 
                     laravel/framework  ^11.0
                     guzzlehttp/guzzle ^7.8
    專案開發過程必需: fakerphp/faker ^1.9.1
                     laravel/pint ^1.0
                     laravel/sail ^1.0
                     mockery/mockery ^1.4.4
                     nunomaduro/collision ^7.0
                     phpunit/phpunit" ^10.0

c.  請試著找出 laravel/framework 及 guzzlehttp/guzzle 
    兩個套件在app1專案當中的位置。
    A:vendor/laravel/framework/、vendor/guzzlehttp/guzzle/

d.  在composer.lock 檔案當中packages 區域，分別找出 laravel/framework
    及guzzlehttp/guzzle 兩個套件，請分別寫出上述兩個套件的真正安裝的版本、原始碼或網站的URL、以及各自相依那些套件。(請自行與這兩個套件的composer.json 的內容比較) 
    A:
    laravel/framework:安裝版本: 11.8.0
                      原始碼/網站URL: url: https://github.com/laravel/framework.git
                      相依套件: illuminate/*
    guzzlehttp/guzzle:安裝版本: 7.8.1
                      原始碼/網站URL: url: https://github.com/guzzle/guzzle.git
                      相依套件:guzzlehttp/promises、guzzlehttp/psr7、psr/http-client、psr/http-message

e.  請分別找出laravel/framework 及 guzzlehttp/guzzle 兩個套件定義了哪些
    命名空間(name space)，命名空間的基底目錄各為何？ 
    laravel/framework: 命名空間:Illuminate\ 
                       基底目錄:vendor/laravel/framework/src/Illuminate/
    guzzlehttp/guzzle: 命名空間:GuzzleHttp\
                       基底目錄:vendor/guzzlehttp/guzzle/src/

f.  請開啟app1專案當中的AppServiceProvider類別，位於
    /app/HTTP/Providers/AppServiceProvider.php，請說出此類別在怎樣的namespace當中。
    A:此類別的命名空間為 App\Providers

g.  上述Controller 類別使用(use)了哪些其他命名空間的類別，你可以找出這些類別
    在那個套件、以及套件當中的位置 (找到後可開啟他們的程式碼欣賞一下)。(提示；滑鼠移動到那些類別，Phpstorm會提示你)
    A:使用的類別:Illuminate\Foundation\Auth\Access\AuthorizesRequests
      所屬套件:laravel/framework
      套件位置:vendor/laravel/framework/src/Illuminate/Foundation/Auth/Access/
      -
      使用的類別:Illuminate\Foundation\Validation\ValidatesRequests
      所屬套件:laravel/framework
      套件位置:vendor/laravel/framework/src/Illuminate/Foundation/Validation/
      -
      使用的類別:Illuminate\Routing\Controller
      所屬套件:laravel/framework
      套件位置:vendor/laravel/framework/src/Illuminate/Routing/Controller.php