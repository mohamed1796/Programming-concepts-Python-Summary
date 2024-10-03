# Programming-Concepts-Python-Summary


### **Chapter 1: Introduction to Computers and Programming**

1. **Basic Definitions:**
   - **Computer**: A programmable machine that follows instructions from a program.
   - **Program**: A set of instructions for the computer to perform tasks (also known as software).
   - **Programmer**: A person who designs, writes, and tests programs.

2. **Computer System Components:**
   - **Hardware**: The physical parts of a computer (e.g., CPU, memory, storage, input/output devices).
     - **Central Processing Unit (CPU)**: The brain of the computer, responsible for executing instructions.
       - **Control Unit**: Manages and decodes instructions.
       - **Arithmetic & Logic Unit (ALU)**: Performs mathematical and logical operations.
   - **Memory**:
     - **Main Memory (RAM)**: Temporarily stores data and programs while in use; volatile.
     - **Secondary Storage**: Non-volatile storage (e.g., hard drives, USBs).
   - **Input Devices**: Allow data to enter the system (e.g., keyboard, mouse).
   - **Output Devices**: Present data from the system (e.g., monitor, printer).

3. **Software Types:**
   - **System Software**: Manages the hardware and basic functions (e.g., operating systems).
   - **Application Software**: Programs that perform specific tasks (e.g., word processing, web browsers).

4. **Programming Concepts:**
   - **Low-level Languages**: Close to machine code, harder to write (e.g., assembly language).
   - **High-level Languages**: Easier to write and understand, closer to human language (e.g., Python, C++).
   - **Compiler**: Translates high-level code into machine language.
   - **Interpreter**: Executes high-level code line by line (e.g., Python interpreter).

5. **Programming Basics:**
   - **Statements**: Instructions for actions (e.g., assignment, print).
   - **Keywords**: Reserved words in programming (e.g., `if`, `else`).
   - **Variables**: Named memory locations to store data.
   - **Operators**: Symbols for operations (e.g., +, -, =).

6. **Problem Solving and Algorithms:**
   - **Algorithm**: A step-by-step procedure to solve a problem.
   - **Control Structures**: Sequence, decision, and repetition control the flow of a program.

7. **Flowcharts and Python:**
   - **Flowcharts**: Graphical representations of algorithms.
   - **Python**: A popular high-level programming language with two execution modes:
     - **Interactive Mode**: Execute single commands.
     - **Script Mode**: Execute entire programs saved as scripts.

---


### **Chapter 2: Input, Processing, and Output**

1. **Designing a Program**:
   - Programs follow a **development cycle**:
     1. **Design** the program.
     2. **Write** the code.
     3. Correct **syntax errors**.
     4. **Test** the program.
     5. Correct **logic errors**.

2. **Basic Program Flow**:
   - **Input**: Data received by the program.
   - **Processing**: Operations performed on input data (e.g., calculations).
   - **Output**: Data displayed to the user after processing.

3. **Python Print Function**:
   - The `print()` function displays output.
   - Multiple items can be printed using a comma (`,`).
   - Control output format with arguments like `end=' '` (to change end-of-line behavior) and `sep='-'` (to change separators between items).

4. **Escape Sequences & String Concatenation**:
   - Special characters can be used in strings:
     - `\n`: New line.
     - `\t`: Horizontal tab.
   - **String concatenation**: Combining strings using the `+` operator.

5. **Formatted Output with F-strings**:
   - F-strings (formatted strings) allow embedding expressions and variables:
     - Example: `print(f'Hello {name}')`.
     - Formatting options (e.g., rounding numbers): `print(f'{num:.2f}')` for two decimal places.

6. **Identifiers and Variables**:
   - **Identifiers**: Names for variables, functions, etc. Should be meaningful and follow rules:
     - Must start with a letter or underscore.
     - Cannot use keywords.
   - **Variables**: Store data in memory; values can change during program execution.
     - Assignment format: `variable = value`.

7. **Input from Keyboard**:
   - Use `input()` function to get data from the user.
   - Converts data into strings by default. For numeric input, use type conversion functions like `int()` or `float()`.

8. **Arithmetic Operations**:
   - Basic operators: `+`, `-`, `*`, `/`, `//` (integer division), `%` (modulus), `**` (exponent).
   - Follow the **order of operations** (parentheses, exponents, multiplication/division, addition/subtraction).

