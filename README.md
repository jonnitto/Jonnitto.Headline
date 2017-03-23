Jonnitto.Headline Package for Neos CMS
======================================

[![Latest Stable Version](https://poser.pugx.org/jonnitto/headline/v/stable)](https://packagist.org/packages/jonnitto/headline)
[![Total Downloads](https://poser.pugx.org/jonnitto/headline/downloads)](https://packagist.org/packages/jonnitto/headline)
[![License](https://poser.pugx.org/jonnitto/headline/license)](https://packagist.org/packages/jonnitto/headline)

With this package you add a headline NodeType into [Neos CMS](https://www.neos.io).  
You can choose the tagName and the style. Like that it's possible to have an `h2` with the style of an `h1`.  
Contributions are very welcome!

Alignment support
-----------------

If you want to add alignment support you can set the super types on the `Headline` node type:

```
'Jonnitto.Headline:Headline':
  superTypes:
    'Jonnitto.Headline:AlignmentLeft': true
    'Jonnitto.Headline:AlignmentCenter': true
    'Jonnitto.Headline:AlignmentRight': true
```

If you want to get a fast overview, take a look at [Settings.yaml](Configuration/Settings.yaml) and [NodeTypes.Content.yaml](Configuration/NodeTypes.Content.yaml) in the [Configuration](Configuration) folder.


License
-------
The MIT License (MIT)

Copyright (c) 2017 Jon Uhlmann

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.
