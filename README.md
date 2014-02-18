## Basset for Laravel 4

[![Build Status](https://secure.travis-ci.org/jasonlewis/basset.png)](http://travis-ci.org/jasonlewis/basset)

Basset is a better asset management package for the Laravel framework. Basset shares the same philosophy as Laravel. Development should be an enjoyable and fulfilling experience. When it comes to managing your assets it can become quite complex and a pain in the backside. These days developers are able to use a range of pre-processors such as Sass, Less, and CoffeeScript. Basset is able to handle the processing of these assets instead of relying on a number of individual tools.

### Installation

- [Basset on Packagist](https://packagist.org/packages/jasonlewis/basset)
- [Basset on GitHub](https://github.com/jasonlewis/basset)

To get the latest version of Basset simply require it in your `composer.json` file.

~~~
"jasonlewis/basset": "dev-master"
~~~

You'll then need to run `composer install` to download it and have the autoloader updated.

> Note that once Basset has a stable version tagged you should use a tagged release instead of the master branch.

Once Basset is installed you need to register the service provider with the application. Open up `app/config/app.php` and find the `providers` key.

~~~
'providers' => array(
    
    'Basset\BassetServiceProvider'

)
~~~

Basset also ships with a facade which provides the static syntax for creating collections. You can register the facade in the `aliases` key of your `app/config/app.php` file.

~~~
'aliases' => array(

    'Basset' => 'Basset\Facade'

)
~~~

### Documentation

[View the official documentation](http://jasonlewis.me/code/basset/4.0).
