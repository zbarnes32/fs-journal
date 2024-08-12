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






