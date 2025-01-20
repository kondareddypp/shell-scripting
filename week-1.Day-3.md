Day 3: Shell Scripting - Control Structures
Conditional Statements

  - if: Executes a block of code only if a specified condition is true.
    
    if [ condition ]; then
        # Commands to execute if condition is true
    fi

  - if-else: Executes one block of code if the condition is true, and another block if it's false.
    
    if [ condition ]; then
        # Commands to execute if condition is true
    else
        # Commands to execute if condition is false
    fi

  - if-elif-else: Handles multiple conditions sequentially.
    
    if [ condition1 ]; then
        # Commands to execute if condition1 is true
    elif [ condition2 ]; then
        # Commands to execute if condition2 is true
    else
        # Commands to execute if none of the conditions are true
    fi

Looping Constructs

  - for: Repeats a block of code for a specific number of times or over a set of values.
    
    for variable in list_of_values; do
        # Commands to execute for each value in the list
    done

  - while: Repeats a block of code as long as a given condition remains true.
    
    while [ condition ]; do
        # Commands to execute as long as the condition is true
    done

  - until: Repeats a block of code as long as a given condition remains false.
    
    until [ condition ]; do
        # Commands to execute as long as the condition is false
    done

Case Statement

  - case: Executes different blocks of code based on the value of a variable.
    case "$variable" in
        value1)
            # Commands to execute if variable equals value1
            ;;
        value2)
            # Commands to execute if variable equals value2
            ;;
        *)
            # Commands to execute if none of the above values match
            ;;
    esac

Key Considerations

  - Indentation: Use consistent indentation to improve readability and maintainability.
  - Quoting: Always quote variables within conditional expressions to prevent unexpected behavior.
  - Logical Operators: Combine multiple conditions using logical operators (&& for AND, || for OR, ! for NOT).
