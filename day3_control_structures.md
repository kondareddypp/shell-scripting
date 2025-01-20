## Day 3: Shell Scripting - Control Structures

Control structures allow you to control the flow of execution in your shell scripts. They enable you to make decisions based on conditions and repeat tasks as needed. Here's an overview of common control structures in shell scripting:

### Conditional Statements

* **if statement:** Executes a block of code only if a specified condition is true.

```bash
if [ condition ]; then
  # Commands to execute if condition is true
fi
if-else statement: Executes one block of code if the condition is true, and another block if it's false.
Bash

if [ condition ]; then
  # Commands to execute if condition is true
else
  # Commands to execute if condition is false
fi
if-elif-else statement: Handles multiple conditions sequentially, allowing you to check for different scenarios.
Bash

if [ condition1 ]; then
  # Commands to execute if condition1 is true
elif [ condition2 ]; then
  # Commands to execute if condition2 is true
else
  # Commands to execute if none of the conditions are true
fi
Looping Constructs
for loop: Repeats a block of code for a specific number of times or iterates over a set of values.
Bash

for variable in list_of_values; do
  # Commands to execute for each value in the list
done
while loop: Repeats a block of code as long as a given condition remains true.
Bash

while [ condition ]; do
  # Commands to execute as long as the condition is true
done
until loop: Repeats a block of code as long as a given condition remains false (opposite of while loop).
Bash

until [ condition ]; do
  # Commands to execute as long as the condition is false
done
Case Statement
case statement: Executes different blocks of code based on the value of a variable.
Bash

case "$variable" in
  value1)
    # Commands to execute if variable equals value1
    ;;
  value2)
    # Commands to execute if variable equals value2
    ;;
  *)
    # Commands to execute if none of the above values match (default case)
    ;;
esac
Key Considerations
Indentation: Consistent indentation is crucial for readability and maintainability of your scripts. Use proper indentation to define code blocks within control structures.
Quoting: Always quote variables within conditional expressions to prevent unexpected behavior due to special characters or spaces.
Logical Operators: Combine multiple conditions using logical operators like && (AND), || (OR), and ! (NOT) for complex decision-making in your scripts.
