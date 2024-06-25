# Async

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