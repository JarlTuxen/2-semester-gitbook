# Backend design

**Boilerplate:**

https://github.com/nicklasdean/spring-jdbc

**Data:**

https://nicklasdean.gitbook.io/2-semester/databaseemployees-departments

## **Learning objectives**

- **Retrieving data with the JDBC API designed as a Singleton with Prepared Statements**

  - https://refactoring.guru/design-patterns/singleton
  - https://www.tutorialspoint.com/javaexamples/jdbc_prepared_statement.htm

  

- **Storing DB username & passwords safely**

  - https://mkyong.com/java/java-properties-file-examples/
  - https://www.jetbrains.com/help/objc/add-environment-variables-and-program-arguments.html




- **Building repositories as CRUD interfaces**



## Exercises in class

**Styling is not prioritized here. The main concern is viewing the data in an HTML file**

### 1. View all employees

The customer  want a feature, such that they can see all employees in a table, the same way that they can currently view all departments

### Technical Requirements

A new controller & GetMapping

A new model for modelling Employee data

A new view for displaying all employees

A new repository for querying the employee database



### 2. View single employee

The users want a feature, such that they can see a single employee by their employeenumber.

### Technical Requirements

A new controller & GetMapping with request parameter:

https://www.baeldung.com/spring-request-param

A new view for displaying a single employee

A new repository method for querying a single employee by their parameter



### 3. Create new employe

The users want a feature, such that they can fill a form with employee data and create a new employee in the database.

### Technical Requirements

A new controller & PostMapping

A new view with an input form, such that users can post new data & send to database

A new repository method for querying an insert statement with data from POST form



### (Advanced) 4. View all employees by department name

Hint: Join



## Advanced: Building a Pokedex

The data can be found here https://github.com/nicklasdean/dat20c-temp/blob/master/assets/pokedex.sql
and in resources in the Fronter plan as pokemon-insert-data.sql. Download it and open it in MySQL Workbench.

##### Reflect before engineering:

###### 1. What are the contents of the data-set?

###### 2. What are the semantics (meaning) of the data-set?

###### 3. How can we build a model (java class) that represents each entity? 

##### Exercises:

- Create a new database schema for the data
- Create a table for the data
- Insert the data
- Build the following views that displays:
  - How many pokemon exists pr. primary type? (15 rows - first is Water 28)
  - What are the average defence for all pokemon? (68)
  - What are the average hp for (primary) grass types? (65)
  - How many fire pokemon has higher hp than the average pokemon? (7 pokemon - subquery avg 64.2119)
  - What primary type are the fastest? (fastest pokemon Electric 140, fastest type Electric 98,89)

**Query as much as possible in SQL as this is more efficiant**
