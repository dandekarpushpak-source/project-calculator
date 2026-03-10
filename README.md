# project-calculator
This project is a **Functional Command-Line Interface (CLI) Calculator** written in Python. It is designed to perform basic arithmetic operations while demonstrating core programming concepts like modular function design, error handling, and user input validation.

---

## ### Key Components & Features

### 1. **Modular Arithmetic Logic**

The calculator logic is separated into individual functions for each operation:

* `add(a, b)`: Returns the sum.
* `subtract(a, b)`: Returns the difference.
* `multiply(a, b)`: Returns the product.
* `divide(a, b)`: Returns the quotient, including a specific check to prevent **division by zero**.

### 2. **Robust Input Validation**

The `get_number` function acts as a gatekeeper. It uses a `while True` loop and a `try-except` block to ensure the program doesn't crash if a user accidentally types letters instead of numbers. It will continuously prompt the user until a valid `float` is provided.

### 3. **Interactive Menu Loop**

The `main()` function drives the user experience:

* **Persistent Interface:** The program runs in a loop, allowing for multiple calculations without restarting the script.
* **User Choice:** Users select operations via a simple numbered menu (1-5).
* **Clean Exit:** Option 5 breaks the loop and terminates the program gracefully.

### 4. **Error Handling**

The project handles two primary "edge cases" that often crash simpler scripts:

* **Invalid Menu Selection:** If a user enters "9" or "hello" at the menu, the program alerts them and restarts the loop.
* **Mathematical Errors:** The `divide` function raises a `ValueError` if the divisor is zero, which is then caught and printed in the main loop to prevent a system crash.

---

## ### Project Workflow

1. **Start:** The program displays the operation menu.
2. **Input:** The user selects an operation or chooses to exit.
3. **Data Entry:** If an operation is chosen, the program collects two numbers using the validation helper.
4. **Execution:** The corresponding math function is called.
5. **Output:** The result is formatted and displayed in the console.
6. **Repeat:** The loop returns to the menu until the user selects "Exit."

---

## ### Potential Enhancements

If you're looking to take this further, you might consider:

* **Advanced Math:** Adding a power function ($a^b$) or square roots.
* **Continuous Calculation:** Allowing the user to use the previous result as the first number for the next operation.
* **Logging:** Saving a history of calculations to a text file.

How would you like to evolve this code next?

* Adding scientific functions
* Creating a GUI version
* Storing calculation history
* Refactoring into a Class

What's the next goal for your script?
