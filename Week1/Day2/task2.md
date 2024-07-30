### Table Definitions

**Employees Table**
- **EmployeeID**: INT, Primary Key
- **FirstName**: VARCHAR(50), Not Null
- **LastName**: VARCHAR(50), Not Null
- **Email**: VARCHAR(100), Not Null, Unique
- **Salary**: INT, Not Null
- **DepartmentID**: INT

**Departments Table**
- **DepartmentID**: INT, Primary Key
- **DepartmentName**: VARCHAR(50), Not Null

**Projects Table**
- **ProjectID**: INT, Primary Key
- **ProjectName**: VARCHAR(100), Not Null
- **DepartmentID**: INT, Foreign Key referencing Departments(DepartmentID)

### Sample Data

**Departments Table**
- DepartmentID: 1, DepartmentName: 'Marketing'
- DepartmentID: 2, DepartmentName: 'Sales'
- DepartmentID: 3, DepartmentName: 'IT'
- DepartmentID: 4, DepartmentName: 'Finance'
- DepartmentID: 5, DepartmentName: 'HR'

**Employees Table**
- EmployeeID: 1, FirstName: 'John', LastName: 'Doe', Email: 'john.doe@company.com', Salary: 60000, DepartmentID: 1
- EmployeeID: 2, FirstName: 'Jane', LastName: 'Smith', Email: 'jane.smith@company.com', Salary: 75000, DepartmentID: 2
- EmployeeID: 3, FirstName: 'Michael', LastName: 'Johnson', Email: 'michael.johnson@company.com', Salary: 85000, DepartmentID: 1
- EmployeeID: 4, FirstName: 'Emily', LastName: 'Williams', Email: 'emily.williams@company.com', Salary: 72000, DepartmentID: 3
- EmployeeID: 5, FirstName: 'David', LastName: 'Brown', Email: 'david.brown@company.com', Salary: 65000, DepartmentID: 2
- EmployeeID: 6, FirstName: 'Sarah', LastName: 'Davis', Email: 'sarah.davis@company.com', Salary: 90000, DepartmentID: 3

**Projects Table**
- ProjectID: 1, ProjectName: 'Project A', DepartmentID: 1
- ProjectID: 2, ProjectName: 'Project B', DepartmentID: 2
- ProjectID: 3, ProjectName: 'Project C', DepartmentID: 3
- ProjectID: 4, ProjectName: 'Project D', DepartmentID: 4
- ProjectID: 5, ProjectName: 'Project E', DepartmentID: 5

### Practice Questions

1. **Create a constraint to ensure that the salary of an employee is greater than 0.**

2. **Create a foreign key constraint in the Employees table to reference the DepartmentID in the Departments table.**

3. **Create a unique constraint on the Email column in the Employees table.**

4. **Create a primary key constraint on the DepartmentID column in the Departments table.**

5. **Create a foreign key constraint in the Projects table to reference the DepartmentID in the Departments table.**

6. **Insert a new employee with a DepartmentID that does not exist in the Departments table and observe the foreign key constraint violation.**

7. **Attempt to insert a duplicate email address into the Employees table and observe the unique constraint violation.**

8. **Delete a department from the Departments table that is being referenced by the Employees table and observe the foreign key constraint violation.**

9. **Update the DepartmentID of an existing employee to a value that does not exist in the Departments table and observe the foreign key constraint violation.**