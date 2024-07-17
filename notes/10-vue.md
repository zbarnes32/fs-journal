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


# Tuesday's Lecture Notes with Mick
## Using the TMDB API to create a movie review webpage (vueflix)

1. Delete unnecessary items in the HomePage.vue
2. Created a MoviesService.js file
    A. Created a discoverMovies() method. (making a get request)
    B. Imported axios
    C. used axios.create to use the TMDB api
3. In the HomePage.vue file to create an onMounted inside of the script tag.
    A. Created the discoverMovies() method using a try/catch.
    NOTE: onMounted in the HomePage.vue file allows to load on page load
4. In the axios.create, update the api key
5. Created a Movie.js model and used the object from TMDB to create the model.
    A. Remember to use the VueDevTools
6. Use the computed vue keyword to get the AppState data. 
    A. Test to see if you get the data on the page
7. Inside of the template section, start stubbing out the HTML
    A. Use {{}}, to get the data as string.
    NOTE: {{}} is used inside of the tags whereas :bind (used in an attribute).
8. Moving the card template into its own component file
    A. defineProps({key : value})
9. Create the DiscoverButtons component
    A. Added functionality to previous/next
10. Create the SearchMovieBar component
    NOTE: v-model is a 2-Way data bind
    NOTE: when working with vue's methods, they wrap the value in large reactive objects. These values need to be accessed here in the script if you want their value. 
REVIEW: Went in depth on the SearchMovieBar and the previous/next buttons
11. Created a MovieDetailsPage.vue page
12. Updated the router.js
    NOTE: RouterLink is a built in function that... (:to={name: 'name of route'})


Note: pages are responsible for "getting" the data they want to display

# Wednesday Lecture Notes with Jeremy
## Gregslist Vue with Auth

Look at Jeremy commit history for order of operation

v-model allows two-way data binding
