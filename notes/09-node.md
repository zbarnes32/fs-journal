# Node

## Monday's Lecture Notes with Mick

In Mick's example, Node.js is the island and Express.js is the castle on the island. The knight is the HTTP Request.

Node.js can read/run javascript without the browser.
Express.js is a JavaScript library. 

Using node template in BCW CREATE.

The BaseController creates the door
The super is the class that you extended from. 
for example: 
    export class CatsController extends BaseController {
        constructor(){
            super('endpoint')
        }
    }
    
Postman will help test POST request. **Need to download for further testing**


/: is a route parameter

# Tuesday's Lecture Notes with Mick
## Node.js & Express.js

Follow along with Mick: 
1. Already deleted unnecessary files and created cars in MongoDb.
2. Grabbed json files from BCW sandbox api and put it into the VS Code and MongoDb (insert document option and copy/paste)
3. Created CarsController, CarsService, and Car model.
4. Build the model out using data, created a Schema inside of the model. Also looked at the Figma to help creating the keys with requirements.
5. Go to DbContext to put in the schema.
6. Filed out the basic info in Service then moved to Controller
7. Created a getAllCars method in Controller and Service.
8. Clicked the run and debug ('watch') on the sidebar.
9. Go to Postman to test if the data can be retrieved. 
10. Created a searchCars method in the controller and service using request queries in the find. 
11. Inside of the service, adding results and count, with a limit and skip.
12. Created a super search method inside of the controller and service. 
13. Virtual properties: Update car model to have creatorId. Gluing the two together. { toJSON: {virtuals: true }} -see Mick's greg's list example.
14. To set up Auth0, go to env and fill out the Auth_Domain, Auth_Client_ID, and Auth_Audience. (don't forget to also update the env.js)
15. Create a createCar method inside of the controller and service.
16. Using a piece of middleware. (.use(request, response, next) => ) inside of the constructor. Line 18 on Mick's example for reference.

enum allows you to list the options for a drop-down selector. 


# Wednesday's Lecture Notes with Mick
## Data Relationship
one-to-many
many-to-many
one-to-one

Broadway Babies is a many-to-many

1. Filled out .env file
2. Created Animal.js file with a schema using the Figma as a guide.
        * optional outside of Schema, {timestamps: true, toJSON: { virtuals: true }}
3. Created an AnimalsController and AnimalsService with basic skeleton.
4. Created createAnimal method in controller and service
5. Completed multiple Post request in Postman (see MongoDb to see if it worked). 
6. Showed off Postman variables and other cool features. 
7. Created a getAnimals method in both the controller and service.
8. Went back to Postman to show testing feature.
9. Created an updateAnimal method in the controller and service.
    A. Showed off the breakpoint debugging tool on VS Code.
10. Back in the controller, update the constructor router within the controller for the PUT request. (Remember the :) 
11. Created a Show.js model with schema. 
12. Created a ShowsController and ShowsService
13. Created a getShows method in the controller and service
    A. Created virtuals for ShowSchema for animal and handler
14. Created a createShow method in the controller and service (remember to update the router.)
15. Modify createShow method to included userInfo (auth0 with bearer token, update the router). 
16. Created a getAnimalShows method in the AnimalController/ShowsService (Don't forgot to update the AnimalController router, not the ShowsController because of the endpoint).
17. Utilized the AccountController to create a getAccountShows method (updated the router).


