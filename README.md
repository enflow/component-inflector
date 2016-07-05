# Singularize and pluralize words in multiple languages

[![Latest Version on Packagist](https://img.shields.io/packagist/v/enflow/component-inflector.svg?style=flat-square)](https://packagist.org/packages/enflow/component-inflector)
[![Software License](https://img.shields.io/badge/license-MIT-brightgreen.svg?style=flat-square)](LICENSE.md)
[![Build Status](https://img.shields.io/travis/enflow-nl/component-inflector/master.svg?style=flat-square)](https://travis-ci.org/spatie/component-inflector)
[![Total Downloads](https://img.shields.io/packagist/dt/enflow/component-inflector.svg?style=flat-square)](https://packagist.org/packages/enflow/component-inflector)

The `enflow/component-inflector` package provides a easy way to singularize and pluralize words in multiple languages.   
   
The following languages are (currently) supported:
- English
- Dutch
  
Component is based on [`cakephp/utility`](https://github.com/cakephp/utility) and [`noud/cakephp-dutch`](https://github.com/noud/cakephp-dutch).

## Installation
You can install the package via composer:

``` bash
composer require enflow/component-inflector
```

## Usage
``` php
$inflector = new \Enflow\Component\Inflector\Inflector();

echo $inflector->singularize('apples') // Outputs: apple
echo $inflector->pluralize('apple') // Outputs: apples
```
Or specify a custom inflection (language), Dutch for instance:
``` php
$inflector = new \Enflow\Component\Inflector\Inflector(new \Enflow\Component\Inflector\Inflections\Dutch());

echo $inflector->singularize('appels') // Outputs: appel
echo $inflector->pluralize('appel') // Outputs: appels
``` 

## Testing
``` bash
$ composer test
```

## Contributing
Please see [CONTRIBUTING](CONTRIBUTING.md) for details.

## Security
If you discover any security related issues, please email michel@enflow.nl instead of using the issue tracker.

## Credits
- [Michel Bardelmeijer](https://github.com/mbardelmeijer)
- [All Contributors](../../contributors)
   
Special thanks to [Freek Van der Herten](https://github.com/freekmurze) for providing the package template & multiple useful packages.

## About Enflow
Enflow is a web agency based in Alphen aan den Rijn, Netherlands. We specialize in developing webapplications, mobile applications and websites. You can find more info [on our website](https://enflow.nl/en).

## License
The MIT License (MIT). Please see [License File](LICENSE.md) for more information.
