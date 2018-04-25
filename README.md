# siskel
This is a project I completed as a student at [hackreactor](http://hackreactor.com). This project was worked on with a pair.

Siskel is a simple movie rating app. We'll be using this app to explore backbone events and how they relate to MVC components. In particular, you will explore the following ideas:
* Controllers translate click events into intention (invoking a model function)
* Models effect state changes in other models (by broadcasting events)
* Views update as a result of model changes (by listening for changes)

## Environment
Requirements
* Bower 1.3.x
Install Dependencies
* bower install

## Objective
The Siskel app allows the user to 'like' or 'unlike' a movie and to sort the list of movies by various fields (title, year, rating and the user's like status). The app has most of the necessary structure, but is is missing all the functionality that enables sorting and liking to work as you would expect. Your objective is to implement these features by connecting modules together in a way that enables correct behavior.

## Context
At the heart of this exercise is understanding backbone events. The documentation provides an extensive list of built-in events. The two that are most important for this exercise are change and sort.

[Backbone Events](http://backbonejs.org/#Events-catalog)

Backbone will automatically keep a collection sorted if a comparator property is specified. The property can either be a string or a function. When specified as a string, the collection will use that string to look up that property on each item contained in the collection and then sort itself based on the property value (ex: item[comparator]).

[Collection Comparator](http://backbonejs.org/#Collection-comparator)

While a collection does keep itself sorted, there are times when you have to manually re-sort. This can be accomplished by invoking sort(). This assumes you have specified a comparator.

[Collection Sorting](http://backbonejs.org/#Collection-sort)

## Bare Minimum Requirements
* Make the tests pass.
* The tests are written in a way that guides you to make the right connections. You should read the test source code to ensure you are understanding what the goal of each test is.