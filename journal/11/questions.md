# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > Inheritance allows us to define a new class based on an existing class.

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > C# only supports single inheritance meaning that can only inherit the direct parent. However, since it is transitive, the direct child can inherit from grandparents, as long as it was inherited by the parent. For example, type C can't inherit from type A directly, however, if type B inherited from type A, then type C has access to properties from type A. Static constructors, Instance construtors, and Finalizers are not able to be inherited.

3. How does ***accessibility*** affect inheritance?

  > Accessibility determines whether the class's members are visible or not. 

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > A primary key is an unique identifier for each record of a table. The foreign key helps establish a relationship between tables by referencing the primary key of another table.

5. What is an ***alias***?

  > 

6. Demonstrate how you would query a join statement that would get all of a doctors patients from the following collections:

  ```SQL
  CREATE TABLE doctors (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patients (
    id INT NOT NULL AUTO_INCREMENT,
    -- CODE OMITTED
    PRIMARY KEY (id)
  )

  CREATE TABLE patient_doctors (
    id INT NOT NULL AUTO_INCREMENT,
    doctorId INT NOT NULL,
    patientId INT NOT NULL,

    FOREIGN KEY (doctorId)
      REFERENCES doctors(id),
    FOREIGN KEY (patientId)
      REFERENCES patients(id),
  )

  ```

  > | ANSWER HERE |
