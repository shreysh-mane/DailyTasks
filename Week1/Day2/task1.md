### Table Details

**Table Name:** Employees

**Columns:**
- **EmployeeID:** INT, Primary Key
- **FirstName:** VARCHAR(50), Not Null
- **LastName:** VARCHAR(50), Not Null
- **Email:** VARCHAR(100), Not Null
- **Salary:** INT, Not Null
- **Department:** VARCHAR(50)

### Sample Records

**Employees Table**
- EmployeeID: 1, FirstName: 'John', LastName: 'Doe', Email: 'john.doe@company.com', Salary: 60000, Department: 'Marketing'
- EmployeeID: 2, FirstName: 'Jane', LastName: 'Smith', Email: 'jane.smith@company.com', Salary: 75000, Department: 'Sales'
- EmployeeID: 3, FirstName: 'Michael', LastName: 'Johnson', Email: 'michael.johnson@company.com', Salary: 85000, Department: 'Marketing'
- EmployeeID: 4, FirstName: 'Emily', LastName: 'Williams', Email: 'emily.williams@company.com', Salary: 72000, Department: 'IT'
- EmployeeID: 5, FirstName: 'David', LastName: 'Brown', Email: 'david.brown@company.com', Salary: 65000, Department: 'Sales'
- EmployeeID: 6, FirstName: 'Sarah', LastName: 'Davis', Email: 'sarah.davis@company.com', Salary: 90000, Department: 'IT'
- EmployeeID: 7, FirstName: 'Robert', LastName: 'Miller', Email: 'robert.miller@company.com', Salary: 70000, Department: 'Finance'
- EmployeeID: 8, FirstName: 'Jessica', LastName: 'Wilson', Email: 'jessica.wilson@company.com', Salary: 65000, Department: 'Finance'
- EmployeeID: 9, FirstName: 'Daniel', LastName: 'Anderson', Email: 'daniel.anderson@company.com', Salary: 72000, Department: 'IT'
- EmployeeID: 10, FirstName: 'Ashley', LastName: 'Taylor', Email: 'ashley.taylor@company.com', Salary: 58000, Department: 'Sales'
- EmployeeID: 11, FirstName: 'William', LastName: 'Brown', Email: 'william.brown@company.com', Salary: 78000, Department: 'Marketing'
- EmployeeID: 12, FirstName: 'Sophia', LastName: 'Davis', Email: 'sophia.davis@company.com', Salary: 62000, Department: 'HR'


### Practice Questions for Constraints, Primary Key, and Foreign Key

1. **Create a constraint to ensure that the salary of an employee is greater than 0.**

2. **Create a foreign key constraint in the Employees table to reference the DepartmentID in the Departments table.**

3. **Create a unique constraint on the Email column in the Employees table.**

4. **Create a primary key constraint on the DepartmentID column in the Departments table.**

5. **Create a foreign key constraint in the Projects table to reference the DepartmentID in the Departments table.**

6. **Insert a new employee with a DepartmentID that does not exist in the Departments table and observe the foreign key constraint violation.**

7. **Attempt to insert a duplicate email address into the Employees table and observe the unique constraint violation.**

8. **Delete a department from the Departments table that is being referenced by the Employees table and observe the foreign key constraint violation.**

9. **Update the DepartmentID of an existing employee to a value that does not exist in the Departments table and observe the foreign key constraint violation.**