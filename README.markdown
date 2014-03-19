PROTO.js

About Proto:

Proto.js is a library full with helpers and shared funcitons within the HTML Object Elements.
The philosophy behind use a prototype-based script is that this way you don't have to create a custom object each time you need a Element to have the library-features.

Imagine you need to make a querySelectorAll and you want to add a event to the whole NodeList. In JQuery you will have to make that NodeList a JQuery-Object.

var buttons = document.querySelectorAll('.popUpButtons');

$(buttons).on('click',doSomething);

or more easy-

var buttons = $('.popUpButtons');

buttons.on('click',doSomething);


Either way you will have to wrapp that NodeList with a lot of Jquery Functions that you will not use.

If the prototype is global to all NodeList objects, then this can be avoided.

How to add an event in Proto.js

var buttons = document.get('.popUpButtons');

buttons.addEvent('click',doSomething);

** Notice how proto.js use the method .get() in order to grab the elements that match with the selector.
** It works as fine as JQuery, but again, you do not need a custom Object type.


All rights reserverd 2013