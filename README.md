[![Latest Stable Version](https://poser.pugx.org/jonnitto/headline/v/stable)](https://packagist.org/packages/jonnitto/headline)
[![Total Downloads](https://poser.pugx.org/jonnitto/headline/downloads)](https://packagist.org/packages/jonnitto/headline)
[![License](https://poser.pugx.org/jonnitto/headline/license)](LICENSE)
[![GitHub forks](https://img.shields.io/github/forks/jonnitto/Jonnitto.Headline.svg?style=social&label=Fork)](https://github.com/jonnitto/Jonnitto.Headline/fork)
[![GitHub stars](https://img.shields.io/github/stars/jonnitto/Jonnitto.Headline.svg?style=social&label=Stars)](https://github.com/jonnitto/Jonnitto.Headline/stargazers)
[![GitHub watchers](https://img.shields.io/github/watchers/jonnitto/Jonnitto.Headline.svg?style=social&label=Watch)](https://github.com/jonnitto/Jonnitto.Headline/subscription)
[![GitHub followers](https://img.shields.io/github/followers/jonnitto.svg?style=social&label=Follow)](https://github.com/jonnitto/followers)
[![Follow Jon on Twitter](https://img.shields.io/twitter/follow/jonnitto.svg?style=social&label=Follow)](https://twitter.com/jonnitto)

Jonnitto.Headline Package for Neos CMS
======================================

With this package you add a headline NodeType into [Neos CMS](https://www.neos.io).  
You can choose the tagName and the style. Like that it's possible to have an `h2` with the style of an `h1`.  
Contributions are very welcome!

Installation
------------
Most of the time you have to make small adjustments to a package (e.g. configuration in Settings.yaml). Because of that, it is important to add the corresponding package to the composer from your theme package. Mostly this is the site packages located under Packages/Sites/. To install it correctly go to your theme package (e.g.Packages/Sites/Foo.Bar) and run following command:

```bash
composer require jonnitto/headline --no-update
```

The --no-update command prevent the automatic update of the dependencies. After the package was added to your theme composer.json, go back to the root of the Neos installation and run composer update. Et voilà! Your desired package is now installed correctly.



Alignment support
-----------------

If you want to add alignment support you can set the super types on the `Headline` node type:

```yaml
'Jonnitto.Headline:Headline':
  superTypes:
    'Jonnitto.Headline:AlignmentLeft': true
    'Jonnitto.Headline:AlignmentCenter': true
    'Jonnitto.Headline:AlignmentRight': true
```

If you want to get a fast overview, take a look at [Settings.yaml](Configuration/Settings.yaml) and [NodeTypes.Content.yaml](Configuration/NodeTypes.Content.yaml) in the [Configuration](Configuration) folder.


License
-------

Licensed under MIT, see [LICENSE](LICENSE)
