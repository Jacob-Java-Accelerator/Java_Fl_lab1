# Java Foundation Lab 1

This repository contains two Java console applications as part of foundational Java programming labs:

- **FizzBuzzProject**: A classic FizzBuzz implementation with user input and validation.
- **MortgateApp**: A mortgage calculator that computes monthly payments based on user-provided values.

---

## Lab 1: FizzBuzzProject

### Overview

A simple console application that prompts the user for a number and prints:

- "FizzBuzz" if the number is divisible by both 3 and 5
- "Fizz" if divisible by 5
- "Buzz" if divisible by 3
- The number itself otherwise

### Features

- Input validation: Ensures the user enters a valid integer.
- Modular code: Separate methods for input handling and FizzBuzz logic.

### How to Run

1. Navigate to the `FizzBuzzProject` directory:
   ```sh
   cd FizzBuzzProject
   ```
2. Build the project with Maven:
   ```sh
   mvn clean compile
   ```
3. Run the application:
   ```sh
   mvn exec:java -Dexec.mainClass="org.jacob.Main"
   ```

### Example

```
Enter a number: 15
FizzBuzz
```

### Code Structure

- `Main.java`: Contains the main method, input validation, and FizzBuzz logic.

---

## Lab 2: MortgateApp

### Overview

A console-based mortgage calculator that prompts the user for:

- Principal amount (between 1,000 and 1,000,000)
- Annual interest rate (between 1% and 30%)
- Period in years (between 1 and 30)

It then calculates and displays the monthly mortgage payment.

### Features

- Input validation with custom prompts and range checks.
- Modular design: separates input handling and calculation logic.
- Uses Java's `NumberFormat` for currency formatting.

### How to Run

1. Navigate to the `MortgateApp` directory:
   ```sh
   cd MortgateApp
   ```
2. Build the project with Maven:
   ```sh
   mvn clean compile
   ```
3. Run the application:
   ```sh
   mvn exec:java -Dexec.mainClass="org.jacob.Main"
   ```

### Example

```
Principal: 200000
Annual Interest Rate: 5
Period (Years): 30
Mortgage: $1,073.64
```

### Code Structure

- `Main.java`: Handles user interaction and output.
- `InputHandler.java`: Validates and retrieves user input.
- `MortgageCalculator.java`: Performs the mortgage calculation.

---

## Requirements

- Java 17 or higher
- Maven

## How to Build All Labs

You can build each project separately by navigating into its directory and running Maven commands as shown above.

---

## Author

- Jacob Sabbath Adiaba

---

## License

This project is for educational purposes.
