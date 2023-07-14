# A bit more CSharp and SQL
1. What does ***inheritance*** accomplish for us in C#?

  > | it allows classes to inherit properties and behavios from other classes|

2. How does ***member inheritance*** work in C#? Does a `Class` inherit all members of the base `Class`?

  > | Class memebers are usually private but memeber inheritance allows a class to be extended like 'account' can extend a profile class  |

3. How does ***accessibility*** affect inheritance?

  > |determines which members of a base class can be inherited and accessed by derived classes. |

4. What is the difference between a `PRIMARY KEY` and a `FOREIGN KEY`

  > | foregin key references another table and promary key is in reference to that id on the current table  |

5. What is an ***alias***?

  > | where you alias out a variable value? |

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

  > | SELECT p.*
FROM patients p
JOIN patient_doctors pd ON p.id = pd.patientId
JOIN doctors d ON d.id = pd.doctorId
WHERE d.id = doctorId;
