# Employee Salary Calculator

This is a simple Java console application designed to manage employee salary data. It calculates the employee's net salary after tax deductions and applies a percentage-based increase to their gross salary.

## Project Structure

The project is divided into two primary files:

* **`Program.java`**: The main entry point of the application. It handles user inputs for the employee's details (name, gross salary, and tax), prompts for a salary increase percentage, and prints the formatted data to the console.
* **`Employee.java`**: An entity class representing the employee. It encapsulates the data fields (`name`, `salary`, `tax`) and the business logic to calculate the net salary and apply a raise.

## Features and Logic

The application performs two main calculations:

1. **Net Salary**: Calculated by subtracting the tax from the gross salary.
   
   $$
   Net Salary = salary - tax
   $$

2. **Salary Increase**: The percentage increase is applied *only* to the gross salary, not the net salary.

   <div align="center">
      New Salary = salary + (salary * percentage / 100)
   </div>
   
## How to Run

1. Ensure you have Java installed on your machine.

2. Open your terminal or command prompt and navigate to the project's root directory.

3. Compile the Java files (assuming they are structured inside `application` and `entities` folders):

   ```bash
   javac application/Program.java entities/Employee.java
   ```

4. Run the compiled application:

   ```bash
   java application.Program
   ```

5. Follow the on-screen prompts to enter the employee's data. 

   **Note:** The program enforces the US locale, so ensure you use a dot (`.`) for decimal values (e.g., `1500.50` instead of `1500,50`).
