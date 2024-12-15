# Employee Management System in Python (Tkinter Frontend & MySQL Backend)

**Frontend**: Tkinter-based frontend.

**MySQL Integration**: Integrated MySQL as the database backend.

## Features

- **Add an Employee:** Easily add new employees to your database with this function. Input their details, and the system will store them in the database.

- **Delete an Employee:** Select the employee to delete, and with a click of a button, it will remove the employee details from the database.

- **Update an Employee:** Make changes to their information/details and save the updated data.

- **View All Employees:** Fetch all employees from the database in a single click.

## Screenshots

![Home Screen](/screenshots/home_screeen.png)
![Add an Employee](/screenshots/add_an_employee.jpg)
![Delete an Employee](/screenshots/delete_an_employee.png)
![Delete an Employee Confirmation](/screenshots/delete_an_employee.jpg)
![Update an Employee](/screenshots/update_an_employee.png)
![Update an Employee Confirmation](/screenshots/update_an_employee_2.jpg)
![View All Employees](/screenshots/view_all_employee.jpg)

## Setup

### 1. Start MySQL Server
Run the following command to start the MySQL server:
```sh
mysql -u root -p
```

### 2. Create the Database
Run the following SQL command to create the database:
```sql
CREATE DATABASE employees;
```

### 3. Switch to the Database
Use the following command to change to the created database:
```sql
USE employees;
```

### 4. Create the Table
Create the `employeeDetails` table with the following structure:
```sql
CREATE TABLE employeeDetails (
    id INT AUTO_INCREMENT PRIMARY KEY,
    name VARCHAR(255) NOT NULL,
    dateOfBirth DATE,
    joiningDate DATE,
    salary DECIMAL(10, 2),
    department VARCHAR(255)
);
```

### 5. Describe the Table
To verify the table structure, run:
```sql
DESCRIBE employeeDetails;
```

### 6. Insert Sample Data
Insert a sample record into the table:
```sql
INSERT INTO employeeDetails (name, dateOfBirth, joiningDate, salary) 
VALUES ("Example Name", "2004-02-27", "2023-11-01", 5000.00);
```

### 7. Clone the Repository
Fork and clone this repository:
```sh
git clone <repository-url>
```

### 8. Configure Database Settings
Update the `config.json` file with your MySQL credentials:
```json
{
    "pass": "db password",
    "user": "root",
    "host": "localhost",
    "database": "employees"
}
```

### 9. Install Dependencies
Install the required Python packages:
```sh
pip install -r requirements.txt
```

### 10. Run the Application
Execute the `main.py` script:
```sh
python main.py
