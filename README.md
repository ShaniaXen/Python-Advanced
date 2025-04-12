
What Are Functions?
In Python, functions are blocks of reusable code used to perform a specific task. They come in two broad types:

Predefined (Built-in) Functions
e.g., len(), print(), sum(), etc.

User-defined Functions
Created by the user using the def keyword.

We can classify functions further as:

✅ Functions with parameters (accept inputs)

✅ Functions without parameters

✅ Functions with return value

✅ Functions without return 

🎯 Types of Arguments in Python Functions
When dealing with functions, arguments are categorized in two layers:

I. 📘 Based on Function Call and Definition

1. Formal Arguments (also called Parameters):
Variables that appear in the function definition.

Example:

def greet(name):  # 'name' is a formal argument
    print("Hello", name)

2. Actual Arguments:
Values passed to the function when calling it.

Example:
def greet(name):
    print("Hello", name)
greet("Shania")  # "Shania" is an actual argument

🟢 Key Rule:
Number and position of actual arguments must match the formal arguments, unless default or variable-length arguments are used.

II. 📙 Based on the Way Arguments Are Passed
There are four types of arguments in Python:

1. 🔹 Positional Arguments
Values are assigned to parameters in the order they appear.

Example:

def add(a, b):
    return a + b

add(2, 3)  # 2 → a, 3 → b

2. 🔹 Keyword Arguments
Arguments passed in the form key=value.

The order doesn’t matter.

Example:

def student(name, age):
    print(name, age)
student(age=13, name="Ava")  # Reordered but works fine

3. 🔹 Default Arguments
A default value is assigned to the parameter.

If not passed, the default is used.

Example:

def login(user="guest"):
    print("Welcome", user)
login()        # Uses default

4. 🔹 Variable-Length Arguments
Python supports two special symbols:

✅ *args (Non-keyword variable-length arguments)
Collects extra positional arguments into a tuple.

Used when the number of inputs is unknown.

Example:

def sum_all(*args):
    print(args)           # Tuple
    print(sum(args))

sum_all(1, 2, 3, 4)       # args = (1, 2, 3, 4)

🔄 Difference from Normal Positional Arguments:
Positional arguments: Fixed in number (formal and Actual arguments must match)
*args: Accepts any number of positional arguments dynamically.

✅ **kwargs (Keyword variable-length arguments)
Collects extra keyword arguments into a dictionary.

Example:

def user_info(**kwargs):
    print(kwargs)

user_info(name="Shania", age=30, country="India")

🔄 Difference from Normal Keyword Arguments:
Normal keyword arguments: Defined parameters with specific names.

**kwargs: Accepts any number of named parameters, dynamically captured as dictionary key-value pairs.
    
🧩 Summary Table: Parameters vs Arguments
Concept	                      Definition	                           Example
Formal Parameters    :	      Inside function definition	           def f(a, b):

Actual Arguments     :	      Values passed during function call	   f(10, 20)

Positional	         :        Ordered values passed directly	       f(1, 2)

Keyword	Passed using :        key=value format	                       f(x=1, y=2)

Default	Parameters   :        with default values	                   def f(a=5):

Variable-length	Arbitrary arguments: *args, **kwargs	               def f(*a, **b):






