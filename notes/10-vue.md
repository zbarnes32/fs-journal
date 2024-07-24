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

Single-File Component (SFC) - A reuseable self-contained block of code that encapsulates HTML, CSS, and JavaScript that belong together, written inside a .vue file.

Declarative Rendering - Using a template syntax that extends HTML, we can describe how the HTML should look based on JavaScript state. What the state changes, the HTML updates automatically.

Objects created from reactive() are JavaScript Proxies that work just like normal objects

ref() can take any value types and create an object that exposes the inner value under a .value property. 

In vue, mustaches are only used for text interpolation. To bind an attribute to a dynamic value, we can use the v-bind directive.

A directive is a special attribute that starts with the v- prefix (shorthand is :).

We can listen to DOM events using the v-on directive (shorthand is @).

Using v-bind and v-on together, we can create two-way bindings on form input elements. To simplify two-way bindings, Vue provides a directive, v-model.

We can use the v-if directive to conditionally render an element (truthy / falsy).

We can use v-for directive to render a list of elements based on a source array.

You can add toggle functionality to each todo by adding a "done" property to each todo object, and using v-model to bind it to a checkbox. 



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

# Thursday's Lecture Notes with Jeremy
* Look at Jeremy commit history for direction

Prop allows you to send data to a child from a project



# Full Stack Week

# Monday's Lecture Notes with Mick
## Postit

1. Create an application with two templates (client / server)
2. Update both the env.js and .env files
    A. This is why we use baseUrl as localhost:3000
    B. You can test if the client and server is linked together by logging in on the client side and look at the network tab. 
3. TIP: Go back and forth between front-end and back-end, with a focus on back-end first. For example, if you are working on bringing photos to the page, first work on the back-end before working on the front-end. Although you COULD complete the full back-end first, it is more efficient to work on one section at a time. 
4. Delete unnecessary files
(Follow along with Postman tests)
5. Create a new Schema in Album.js file within the server folder. 
6. Update DbContext.js to have the new Album schema
7. Create a AlbumsService.js file
8. Create a AlbumsController.js
9. Create the createAlbum method in the service and controller. 
10. Create the getAllAlbums in the Controller/Service
11. Create the getAlbumById in the Controller/Service
12. Create the achievedAlbumById in the Controller/Service
13. Jump to the front end and create Album.js model and AlbumsService.js
14. Stubbed out a HomePage.vue
15. Created the AlbumArticle.vue component
16. Created AlbumDetailsPage.vue page
..... (Trying to fix checkpoint issues while Mick was styling the site)

# Tuesday's Lecture Notes with Mick
## Continuation of Postit

NOTE: useRoute() is where you are located in the app (think url)
        useRouter() is the vehicle that moves you from place to place.

17. After styling, jumped back to the server and created a Schema for the picture in Picture.js
18. Created Picture Controller and Service files. 
NOTE: Remember to use Postman for suggested order and testing
19. Created CreatePictureForm.vue and built the form inside the template tags

NOTE: fab stands for floating action button
NOTE: The masonry class is what Mick used to make the layout of the pictures in the album. 

20. Created PicturesService.js file
21. Created Picture model in the Picture.js
22. Created getAlbumPictures() function inside the AlbumDetailsPage.vue

Many-to-Many

23. created AlbumMember.js with a AlbumMemberSchema
24. Update dbContext file
25. created createAlbumMember() in controller and service
26. created get AlbumMembersByAlbumId() function in AlbumController.js and AlbumMembersService.js
...
27. Jump to the client side
28. create getAlbumMembersForAlbum() in the AlbumDetailsPage.vue and AlbumMemberService. 
29. Updated the AppState
30. Created a getAccountAlbumMemberAlbums function in the AccountPage.vue and AlbumMembersService.js
31. Update the AppState for accountAlbums
REVIEW: Confused when Mick explained the  AlbumMemberAlbum and AlbumMemberProfile

# Wednesday's Lecture Notes with Mick
## Stetch Goals for Postit

32. memberCount (in albumSchema virtual) - instead of a JustOne, use "count" to just count
33. You can nest .populate() Example in AlbumMembersService.js line 19
34. ...