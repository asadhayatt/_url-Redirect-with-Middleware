There are 2 files 

1- Redirect.php
2- .htaccess


Step # 1

    create a middleware name Redirect using command : 

    => php artisan make:middleware Redirect

    Paste Redirect.php files in your middleware before given command:

    => return $next($request);

    inside handle function 
    public function handle(Request $request, Closure $next): Response{}


Step # 2

Replace .htaccess file with your file. It is globally same in every laravel built-in project.


#   _ u r l - R e d i r e c t - w i t h - M i d d l e w a r e  
 