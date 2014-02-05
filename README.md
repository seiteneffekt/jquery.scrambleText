jquery.scrambleText
===================

jQuery plug-in that scrambles a given text randomly but keeps it surprisingly readable

## Features

* standard jQuery plug-in
* scramble any set of (text) elements
* configurable regex

## Usage

```js
$('p').scrambleText();
```

## Configuration

You can optionally configure the plug-in to set another regular expression to sepearte your text in single words, e.g. to allow special characters (see demo.html with German text).

```js
$('h1, p').scrambleText({
  regex: /[A-Za-zÄÖÜäöüß]+/g
});
```

## Known problems

Cascaded HTML elements (e.g. inner _span_ elements or formattings with _strong_) get lost.

## License

This plugin is released under the [MIT License](http://en.wikipedia.org/wiki/MIT_License). Feel free to use it in personal and commercial projects.