9. **Named Constants**:
   - Constants are variables whose values don’t change. While Python doesn’t have built-in constants, you can indicate a constant by using all uppercase letters (e.g., `TAX_RATE = 0.075`).

10. **Comments**:
    - Comments are used to explain code and are ignored by the interpreter. Begin with `#`.
    - Good practice: Add comments at the start of a program and throughout complex sections.
   
--- 


### **Chapter 3: Decision Structures and Boolean Logic**


### **1. Relational Operators**
- **Relational operators** compare two values and return `True` or `False`.
  - Examples: `>`, `<`, `>=`, `<=`, `==`, `!=`.
  - These expressions allow you to check conditions like "is greater than" or "is equal to."

### **2. The `if` Statement**
- **`if` statement**: Controls the execution of statements based on a condition. If the condition is `True`, the statements inside the `if` block are executed.
  - Example: 
    ```python
    if score >= 60:
        print("Passed")
    ```

### **3. The `if-else` Statement**
- **`if-else` statement**: Provides two possible paths of execution. If the condition is `True`, one block is executed; if `False`, the other block is executed.
  - Example:
    ```python
    if score >= 60:
        print("Passed")
    else:
        print("Failed")
    ```

### **4. Nested `if` Statements**
- **Nested `if`**: An `if` statement inside another `if` statement. It allows for more complex decision-making by testing multiple conditions.
  - Example:
    ```python
    if account_type == 'premium':
        if balance > 1000:
            print("Eligible for loan")
    ```

### **5. The `if-elif-else` Statement**
- **`if-elif-else`**: Tests multiple conditions in sequence until one is `True`. Once a `True` condition is found, the corresponding block is executed, and the rest are skipped.
  - Example:
    ```python
    if score >= 90:
        print("Grade A")
    elif score >= 80:
        print("Grade B")
    else:
        print("Grade C")
    ```

### **6. Logical Operators**
- **Logical operators** (`and`, `or`, `not`) are used to combine relational expressions into compound Boolean expressions.
  - **`and`**: Both conditions must be `True` for the overall expression to be `True`.
  - **`or`**: At least one condition must be `True` for the overall expression to be `True`.
  - **`not`**: Reverses the Boolean value of an expression.
  - Example:
    ```python
    if age > 18 and age < 65:
        print("Eligible for work")
    ```

### **7. Checking Numeric Ranges**
- You can check if a number falls within a certain range using relational and logical operators:
  - Example:
    ```python
    if 0 <= grade <= 100:
        print("Valid grade")
    ```

### **8. Boolean Variables**
- **Boolean variables** store `True` or `False` values and are often used as flags in programs to track conditions.
  - Example:
    ```python
    flag = False
    if temperature > 30:
        flag = True
    ```

--- 

### **Chapter 4: Repetition Structures**

### 1. **Introduction to Loops**:
- Loops allow repeated execution of code without duplicating it.
- **Two main types**:
  - **Condition-controlled** (e.g., `while` loops): Runs until a condition is no longer true.
  - **Counter-controlled** (e.g., `for` loops): Runs a specific number of times.

### 2. **The `while` Loop**:
- A **pretest loop**: Checks the condition before each iteration.
- **Example**: Counting down from 5 to 0. The loop stops when the condition is no longer met.
- Infinite loops occur if there's no code to make the condition false.

### 3. **Counters**:
- A **counter** is a variable that changes (increments or decrements) during loop execution. It controls the loop.

### 4. **Augmented Assignment Operators**:
- Shorthand for incrementing, decrementing, or modifying variables (e.g., `+=`, `-=`, etc.).

### 5. **Input Validation with Loops**:
- Loops can validate user input by repeatedly asking for correct values until valid input is provided.

### 6. **Common Loop Errors**:
- Forgetting to update the loop control variable or incorrect indentation can cause infinite loops or incorrect execution.

### 7. **Running Totals and Averages**:
- Loops can be used to **accumulate totals** or calculate averages by iterating over a set of numbers.

### 8. **Sentinels**:
- A **sentinel value** marks the end of user input (e.g., `-1` could stop data entry).

### 9. **The `for` Loop**:
- A **count-controlled loop** that iterates over a sequence (e.g., a list or range).
- Useful for precise repetitions and when the number of iterations is known in advance.

