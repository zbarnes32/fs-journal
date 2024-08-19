# CSharp

# Monday Lecture Notes with Jeremy

dotnet new console (inside the terminal to create the file)

Program.cs

Cs version of console.log() is Console.WriteLine()
dotnet run in the terminal will run the terminal

Any class and method is Pascal-Cased

When declaring a variable, you need to say the type. 

## Strings
For example, a variable with a string as the value would look like:
string firstName = "Zach";
(Remember that statements have to end with a ; (semi-colon))

NOTE: When declaring a string, it has to be in double-quotes(" ")

If you are declaring a string with a single character ('x'), is a char instead of a string. 

String interpolate example in cs: Console.WriteLine($"My name is {firstName}.")

## Booleans

To assign booleans, use bool.

Example: 
bool likesCats = true;

NOTE: Truthy/Falsy does not exist in c sharp.

## Numbers

To assign numbers, use int.

Example: 
int numberOfShoes = 5;
numberOfShoes++

The max a int can be is 2,147,483,647
If wanting a larger number, use long

If you want to use a decimal, use double.

## Weird Stuff

c sharp can not have undefined.

A string can technically be null.

## Arrays

NOTE: Arrays are terrible in C#

string[] names = ["Zach", "Joe", "Thomas", "Porter", "Aziz", "Seth", "Evan"]

Instead you can use List
Example: List<string> dogNames = ["Dipper", "Pluto"];

## Objects

class Cat 
{
    Cat(string name)
    {
        this.Name = name;
    }

    public string Name { get; set; }
}

NOTE: public allows for full access while private doesn't



## Following Along sandwich_api 

In dbSetup.sql, you can create a table with CREATE TABLE following the name of the table.

To create a row (data), type INSERT INTO, followed by the table name. 
To remove a row from the table, type DELETE FROM, followed by the table name, plus details from the row you want to delete. 
To pull a row, type SELECT, FROM WHERE
To update a row, type UPDATE following the table name, with SET column





# Tuesday Lecture Notes with Jeremy
## Gregslist_dotnet
** NOTE: Although this is a full stack application, we are focusing on the back end. 

1. Go to appsettings.Development.json to fill out information.
2. Fill out env.js file
3. Run and Debug
4. Make sure to change the baseURL in the env.js file (make sure to check the network tab on the browser to see if it is working).
5. Create a table in the dbSetup.sql file
6. Create a model file
    ** NOTE: this is similar to setting up a schema. 
7. Create a controller file
    ** NOTE: Remember to add a namespace at the top
8. Create a service file
9. Create a repository file
10. Update the Startup.cs file with services.AddScoped<CarsService>(); and services.AddScoped<CarsRepository>();
11.  Create a profile model

NOTE: Ended up watching the rest of the lecture instead of taking notes. Make sure to follow Jeremy's commit history for more information.




# Wednesday's Lecture Notes with Jeremy
## Follow Along with PostIt

1. Fill out appsettings.Development.json & env.js (If you can log in, it's working)
2. Look at Postman test to see where we should start (Album).
3. Create an album table in dbSetup.sql
    ** NOTE: Remember to put the id as the first column.
4. Create the model.cs for albums
    ** NOTE: typing prop and then hitting enter will a line for the property type.
    ** NOTE: Make sure to add the data validation
5. Create a repository, service, and controller. 
    ** NOTE: Keeping it in that order will help with with error handling that would happen with creating it as controller, service, repository since the controller talks to the service, and the service talks to the repository. 
6. Update the Startup.cs file. 
7. Start filling out the controller, service, and repository for createAlbum.
8. Add a Profile class in Account.cs and add a Creator in the album model.
9. Create function GetAllAlbums()
    - Create in controller
    - Create in service
    - Create in repository
10. Refactored by created JoinCreator()
11. Create function GetAlbumById()
    - Create in controller
    - Create in service
    - Create in repository
12. Create function achieveAlbum()
    - Create in controller
    - Create in service 
    - Create in repository
13. Create a picture table in dbSetup.sql
14. Create a repository, service, and controller for the pictures.
15. Create function CreatePicture()
    - Create in controller
    - Create in service
    - Create in repository
16. Update the startup.cs
17. Create function GetPicturesInAlbum
    - Create in AlbumsController
    - Create in PicturesService
    - Create in PicturesRepository
18. Create function destroyPicture
    - Create in PicturesController
    - Create in PicturesService
    - Create in PicturesRepository

# Thursday's Lecture Notes with Jeremy
## Picking up where we left off on PostIt

19. Create albumMembers table in dbSetup.sql
    ** NOTE: Jeremy showed off the Unique constrant that limits the collaboration. 
20. Create an AlbumMember model, repository, service, and controller.
21. Create function CreateAlbumMember
    - Create in AlbumMembersController
    - Create in AlbumMembersService
    - Create in AlbumMembersRepository
    - Update the startup.cs
22. Create function GetAlbumMembersProfilesByAlbumId
    - Create in AlbumsController
    - Create in AlbumMembersService
    - 
23. Create the AlbumMemberProfile class in the AlbumMember model

    ```cs
    
    ```
    ** REVIEW: Look at Jeremy's commit with the 🧠🧂 message for great example of many-to-many. 

24. Create function GetAlbumMembersAlbumsByAccountId
    - Create in AccountController
    - Create in AlbumMembersService
    - Create in AlbumMembersRepository
25. Create function ...
    - Update the AlbumMember model
    - 

** REVIEW: Look at Jeremy's commits for great examples for the many-to-many examples.

** NOTE: Cloudflare is a great spot to buy a domain. 

26. Create function DestroyAlbumMember
    - Create in AlbumMemberController
    - Create in AlbumMemberService
    - Create in AlbumMemberRepository





# Monday's Lecture Notes with Jeremy
## Follow Along with insta_cult


1. Set up env files (Make sure you can log in on localhost:8080)
2. Create table Cults in dbSetup.sql
3. Create a Cult model (Cult.cs)
4. Scaffold out Repository, Service, and Controller for cults.
    **NOTE: You can fill out on the Accounts Repository, Service, and Controller and move them to their own files for a faster process.
5. Create function CreateCult
6. Joining the Accounts table to the Cults table
    **NOTE: Make sure to update for a Profile and Leader
7. Create function GetAllCults
    **NOTE: Creating JoinLeader will make things faster later on. 
8. Create function GetCultById

Moving to the client side

9. Update the HomePage
10. Create a CultsPages.vue (Use a router link around the button on the home page)
11. Create function getAllCults (Fill out page and service)
12. Create a model for cults
13. Update AppState to have cults as an empty array
14. Finish the function in the service. 
15. Create a cult card component
16. Style up the cult card
17. Create a modal component for creating a cult (Make sure to link the modal correctly).
18. 

