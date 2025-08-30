Q: Why Python or Shell vs Python?
A: Any day-2-day tasks in a linux systems like creating folders/files, checking memory/disks we must know shell commands. The primary purpose not the only purpose of Devops engineers is to interact with Linux systems.
* Shell is restricted to linux systems whereas python is for both linux and windows.
* I can learn ansible to interact with both the linux and windows so why to learn python because ansible is also written on python.
* When we want to write some complex tasks like to interact with API, data manupulation. There python wins over shell scripting because python is designed to perform these activities in a simpler way.
* Example: We have a github account in a account we have some 20-30 repositories, our tasks is to list out all the issues that created in the repository and who has the author of that issue? Our tasks is talk to the API of github that fetch issue of the repository and get the author name from it.
* We can acheive this through shell or python but the modules of the python is rich then shell.  





Shortcuts:
* Clt+/                        # Comment selected lines
* After if statement put ":"   # it will automatic make indentation on next line.
* alt+click                    # type same thing on multiple line: press alt & click on the lines you want to write
  


- Variables & Data Types:

* **Variables** used to temporary store the value of a data-type. 
* **Data-type:** Categorize the type of values a variable can hold. Below are the some commonly used data-types:
  
  1. integer (int)  - Whole numbers (1,2,5,19)
  2. float          - Decimal numbers (1.4, 0.9)
  3. string (str)   - Text enclosed in single or double quotes ("Hello", 'Python') 
  4. boolean (bool) - True or False
  5. list           - Ordered mutable collections (e.g., [1, 2, 3])
  6. tuple          - Ordered immutable collections (e.g., (1, 2, 3))
  7. sets           - Unordered collections of unique elements (e.g., {1, 2, 3})
  8. dictonary      - key-value pairs (e.g., {"name": "Alice", "age": 25 })
  
 **Important:** Python is a dynamically typed programming language where we do not need to specify the data-type of a variable, it automatically understands.

    name = "Sunny"
    Age = 35
    City = "Pune"
    Package = 18
    
    print(name)  # print the value of variable
    print(Age)
    print(City)
    print(Package)
    
    print (type(name))  # get the type of data-type
    print (type(Age))
    print (type(City))
    print (type(Package))

    this_task_is_completed = True # this also could be False
    print (this_task_is_completed)
    print(type(this_task_is_completed))

  - Rules to define variables:
* Variable name must start with letter (a-z, A-Z) or an underscore (_).
* They can contain letters, numbers, & underscores.
* Variables names are case sensitive (small & SMALL both will treated differentely)
* Avoid using keywords (e.g., if, for, while) as variable names.

# Typecasting in Python

* Type casting in Python, also known as type conversion, is the process of converting a value from one data type to another. This is often necessary when performing operations that require specific data types, or when you need to change the representation of data for a particular purpose.

Python supports two main types of type conversion:
* Implicit Type Conversion (Coercion): This occurs automatically when Python converts one data type to another without explicit instruction from the programmer.
* Explicit Type Conversion (Type Casting): This requires the programmer to explicitly use built-in functions to convert a value from one data type to another.

    a = 34
    b = "34"
    
    print(a)
    print(b)
    
    print(type(a))
    print(type(b))
    
    c = int(b)    # this converts type of value from one data-type to another like value of 'b' from string to integer
    print(c)
    print(type(c))

    d = bool(a)
    print(d)
    print(type(d))

# User input in Python
 
* User input in Python is primarily taken using the built-in **input()** function. The input() function prompts the user to enter text and waits for them to press Enter. Whatever the user types is returned as a string.

        a = input("Enter a name: ")
        print(a)
        print(type(a))
    
        b = input("Enter a number")
        print(b)
        print(type(b))

Note: Whatever value we assign for 'a/b' or 'input()' will be considered as string not integer even if we give input as a number still it is consider as string.

* Convert string into a integer

      c = input("Enter a number: ")
      c = int(c) # Convert c into int version of c
      print(c)
      print(type(c))
    
      c = input("Enter a number: ")
      c = int(c) # Convert c into int version of c
      print(c)
      print(type(c))
      print(c+10)  # here, we can add 10 in the output after converting into an integer else we cannot do.


Note: Another simple way to converting an string into inter is below:

      c = int(input("Enter a number: "))    # just put 'int' before "input()"
      print(c)
      print(type(c))
      print(c+10)

- Comments, Escape sequences & Print statements

* Clt+/ # comment multiple lines
* '''abc xyz''' # comment multiple lines with tripple single quotes

* Escape sequence: used to include special characters in string

    print("My name is sunny valechha \nmy wife's name is anjali \nson's name is saarth")

* \n will create a new line

    print("My name is sunny valechha \nmy wife's name is anjali \\ my son's name is saarth")

* double \\ is treated as single '\' so when you want to use single, in code use double.

    print ("Sunny \" Valechha")

* Suppose, you want to print double quote " somewhere but it cannot print directly so use (\")

# Operators

* Python operators are special symbols or keywords that perform operations on one or more operands (values or variables). They are categorized into several types:

1. Arithmetic Operators
2. Assignment Operators
3. Comparison Operators
4. Logical Operators
5. Identity Operators
6. Membership Operators
7. Bitwise Operators


# Data-type, String, String handling functions

* split the arn by last or second last word

    arn = "arn:aws:iam::123456789012:user/john"
    print(arn.split("/")[1])

* Convert name into upper case

    name = "sunny"
    print (name.upper())

* Concatenation of strings

    string1 = "Sunny"
    string2 = "Valechha"
    print (string1 + string2)

    string1 = "Sunny"
    string2 = "Valechha"
    result = (string1 + string2)
    print (result)

* Count the number of characters in a string using 'len'

  
