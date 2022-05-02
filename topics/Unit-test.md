# Unit Tests

**Very informative article** 

https://freecontent.manning.com/making-better-unit-tests-part-1-the-aaa-pattern/

**Video**

https://youtu.be/vZm0lHciFsQ

**Code**

https://github.com/nicklasdean/spring-jdbc

Note: **You should use test-data and not fetch data from the repository**

## Exercise-set #1

**Exercise 1**

Implement a method with the following functionality: 

- If the method receives: 
  - 5-12 return "morning"
  - 12-16 return "afternoon"
  - 16-22 return "evening"
  - 22-5 return "night"
- Identify equivalence partitions
- Unit-test the code



**Exercise 2**

Implement a method with the following functionality:

- A valid department number has:
  - 2 or 3 digits
  - Is divisible by 10 (meaning that 21 is not valid where 20 is valid)

- Unit-test the code



**Exercise 3 - employees and departments** 

Implement a method with the following functionality:

- An employee can never receive a higher commission than their base salary
- The method receives an employee object and returns true if the salary is valid
- The method returns false if the salary is not valid
- Unit-test the code



**(Advanced) Exercise 4 - employees and departments**

- Implement the following functionality:
  - Given an Employee object, return true if the Employee has a salary above the average of all employees
- Unit-test the code



## Exercise-set #2

##### **(Improvement) Exercise 4.2 - employees and departments**

- Implement the following functionality:
  - Given an Employee object, return true if the Employee has a salary above the average of all employees
- Unit-test the code
  - Write a mock/test repository that implements the CRUD interface
  - Use the aforementioned mock/test repository to unit-test

##### Exercise 1

- Implement the following functionality:
  - Write a service method that finds and returns the highest department number 
- Unit-test the code
  - Use a mock/test repository to unit-test

**Exercise 2**

- Implement the following functionality: 
  - Write a service method that returns department with the most employees
- Unit-test the code
  - Use a mock/test repository to unit-test

**(Advanced) Exercise 3**

- Implement the following functionality: 
  - Write a service method that calculates and returns the Department name with the highest average salary
