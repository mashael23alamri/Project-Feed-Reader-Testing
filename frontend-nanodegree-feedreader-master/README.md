# Feed-Reader---Testing
Feed-Reader-Testing ْUdacity

------------------------------------------------------------------------
## what is Jasmine?
Jasmine is the most popular JS library for unit testing web apps.

Jasmine is , a popular behavior-driven testing framework for JavaScript , which can help you easily check for bugs in your code.

------------------------------------------------------------------------
## Jasmine has many features such as:

1-It’s fast and has low overhead and no external dependencies.

2-It’s a batteries included library and offers everything you need for testing your code.

3-It’s available both for Node and the browser.

4-It can be used with other languages like Python and Ruby.

5-It does not require the DOM.

6-It provides a clean and easy to understand syntax and also a rich and straightforward API.

7-We can use natural language to describe the tests and the expected results.

------------------------------------------------------------------------
## Method of embedding Jasmine inside the project:
In this project Jasmine was used by a modulation Jasmine core and test files using a <script> tag.
```html
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/jasmine/3.3.0/jasmine.min.css">

        <script src="https://cdnjs.cloudflare.com/ajax/libs/jasmine/3.3.0/jasmine.min.js"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/jasmine/3.3.0/jasmine-html.min.js"></script>
        <script src="https://cdnjs.cloudflare.com/ajax/libs/jasmine/3.3.0/boot.min.js"></script>
```
------------------------------------------------------------------------
## Simple explanation of how the test works + include an example of the project:

Specs are defined by calling the global Jasmine function ( it ), 
which like describe takes a string and a function.
The string is the title of the spec and the function is the spec or test.
A spec contains one or more expectations that test the state of the code.
An expectation in Jasmine is an assertion that is either true or false. A spec with all true expectations is a passing spec.
A spec with one or more false expectations is a failing spec.

Expectations are built with the function expect which takes a value, called the actual.
It is chained with a Matcher function, which takes the expected value.

## Example :
```js
$(function() {
    /* This is our first test suite - a test suite just contains
    * a related set of tests. This suite is all about the RSS
    * feeds definitions, the allFeeds variable in our application.
    */
    describe('RSS Feeds', function() {
        /* This is our first test - it tests to make sure that the
         * allFeeds variable has been defined and that it is not
         * empty. Experiment with this before you get started on
         * the rest of this project. What happens when you change
         * allFeeds in app.js to be an empty array and refresh the
         * page?
         */

         //Make sure there is Feeds ...
        it('are defined', function() {
            expect(allFeeds).toBeDefined();
            expect(allFeeds.length).not.toBe(0);
        });
}());
```
------------------------------------------------------------------------
# Resources
- [link to site jasmine](https://jasmine.github.io/index.html) 
- [link to  site jquery](https://jquery.com/)   
- [link to  site freecodecamp](https://www.freecodecamp.org/news/jasmine-unit-testing-tutorial-4e757c2cbf42/) 
