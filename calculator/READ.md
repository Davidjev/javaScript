# Calculator App

This is a simple calculator app that allows users to perform basic arithmetic operations such as addition, subtraction, multiplication, and division. The app takes user input from an input field and outputs the result and calculation history on the page.  

### How to Use

Enter a number in the input field  
Click on one of the operator buttons (+, -, *, /)  
The result of the calculation will be displayed in the "Current Result" section, along with the calculation history in the "Current Calculation" section.  

### Code Explanation

The app consists of a few global variables and several functions:  

#### Variables
- defaultResult - the default result value, which is set to 0.  
- currentResult - the current result value, which is initially set to defaultResult.  
- logEntries - an array that stores the calculation history as objects.  

#### Functions

- getUserNumberInput() - a function that retrieves the user input value from the input field and returns it as a parsed integer.  
- createAndWriteOutput() - a function that generates a calculation log and writes it to the page using the outputResult() function. It takes three arguments: the operator symbol, the result before the calculation, and the entered number.  
- writeToLog() - a function that creates a log entry object and pushes it to the logEntries array. It takes four arguments: the operation identifier (ADD, SUBTRACT, MULTIPLY, DIVIDE), the previous result, the entered number, and the new result.  
- calculateResult() - the main function that performs the calculation. It takes one argument: the calculation type (ADD, SUBTRACT, MULTIPLY, DIVIDE). It first checks whether the calculation type is valid and whether the user has entered a number. If not, it returns. Otherwise, it performs the calculation based on the calculation type and updates the currentResult value. It then calls the createAndWriteOutput() and writeToLog() functions to generate the calculation log and update the logEntries array.  
- add(), subtract(), multiply(), divide() - functions that call the calculateResult() function with the corresponding calculation type (ADD, SUBTRACT, MULTIPLY, DIVIDE) when the corresponding operator button is clicked.  

The app also has several event listeners that listen for clicks on the operator buttons and call the corresponding functions. It also retrieves and initializes various elements on the page, such as the input field, operator buttons, and result/output sections.
