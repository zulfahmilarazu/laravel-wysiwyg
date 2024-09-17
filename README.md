# laravel-wysiwyg
 Make WYSIWYG HTML Rich Text Editor with Laravel 11 as framework and TinyMCE as WYSIWYG plugin 

# go to https://unisharp.github.io/laravel-filemanager/installation
according to the page, i have to follow the requirements,
    run `composer require intervention/image` on terminal to add Intervention Image on this project.
once its done, lets move on to full instalation of laravel-filemanager by unisharp:
    run `composer require unisharp/laravel-filemanager`
    run `composer require intervention/image-laravel`
    run `php artisan vendor:publish --provider="Intervention\Image\Laravel\ServiceProvider"`
    run `php artisan vendor:publish --tag=lfm_config`
    run `php artisan vendor:publish --tag=lfm_public`
    optional run `php artisan route:clear`
    optional run `php artisan config:clear`
    run `php artisan storage:link`

Edit on routes/web.php

Copas this `Route::group(['prefix' => 'laravel-filemanager', 'middleware' => ['web', 'auth']], function () {\UniSharp\LaravelFilemanager\Lfm::routes();});` to routes/web.php

