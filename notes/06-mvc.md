# MVC

# Monday's Lecture Notes with Jeremy
#### Week 3 can be considered a one of the harder weeks in the program

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

# Tuesday's Lecture Notes with Jeremy

When thinking about starting a MVC program, consider building a controller with a console.log to see if it works. 

When creating a controller file, make it plural. 

Blueprint example for controller

export class GachamonsController {
    constructor (){
        NOTE: this will run on page load.
    }
}

NOTE: Make sure the controller is loaded in the router.

AppState stores all of the data

A model is a blueprint to use to not break your data. Look at Jeremy's Gachamon.js inside of the Model folder for example. 

Inside of HTML, if you want to change something (like a emoji) as a button, you can use role = "button" to change the cursor to a pointer. 

TOOL: debugger is a great tool to use when debugging your code. 

AppState.on(event, function)



# Wednesday's Lecture Notes with Jeremy

## Application: Gregslist

Bootstrap has some great options for forms that you can utilize and modify for your own use.

**A handful of notes on Jeremy's repo**

Handle local storage inside of the Service.js
In util folder, the Store.js handles local storage.



# Thursday's Lecture Notes with Mick

If you make changes in Sass, you need to compile it to css. 
Go to your terminal  and type --> npm run sass

When working in MVC, consider starting with the model/data. 

Cool feature: selectable

When trying to use local storage: 

saveCaseFiles() {
    saveState('', AppState.caseFiles)
}

loadCaseFiles() {
    AppState.caseFiles = loadState('', [Class])
    
}

# Monday June 24th: Lecture Notes with Jeremy

## APIs

API stands for Application Programming Interface
In the context of APIs, the word Application refers to any software with a distinct function. Interface can be thought of as a contract of service between two applications. 

When debugging, use the Network tab in the inspect tools

Example with Google.com:
Request Method: GET
Status Code: 200 OK

JSON - JavaScript Object Notation

Status Code: 404 - Not Found

https://http.cat Helps with status codes.

Use controller when sending a get request to an API

Within JavaScript, you can use "fetch" to get information from an API

A promise is code that must be resolved before it can be returned

async on a method allow for the fetch to be complete. 

Axios is a promise-based HTTP Client for node.js and the browser. It is isomorphic. 

.map() creates a new array from calling a function for every array element. It does not execute the function for empty elements and it does not change the original array.

Map converts an array into a new data type and returns it. 

To let the user know that an error occured, use try/catch
Example: 

async getMonsters() {
    try {
        monstersService.getMonsters()
    } catch (error) {
        Pop.error(error)
    }
}

try will attempt to run the code inside of the first codeblock
catch will alert that 

# Tuesday June 25th: Lecture Notes with Jeremy
## APIs 

mcv-auth 

### Environment Variables









