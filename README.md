 BODOMAS Calculator
* Overview
This project is a web-based calculator that follows the BODMAS rule (Brackets, Orders, Division and Multiplication, Addition and Subtraction). It supports basic arithmetic operations, square roots, percentages, exponents, and even includes simple memory functions.
The calculator is built using HTML, CSS, and JavaScript, with a user-friendly interface and responsive styling for a clean desktop view.

* Features
- Basic Arithmetic: Addition +, Subtraction -, Multiplication *, Division /
- Advanced Operations:
- Exponentiation using ^ (handled as ** in JS)
- Square root using √
- Percentage using %
- Memory Functions:
- M+ adds the current result to memory
- MR recalls the stored value
- Bracket Support: Calculations inside () are processed first
- Live Expression Display: Shows the full mathematical expression before calculation
- Error Handling: Displays "Error" for invalid operations
- Delete & Clear:
- Del removes last character
- C clears the entire display

* How It Works
HTML
- Defines the layout of the calculator
- Includes a disabled input (#display) to show the expression/result
- Buttons are organized in rows and linked with onclick functions
CSS
- Provides a centered layout with a soft blue theme
- Adds shadows, rounded borders, and hover effects for interactivity
JavaScript
Handles all logic:
- appendToDisplay(value): Adds characters/operators to the input
- clearDisplay(): Resets the input
- calculate(): Transforms symbols into valid JavaScript expressions (√ → Math.sqrt, % → *0.01, ^ → **) and uses eval() to compute the result
- memoryAdd(): Evaluates and adds the result to a memory variable
- memoryRecall(): Inserts memory value into the display
- deleteEachItem(): Removes the last character from the input

* How to Run
- Save the code in a .html file (e.g., calculator.html)
- Open the file in any modern web browser
- Start entering expressions and enjoy instant calculations

