# JavaScript

## Monday Lecture Notes with Jeremy

'alt' + 'shift' + 'down' will copy the selected line of code and paste on the line(s) below.

The HTML script tag goes on the last line of the body

To test if the JavaScript file is working, use console.log().

Three ways to declare a variable
1.  let
2. const - cannot be changed. Main way to declare a variable.
3. var (not really used anymore because of scope)

For string interpolation, use backticks ``.

&& to check two conditionals
|| to check if one of the two conditionals are two.

NaN = not a number
Example: 'Jeremy' - 7 = NaN

console.group()
"will group everything inside."
console.groupEnd()


function is a piece of code that can be reused.

log + tab will create a console.log()

Putting a function inside of the function will run an endless loop
 
Hitting control + click (on a js function) will take you to the function in question.


## Tuesday Lecture Notes with Mick

Reference Data Types:
1. Array - store data by position (index) (also called lists, set)
2. Objects - store data by Key:Value pairs (great for storing mixed data types) (also called dictionaries, maps)


putting "defer" in the script tag will allow for the javascript to load last. This is useful when you want to put the script tag in the head instead of the bottom of the body. 
Example: <script src="app.js" defer></script>

Note: Arrays can hold other arrays.
Technically arrays can hold multiple data types, but this is considered bad practice.


Primitive data type are not shared. Reference data types are shared.

When we "reference" Reference types (copy them, use them) it will point back to the original
When we "reference" Primitive types, they create new data of the same value.

Looping is great for searching through an array.

"control + /" will comment out multiple lines at once.

.toFixed() will have the decimals out to a certain point 
For example: total.toFixed(2) would allow the number to round to the 2nd decimal. 


## Wednesday's Lecture Notes with Jeremy
// Gives a single value back when callback function returns true.

.find() will call every item in the array --> .find() is considered a callback function. <-- .find() predicate. Use intelliscene on vsCode for more information.

anonymous function -->  (()=>{}) or considered arrow function

// Gives an array back of items that match statement in callback 
.filter()

.forEach() essentially a for loop. check out Jeremy's animal_murder_mystery for more notes.


method is a function that exists on an object.


**Generating a random number by whole number**
Math.floor(Math.random() * array.length)

.shift() removes the first element from an array and returns it.


# Thursday's Lecture Notes with Jeremy

Try to not style the <div class=col.12>, instead create a <div> inside of the col-12. 

In HTML, you can use the marquee tag to make elements inside move. 

in CSS, you can use user-select: none; to remove the ability to highlight on the webpage

in HTML tags, using the role attribute on the button element helps readers identify it a button. 

document.querySelector('.class-name') allows you to find an HTML class

control + . on a

the forEach() just performs and action, it doesn't return a value.

setInterval(what do you want to do, how often do you want to do it)
Example: 
setInterval(() => { console.log('running interval')}, 1000)
would console.log the message every second. 

Example: 
setInterval(decreaseAnimalsHunger, 1000)
NOTE: Just put the instructions of the function, not calling the function itself.

# Monday's Lecture Notes with Jeremy
## Week 3 can be considered a one of the harder weeks in the program

### MVC - Model View Controller

View --> app.js --> Controller --> Service --> Appstate <-- Model

### View: 
HTML
DOM
index.html

html representation of the data in the app

### Controller
Takes in actions from user
draws data to dom

### Service
Business logic happens
Any thing that modifies
data goes here

### Appstate
Single Source of Truth
aka
where all the app's data will be stored

### Model
Blueprint of what the data in the appstate will look like.

In Git, you can use bcw create, to create a new project. --templates that BCW created to have prewritten code for different starter points

ctrl + p will allow you to search files by name.

A function that exists on an object is called a method

Class is a structured object within javascript.
The constructor method runs every time a class is constructed (built, newed up).

"ctrl + ." will add intellisense

Note from Jeremy's VSCode
exportconst gamersService = new GamersService
The code above will create a single service that our application interacts with (Singleton).




