# Vue

# Sunday's Pre-work Notes

* Vue Basics (tutorial): https://vuejs.org/tutorial/
    + Reactivity Fundamentals: https://vuejs.org/guide/essentials/reactivity-fundamentals.html
    + Template Syntax: https://vuejs.org/guide/essentials/template-syntax.html
    + Conditional Rendering: https://vuejs.org/guide/essentials/conditional.html
    + Form Input Bindings: https://vuejs.org/guide/essentials/forms.html
    + Event Handling: https://vuejs.org/guide/essentials/event-handling.html
    + List Rendering: https://vuejs.org/guide/essentials/list.html
    + Lifecycle Diagram: https://vuejs.org/guide/essentials/lifecycle.html#lifecycle-diagram





# Monday's Lecture Notes with Jeremy
## Vue.js

The big three of JavaScript frameworks: Vue.js, React.js, and Angular.io (typescript).

React is probably the most popular, Angular is the most robust, and Vue is in a happy medium. 

VITE will replace bcw serve. 

A ref creates a watchable object around whatever value is passed to the ref function.

.value accesses the value stored within the watchable object.

There is no longer controllers, instead it is in the App.vue.

Computed allows us to bring in properties from the appstate and attach listeners to them. 

v-for essentially will complete a for loop. For an example, look at the HTML in the App.vue in Jeremy's boss_monster. 

The key in a v-for should be a unique property on whatever you are iterating over. 

Use {{}} to display javascript as text

: before an attribute binds that attribute to a javascript value. 

computed values can calculate things for us and return them, and if...

onMounted is a lifecycle hook that will execute a callback function when this component (page) is rendered to the DOM. 

* Make sure Vue - Official in installed in VS Code.
