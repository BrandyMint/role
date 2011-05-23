# jquery.role — jQuery plugin to provide easy way to handle DOM elements by role attribute

This project uses [Semantic Versioning](http://semver.org/) for release numbering.

## Idea behind this piece of code

I start using role attrbute (`<div role="role_name"></div>`) to handle DOM elements.

![Y U NO USE CLASSES?](https://github.com/kossnocorp/jquery.role/raw/master/doc/yuno.png)

Some reasons:

* Markup-guys always change classes and class names (and this is normally)
* It's hard to know this class is used for JavaScript or not?
* And finally: semantic

But what wrong with id's? Isn't usage of id's is more faster than class or attributes?

Id is ok, but it uses for styles to. So why not use prefix? For example `role-id_name`.

## Usage

### Basic

``` javascript
$.role('login_form'); // To handle <form role="login_form"></form>
```

or via alias `$.r`:

``` javascript
$.r('login_form');
```

### Pick by element id

``` javascript
$.r('#login_form'); // To handle <form id="role-login_form"></form>
```

### With context

``` javascript
$.r('submit', loginForm); // To handle <a href="#" role="submit"></a> inside loginForm element
```

## Changelog

### 0.2.0 (May 20, 2011)

* Added mechanism to pick roles by element id

### 0.1.0 (May 05, 2011)

* Initial release

## Contributors

Idea by @kossnocorp and @ai.

* @kossnocorp
* @chrome

## License

The MIT License

Copyright (c) 2011 Sasha Koss

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
