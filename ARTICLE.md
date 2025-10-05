# Simple Python Calculator

A clean command-line calculator built with Python. Performs basic arithmetic operations with error handling.

## What It Does

This calculator lets you:
- Add, subtract, multiply, and divide numbers
- Handle decimals and negative numbers
- Prevent crashes from bad input
- Run multiple calculations without restarting

## How It Works

### The Functions

Each math operation gets its own function:

```python
def add(x, y):
    return x + y

def divide(x, y):
    if y == 0:
        return "Error! Division by zero."
    return x / y
```

**Why separate functions?** Makes the code easy to test and reuse.

### The Menu Loop

The calculator runs in a loop, showing a menu each time:

```
1. Add
2. Subtract
3. Multiply
4. Divide
5. Exit
```

Users pick a number, enter two values, and get their answer. Press 5 to exit.

### Error Handling

Two types of errors are handled:
1. **Division by zero** - Returns an error message instead of crashing
2. **Invalid input** - Catches when users type letters instead of numbers

```python
try:
    num1 = float(input("Enter first number: "))
except ValueError:
    print("Invalid input! Please enter numbers only.")
```

## Key Features

✓ Simple menu interface  
✓ Works with decimals (3.14, 2.5)  
✓ Works with negatives (-5, -10)  
✓ Doesn't crash on bad input  
✓ Only 50 lines of code  

## Usage Example

```
Enter choice (1/2/3/4/5): 1
Enter first number: 10
Enter second number: 5
10.0 + 5.0 = 15.0
```

## What I Learned

Building this taught me:
- Writing clean functions
- Handling user input safely
- Using loops for repeated actions
- Managing errors without crashes

## Possible Improvements

Ideas for future versions:
- Add more operations (square root, power)
- Save calculation history
- Add a memory function
- Create a GUI version

## Running the Code

```bash
python calculator.py
```
---

**Tech**: Python 3  
**Lines of Code**: ~50  
**License**: MIT

Simple, functional, and ready to use.
