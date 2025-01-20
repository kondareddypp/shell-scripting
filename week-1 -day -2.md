bash
name="John Doe"
age=25

````

**Accessing Variables**

* Use the variable name directly, preceded by a dollar sign ($).

**Input and Output**

* **Reading user input:** Use the `read` command to read values from the user.
* **Displaying output:** Use the `echo` command to display text on the screen.

**Examples:**

```bash
echo "Enter your name:"
read user_name
echo "Hello, $user_name!"

````

**Exercises:**

1.  Create a script that prompts the user for their name and age, then displays a personalized greeting.
2.  Write a script that calculates the sum of two numbers entered by the user.

**Additional Resources:**

  * Shell Scripting Variables](https://www.tutorialspoint.com/unix/unix\_shell\_variables.htm)
  * [Input and Output in Shell Scripting](https://www.google.com/url?sa=E&source=gmail&q=https://www.tutorialspoint.com/unix/unix_shell_input_output.htm)
    """))

<!-- end list -->

````
Whoops, it looks like I messed up the formatting. Here's the corrected note:

**Day 2: Shell Scripting - Variables and Input/Output**

**Variables**

* **Definition:** Used to store values for later use within the script.
* **Types:**
    * User-defined variables: Created by the user.
    * Environment variables: Set by the system or other programs.
    * Special variables: Have predefined meanings (e.g., $0, $1, $#).
* **Syntax:** `variable_name=value`

**Examples:**

```bash
name="John Doe"
age=30
````

**Accessing Variables**

To use a variable, simply refer to its name preceded by a dollar sign ($).

```bash
echo "My name is $name and I am $age years old."
```

**Input/Output**

  * **Reading Input:** Use the `read` command to read user input from the terminal.

<!-- end list -->

```bash
echo "Enter your name: "
read user_name

echo "Hello, $user_name!"
```

  * **Displaying Output:** Use the `echo` command to display text on the terminal.

<!-- end list -->

```bash
echo "This is a message from my script."
```

**Exercises:**

1.  Create a script that asks for your name and age, then displays a personalized greeting.
2.  Write a script that calculates the sum of two numbers entered by the user.

**Additional Resources:**

  * [Variables in Shell Scripting [invalid URL removed]
  * Input/Output in Shell Scripting [invalid URL removed]
