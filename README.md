Calculator
==========

This is a simple calculator application built using HTML, CSS, and JavaScript. It can perform basic arithmetic operations such as addition, subtraction, multiplication, and division. It also has a number of features and edge cases that are described below.

Features
--------

*   The calculator has a display that shows the current number or the result of the calculation.
    
*   The calculator has buttons for the numbers 0-9, as well as buttons for the decimal point, addition, subtraction, multiplication, division, equal, clear, and backspace.
    
*   The calculator can handle decimal points.
    
*   The calculator can handle negative numbers.
    
*   The calculator can clear the display and reset the calculation.
    
*   The calculator can remove the last character from the display.
    
*   The calculator can perform the current operation on the first operand and the display, and update the display with the result.
    
*   The calculator can display an error message when dividing by zero.
    

Edge Cases
----------

*   The calculator does not evaluate more than a single pair of numbers at a time. For example, if you press a number button (12), followed by an operator button (+), a second number button (7), and finally a second operator button (-), the calculator will first evaluate the first pair of numbers (12 + 7), second, display the result of that calculation (19), and finally, use that result (19) as the first number in your new calculation, along with the next operator (-).
    
*   The calculator rounds answers with long decimals so that they don’t overflow the screen.
    
*   Pressing = before entering all of the numbers or an operator could cause problems!
    
*   Pressing “clear” should wipe out any existing data. Make sure the user is really starting fresh after pressing “clear”
    
*   Display a snarky error message if the user tries to divide by 0… and don’t let it crash your calculator!
    

How I Struggled and Tackled the Logic
-------------------------------------

At first, I struggled with figuring out how to handle the different arithmetic operations and how to display the result on the screen. I also had trouble with handling decimal points and negative numbers.

To tackle these issues, I broke down the problem into smaller parts and tackled each part one at a time. For example, I started by creating a simple calculator that could only add two numbers. Once I had that working, I added the ability to subtract, multiply, and divide.

To handle decimal points, I added a check to see if the current number already had a decimal point before adding another one. To handle negative numbers, I added a button for the negative sign and updated the logic to handle negative numbers.

Overall, I learned a lot about how to break down a complex problem into smaller parts and how to tackle each part one at a time. I also learned about how to handle user input and how to display the result on the screen.

Functions
---------

*   **onButtonPress(event)**: This function is called when a button is pressed. It takes an event object as an argument and extracts the ID of the button that was pressed. It then performs the appropriate action based on the button that was pressed. For example, if a number button is pressed, it appends the corresponding number to the display. If the "dot" button is pressed, it appends a decimal point to the display. If the "clear" button is pressed, it clears the display and resets the calculator. If the "backspace" button is pressed, it removes the last character from the display. If an operator button is pressed, it sets the current operator and stores the first operand. If the "equal" button is pressed, it performs the current operation on the first operand and the display, and updates the display with the result. If the "sign" button is pressed, it changes the sign of the number in the display. If an operator button is pressed, it sets the current operator and stores the first operand.
    
*   **operate(op1, operator, op2)**: This function takes an operator and two operands, and returns the result of applying the operator to the operands. For example, if **op1** is 12, **operator** is '+', and **op2** is 7, this function will return 19.
    
*   **updateDisplay()**: This function updates the display with the current number or the result of the calculation.
    
*   **add(a, b)**: This function returns the sum of **a** and **b**.
    
*   **subtract(a, b)**: This function returns the difference between **a** and **b**.
    
*   **multiply(a, b)**: This function returns the product of **a** and **b**.
    
*   **division(a, b)**: This function returns the quotient of **a** and **b**.
    

How to Use
----------

To use the calculator, simply click on the buttons to enter numbers and perform operations. The display will show the current number or the result of the calculation. To clear the display and reset the calculator, click the "clear" button. To remove the last character from the display, click the "backspace" button. To perform the current operation on the first operand and the display, and update the display with the result, click the "=" button.

Built With
----------

*   HTML
    
*   CSS
    
*   JavaScript