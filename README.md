# Functions & Scopes Workshop

You're here to solidify your understanding of Functions & Scopes in JavaScript.

*IMPORTANT*: Completion of this workshop is no guarantee of admission into the Hack Reactor immersive program, nor does it have any influence in the admissions process.

## Prerequisites

It is recommended that students understand JavaScript variables, if/else statements, loops, objects, arrays and functions prior to this course; however it is not required. Students should have approximately 2 months of experience with JavaScript and programming.

## Textbook

No textbook is required for this course. All materials are included in this GitHub repo.

## Technical requirements

Laptop, Google Chrome browser and a text editor. If you do not have a text editor, we recommend Sublime Text, Atom or Visual Studio Code.

# How to use this repository

#### It is your mission to go through the function.js file and change all the `'???'` in such a way that all the tests pass true.

### Let's get started...

Run the specrunner.html file in a browser. This document shows one passed test and a series of failing tests.

The **functions.js** folder holds all the failing tests that are being displayed in **SpecRunner.html**. You will be editing this file and using the **SpecRunner.html** to check your progress on making these tests pass. This is just a javascript file so you can use console.log to help debug and inspect these functions.

A test block starts with an `it` function. The `it` function takes two arguments. The first one is a statement describing the rule addressed by the test. The second is a function that will either evaluate to true or false using the `expect` function. The expect statement (`expect(ACTUAL === 'inner').to.be.true;`) will evaluate if the statement between the parens `ACTUAL === 'inner'` is true. You can almost read it like plain English. The expect statement below "expects that the variable ACTUAL equals the value 'inner' to be true".

#### Failing Test Example

      it('a function has access to its own local scope variables',

      function () {
        var fn = function () {
          var name = 'inner';
          ACTUAL = name;
        };
        fn();
        expect(ACTUAL === '???').to.be.true;
        //change '???' to what ACTUAL evaluates to.
      });

#### Passing Test Example

      it('a function has access to its own local scope variables',

      function () {
        var fn = function () {
          var name = 'inner';
          ACTUAL = name;
        };
        fn();
        expect(ACTUAL === 'inner').to.be.true;
        //changed '???' to 'inner'
        //(because we assigned ACTUAL, a global variable to name inside fn)
      });

### Don't forget..
To read all code to try to understand how the whole testing process works. Welcome to programming :)
