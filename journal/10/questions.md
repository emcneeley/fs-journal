# CSharp and SQL Fundamentals
01. What is the purpose of a `namespace`?

o provide a way to organize and group related code elements and to avoid naming conflicts
02. What is the difference between a `class` and an `interface`?

Class: A class is a blueprint or template that defines the properties (attributes) and behaviors of objects.


Interface: defines a contract or a set of rules that a class must adhere to.

03. What is the method that returns an instance of a class, yet it has no return type?

 constructor

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

 public 

06. In the Car example what is `string` an indication of?

 its declaring what "start is"
  which is the string "vrooom "
07. In the Car example what is `abstract` preventing?

  global access 

08. In a SQL table, what is the difference between information in a row and information in a column?

rows hold columns 

09. Demonstrate the necessary SQL for creating a table called `characters` with the values `name, age, description` as strings, and an `int` id.

  CREATE TABLE
   characters (
        id INT NOT NULL AUTO_INCREMENT PRIMARY KEY,
        name VARCHAR (500),
        age INT NOT NULL,
        description VARCHAR (500),
       

10. In SQL how can you query more than a single table? Provide an example.

  using a JOIN 



          SELECT 
          rec.*,
          creator.*
          FROM recipe rec
          JOIN accounts creator ON rec.creatorId = creator.id
          WHERE rec.id =LAST_INSERT_ID();";
