# Intro to JavaScript
01. Which keywords are used to declare a variable in JavaScript?

    > const, let, and var

02. What is the definition of a function?

    > A function is a reuseable block of code designed to perform a certain task.

03. What are the `SOLID` principles?

    > Single-responsibility, Open-closed, Liskov substitution, Interface segregation, Dependency inversion

04. Given this array: How could you remove the `pineapple`?

    ```js
    let fruit = ['apple', 'banana', 'pineapple', 'orange', 'strawberry']
    ```

    > splice(2)

05. Given these two objects: How could you add each to the others friends arrays?

    ```js
    let you = {
        name: "You",
        hair: true,
        friends: []
    }
    let them = {
        name: "Them",
        hair: false,
        friends: []
    }
    ```

    > To add to the friends in the you object, you could use you.friends.push(). You could do the same with the them object. them.friends.push().

06. Give an example of a JavaScript `Conditional`:

    > An if else statement is an example of a JavaScript conditional.

07. What is the main difference between `parameters` and `arguments`?

    > A parameter is a variable in the function definition (like a placeholder), while the argument is actual values that are passed to the function when it is called. 

08. Instead of writing everything to the console, what is a better way to debug your code?

    > You can code small and test small so you don't have to right everything in the console when using console.log(), however if you don't want to use console.log, with DevTools, you can create breakpoints. Alternatively, you could comment out the code in sections and uncover from there. 

09. What is the difference between a `primitive` value and a `reference` value?

    > Primitive values are values that are stored directly in the variable. Examples of primitives would be strings, numbers, booleans, null, and undefined. Reference values are values that are stored in memory and are accessed through a reference. Examples of references are arrays and objects.

10. Demonstrate a loop that prints the numbers between -100 and 100?

    > for (let i = -100; i <= 100; i++) {
        console.log(i);
    }