### 10. **Nested Loops**:
- Loops within loops are useful for tasks like processing multi-dimensional data (e.g., calculating student test averages).

### 11. **Breaking and Continuing Loops**:
- The `break` statement exits a loop early, while `continue` skips to the next iteration without finishing the current one.

### 12. **Turtle Graphics and Loops**:
- Loops can be used to draw shapes and patterns using turtle graphics (a method of creating visuals with code).

Here are some code examples based on the topics covered in Chapter 4 of GENG 106:

### Examples

### 1. **Basic `while` Loop Example**
This loop counts down from 5 to 0:

```python
n = 5
while n > 0:
    print(n)
    n -= 1  # Decrease n by 1 each iteration
print('Blastoff!')
```

**Output:**
```
5
4
3
2
1
Blastoff!
```

### 2. **Counter-Controlled `while` Loop**
This loop counts the sum of numbers from 1 to 10:

```python
sum = 0
number = 1
while number <= 10:
    sum += number  # Add the current number to sum
    number += 1    # Increment the counter
print(f'Sum of numbers 1 to 10 is {sum}')
```

**Output:**
```
Sum of numbers 1 to 10 is 55
```

### 3. **`for` Loop Example**
This loop prints a list of friends:

```python
friends = ['Joseph', 'Glenn', 'Sally']
for friend in friends:
    print(f'Happy New Year, {friend}!')
```

**Output:**
```
Happy New Year, Joseph!
Happy New Year, Glenn!
Happy New Year, Sally!
```

### 4. **Input Validation with `while` Loop**
This example asks for a number between 1 and 100 and keeps asking until valid input is provided:

```python
number = int(input("Enter a number between 1 and 100: "))
while number < 1 or number > 100:
    number = int(input("Invalid input. Enter a number between 1 and 100: "))
print(f'You entered {number}')
```

**Sample Run:**
```
Enter a number between 1 and 100: 150
Invalid input. Enter a number between 1 and 100: -5
Invalid input. Enter a number between 1 and 100: 50
You entered 50
```

### 5. **Running Total and Average**
This example calculates the average of 5 input numbers:

```python
count = 0
total = 0
while count < 5:
    number = int(input('Enter a number: '))
    total += number
    count += 1
print(f'The average is {total / 5}')
```

**Sample Run:**
```
Enter a number: 10
Enter a number: 20
Enter a number: 30
Enter a number: 40
Enter a number: 50
The average is 30.0
```

### 6. **Sentinel Loop**
This example uses a sentinel value of `-1` to end a sequence of points scored in a game:

```python
total = 0
points = int(input("Enter points earned (or -1 to quit): "))
while points != -1:
    total += points
    points = int(input("Enter points earned (or -1 to quit): "))
print(f'The total points are {total}')
```

**Sample Run:**
```
Enter points earned (or -1 to quit): 12
Enter points earned (or -1 to quit): 22
Enter points earned (or -1 to quit): -1
The total points are 34
```

### 7. **`for` Loop with `range()`**
This example prints numbers from 1 to 5 using a `for` loop and the `range()` function:

```python
for num in range(1, 6):
    print(num)
```

**Output:**
```
1
2
3
4
5
```

### 8. **Nested Loops Example**
This example prints a pattern of stars using nested loops:

```python
for row in range(6):  # Outer loop
    for col in range(8):  # Inner loop
        print('*', end='')  # Print stars in the same line
    print()  # Move to the next line after each row
```

**Output:**
```
********
********
********
********
********
********
```

### 9. **Breaking Out of a Loop**
This example shows how to use the `break` statement to exit a loop early:

```python
while True:
    line = input('> ')
    if line == 'done':
        break
    print(line)
print('Done!')
```

**Sample Run:**
```
> hello
hello
> done
Done!
```

### 10. **Continue Statement Example**
This example uses the `continue` statement to skip lines starting with `#`:

```python
while True:
    line = input('> ')
    if line.startswith('#'):
        continue  # Skip the rest of the loop if line starts with #
    if line == 'done':
        break
    print(line)
print('Done!')
```

**Sample Run:**
```
> hello
hello
> # This is a comment
> done
Done!
```

These examples cover a variety of loop types, input validation, counters, and control structures that are critical to programming.
