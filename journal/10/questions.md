# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

  > Namespaces are used both as an “internal” organization system for a program, and as an “external” organization system—a way of presenting program elements that are exposed to other programs.

02. What is the difference between a `class` and an `interface`?

  > A class contains attributes, methods and events as its components. Interfaces contain only method prototypes, they don't provide an implementation of their methods, we can provide an implementation of its methods in our class, and for that, we can implement the interface.

03. What is the method that returns an instance of a class, yet it has no return type?

  > Any method declared void doesn't return a value. The Delete method does no have a return type.

05. In the Car example what is the access modifier of the `Start()` method?

  ```c#
  abstract class Car
  {
    public string Start()
    {

      return "Vroooom";

    }
  }
  ```

  > The public access modifier.

06. In the Car example what is `string` an indication of?

  > The type.

07. In the Car example what is `abstract` preventing?

  > It is hiding certain details about the Car class.

08. In a SQL table, what is the difference between information in a row and information in a column?

  > The column is the properties of the table and the row is the data in the tables.

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  > CREATE TABLE 
  characters(
  id INT NOT NULL PRIMARY KEY AUTO_INCREMENT,
  name VARCHAR(255) NOT NULL,
  age VARCHAR(255) NOT NULL,
  description VARCHAR(1000) NOT NULL
);

10. In SQL how can you query more than a single table? Provide an example.

  > Using the Join allows you to query two tables. An example of this is when we JOIN recipes and accounts in the All Spice checkpoint.
  
SELECT 
  recipes.*,
  accounts.*
FROM
  recipes
  JOIN accounts ON accounts.id = recipes.creatorId
  WHERE
    recipes.id = 1