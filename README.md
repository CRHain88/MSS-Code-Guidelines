# MSS-Code-Guidelines
Version 0.10.0


## Contributors
* **YOU!** - please contribute to these code guidelines! If you have any
suggestions for improvement to these guidelines, *[create an issue][issue]* to
discuss it or *create a [pull request][pr]* with your changes and discussion will
occur on that PR.

### Original Authors
* James Young [@jamsyoung](http://twitter.com/jamsyoung), [github](https://github.com/jamsyoung)
* Matt Crutchfield [@mtcrutch](https://twitter.com/mtcrutch), [github](https://github.com/mtcrutch)


## JavaScript
The JavaScript guidelines are based off of [idiomatic.js](https://github.com/rwaldron/idiomatic.js).

The MSS Guidelines will be the same with the following additional rules applied.


### Test Facility
We will be using:

* Mocha / Chai for unit tests
* Selenium (WebdriverJS) / Mocha / Chai for functional tests
* PhantomJS / CasperJS for functional tests


### Idiomatic Style Manifesto
1. Whitespace
    * 4-space soft indents are required.  This means four spaces or four spaces representing a tab.

2. Beautiful Syntax
    * 2.A - 2.C should not have `inner-space`.  Refer to 2.D for a syntax without `inner-space`.  Here is an example.
        ```javascript
        function foo(bar, baz) {
            var qux = bar + baz;

            for (i = 0; i < 10; i++) {
                console.log(qux);
            }

            if (bar === baz) {
                qux = bar * baz;
            } else {
                qux = bar / baz;
            }

            return qux;
        }
        ```

    * Single quotes must be used.

    * Object literals should look like this.
        ```javascript
        var objectLiteral;

        objectLiteral = {
            foo: 'bar',
            baz: 'qux'
        };
        ```

    * Milliseconds should be assigned in multiples of 1000, and always use explicit order of operations.
        ```javascript
        var
            oneSecond = 1000 * 1,
            oneMinute = 1000 * 60,
            fiveMinutes = (1000 * 60) * 5;
        ```


## HTML
0. Write clean semantic HTML5 markup.
0. Use double quotes for attributes.
0. Use proper indention.
0. Selector Attributes
  Never use an ID as a styling hook.
  Prefix any JavaScript class hooks with `js-`. Example: `class="js-foo foo"`
0. Closing `<li>` elements.
  `<li>` elements should not be closed. [Further reading on this inline-block issue.][inline]


## CSS / Sass
0. The CSS / Sass guidelines are based off of [csswizardry/CSS-Guidelines][css].
0. We use [nomalize.css][normalize] as our style reset.


#### Our CSS / Sass overrides
0. Declarations.
  Declarations should be in aplhabetical order (**NOT** by relevance).


## Changelog

### 0.10.0
- Added Changelog and version number

### 0.9.0
- Added if/else example in JavaScript code example

### 0.8.0
- Change to Contributors
- Added Original Authors

### 0.7.1
- Fixed typo

### 0.7.0
- Fixed typo
- Clarity on JavaScript milliseconds
- More details on HTML for quotes and whitespace

### 0.6.0
- Changed Maintainers to Contributors
- Markdown cleanup

### 0.5.0
- Updates to JavaScript code example
- Added details for JavaScript object literals
- Added details for JavaScript milliseconds

### 0.4.0
- Updates to HTML guidelines
- Updates to CSS / SASS guidelines

### 0.3.0
- Added HTML guidelines
- Added CSS / SASS guidelines

### 0.2.0
- Added exceptions over idiomatic for unit testing

### 0.1.0
- Initial version



[inline]: http://css-tricks.com/fighting-the-space-between-inline-block-elements/
[css]: https://github.com/csswizardry/CSS-Guidelines
[normalize]: http://necolas.github.io/normalize.css/
[pr]: https://github.com/TurnerBroadcasting/MSS-Code-Guidelines/compare/
[issue]: https://github.com/TurnerBroadcasting/MSS-Code-Guidelines/issues/new
