# Topics:

1. Python vs Shell
2. Variables & Data Types
3. Typecasting
4. User inputs
5. Operators
6. if, elif, else Conditional Handling
7. loops
8. Data-type, String, String handling functions
9. Strings & Indexing
10. Functions, Modules, Packages & Virtual Environment
11. Command line arguments & Environment variables
12. Lists and Tuples


Q: Why Python or Shell vs Python?
* Any day-to-day tasks in a Linux system, like creating folders/files, checking memory/disks, we must know shell commands.
* The primary purpose, not the only purpose, of DevOps engineers is to interact with Linux systems.
* Shell is restricted to Linux systems, whereas Python is for both Linux and Windows.
* I can learn Ansible to interact with both the linux and windows so why learn python because Ansible is also written in Python.
* When we want to write some complex tasks, like interacting with an API or data manipulation. There python wins over shell scripting because Python is designed to perform these activities more simply.
* Example: We have a GitHub account with some 20-30 repositories. Our task is to list out all the issues that were created in the repository, and who is the author of that issue? Our task is talk to the API of GitHub that fetch issue of the repository and gets the author name from it.
* We can acheive this through shell or python but the modules of the python is rich then shell.


**Shortcuts & Best practises:**
* Clt+/                        # Comment selected lines
* After if statement, put ":"   # it will automatically make indentation on the next line.
* alt+click                    # type same thing on multiple line: press alt & click on the lines you want to write
* Snake casing:                # Snake case is a naming convention particularly for variables, functions, and module names. Writing names by joining words with underscores (_) and using only lowercase letters.
* Camel casing:                # Camel case is a naming convention where multiple words in a name are joined without spaces, and the first letter of each word is capitalized.

  
# Variables & Data Types:

* **Variables** are used to store the value of a **data type** temporarily. 
* **Data-type:** Categorize the type of values a variable can hold. How complier knows that which data type we have specified?
* Compiler knows through single or double inverted.
* If we mention anything inside '', "" qoutes consider as string.
* If we mention with inverted's will be considered as an integer or float if it is decimal.
* Below are some commonly used data types.
  
  1. integer (int)  - Whole numbers (1,2,5,19)
  2. float          - Decimal numbers (1.4, 0.9)
  3. string (str)   - Text enclosed in single or double quotes ("Hello", 'Python') 
  4. boolean (bool) - True or False
  5. list           - Ordered mutable collections (e.g., [1, 2, 3])
  6. tuple          - Ordered immutable collections (e.g., (1, 2, 3))
  7. sets           - Unordered collections of unique elements (e.g., {1, 2, 3})
  8. dictionary      - key-value pairs (e.g., {"name": "Alice", "age": 25 })
  
 **Important:** Python is a dynamically typed programming language where we do not need to specify the data-type of a variable; it automatically understands.

    name = "Sunny"
    Age = 35
    City = "Pune"
    Package = 18
    
    print(name)  # print the value of the variable
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
* Variable name must start with a letter (a-z, A-Z) or an underscore (_).
* They can contain letters, numbers, & underscores.
* Variable names are case sensitive (small & SMALL both will be treated differently)
* Avoid using keywords (e.g., if, for, while) as variable names.

# Typecasting in Python

* Type casting in Python, also known as type conversion, is the process of converting a value from one data type to another. This is often necessary when performing operations that require specific data types or when you need to change the representation of data for a particular purpose.

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

* Arithmatic:

      a = 30
      b = 20
      
      print(" a + b = ", a + b)
      print(" a - b = ", a - b)
      print(" a * b = ", a * b)
      print(" a / b = ", a / b)
      print(" a % b = ", a % b)
      print(" a // b = ", a // b)

Note: Last '//' is for the floor division that will ignore the digit after decimal

* Assignment Operators: used to assign values to variables. They take the value on their right side and store it in the variable on their left side. The most fundamental assignment operator is the equals sign (=).

      a = 30
      print(a)
      a*=2
      print(a)
      a+=5
      print(a)
      a-=6
      print(a)

* Comparision operators: It always give output as True or False

      a = 30
      b = 20
      
      print(a>b)
      print(a<b)
      print(a==b)
      print(a<=b)
      print(a>=b)

* Logical Operators: Three logical operators: and, or, and not. These operators are used to combine or modify conditional expressions, resulting in a Boolean value.

      print (True and False)
      print (True and True)
      print (False and False)
      print(False or True)

      print("Not Operator")
      print(not(True))
      print(not(False))


# If-Else Conditional Handling

* Conditional handling in Python allows for the execution of different blocks of code based on whether certain conditions are met.
* This is achieved through the use of **if, elif, and else** statements.

* If statement

    age = 30
    if (age > 15):
        print ("You are eligible to drive")
        print("Thank you")

* If else

    type = (input("Enter the required instance type: "))
    
    if type == "t2.micro":
        print("It will charge you 2 INR")
    
    elif type == "t2.medium":
        print("It will charge you 4 INR")
    
    elif type == "t2.large":
        print("It will cost you around 8 INR")
    
    else:
        print("Type is not valid instance type, please select a valid type of Instance")


      age = int(input("Enter your age: "))
  
      if(age > 18):
          print("You are elegible for driving")    # 4 spaces (indentation) in the begenning indicate that the print statement is inside the 'if' statement. 
      else:
          print("You are not eligible to drive")   # 4 spaces (indentation) in the begenning indicate that the print statement is inside the 'else' statement.
      print("End of Program")

Note: In above code, at the end, "End of Program" is not inside the 'else' statement hence it will always printed.

      age = int(input("Enter your Age: "))
      
      if (age > 20):
          print("You can drive")      # If age is more than 20 you can drive, this will print
      elif(age == 20):    # If age is exactly 20, schedule an interview
          print("Let's schedule an interview for re-evaluation")
      else:
          print("Sorry you cannot drive")


      if (age > 20):
          print("You can drive")      # If age is more than 20 you can drive, this will print
      elif(age == 20):    # If age is exactly 20, schedule an interview
          print("Let's schedule an interview for re-evaluation")
      elif(age == 0):
          print("oh my god! you are just born")
      else:
          print("Sorry you cannot drive")

* Match case

      a = int(input("Enter a number between 1 to 10: "))
      match(a):
          case 2:
              print("you won a mobile")
          case 4:
              print("you won a tablet")
          case 6:
              print("you won a cycle")
          case 8:
              print("you won a cap")
          case _:
              print("Sorry, better luck next time")

# Loops

* Every programming language this concept must exist.
* Loops is useful to perform repetetive action on a block of code.
* Python has two primitive loop commands:

1. for loops: Used when you know this block of code will run definite number of times. E.g., 2 times or 5 times.
2. while loops: While loops execute a block of code as long as a condition is True. They are useful when the number of operations is not known in advance. Example: Print 'files are deleting' till the time all the files are deleted from the specific folder.

* for loops: I want to print numbers from 1 to 10. So it will be 'n-1' take 1 number extra for e.g. here take 11

**For Loop Syntax:**

* for variable in sequence

    colors = ["blue", "green", "yellow"]
    for s in colors:
        print(s)

      for i in range(1, 11):
          print(i)
  
      for i in range(1, 5):
          print(2*(i))    # this will multiple 1-4 with 2
  
        for i in range(1, 11):
          print("5 X", i , "=", 5*i)    # it will print table of 5

  
Note: Everytime we put a comma ',' it will create a space


**while loops Syntax**:

      i = 1
      while i < 10:
          print(i)
          i = i + 1

Note: In above while loop code the control goes to the 'while' till the value of i is less than the value of i (10). It will check if its less than 10 than + 1 

* Break Loop: The break command allows you to terminate/cancel the execution of loop and exit a loop

      for i in range (1, 20):
          print(i)
          if i == 10:
              break

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

      fname = "sunny"      # concatenate and result in upper case with space in middle
      sname = "valechha"
      result = fname + " " + sname
      upperresult = result.upper()
      print(upperresult)

* Count the number of characters in a string using 'len'

      allout = "all insects is dead"
      print(len(allout))

* Replace

      text = "Python is Great !"
      update = text.replace("Great", "Awesome")
      print("modified text is: ", update)

* Strip: Remove unnecessary spaces

      speaker = "                                                              International day"
      striptext = speaker.strip()
      print(striptext)

* Substring

    text = "Boat is Great !"
    substring = "was"
    if substring in text:
        print(substring, "bla bla bla ho ho")
    else:
        print("no substring found")

* Integer dividation

    num2 = 10.88787
    num3 = 5.84474
    result = num2 // num3      # this '//' will result in single value, it will ignore numbers after decimal
    print(result)

* Modulus (Remainder)
  
    result2 = num1 % num2
    print("Modulus (Remainder):", result2)
    
* Absolute Value

    result3 = abs(-7)
    print("Absolute Value:", result3)

# Strings & Indexing

* Single line string: enclosed within a single pair of quotes

    single_string = "This is a single-line string."

* Multi-line-string: A multi-line string can span across multiple lines of code.

    multi_string = '''This is a
    multi-line string
    that spans multiple lines.'''

# Functions, Modules & Packages

* Functions in python used to bundle a set of instructions that you want to use repeatedly or, because of their complexity.
* A function is a block of code which only runs when it is called.
* In Python any function is defined using the **'def'** (defination) keyword.
* Once we define the function we must call the function by specifying the name of the function as per the variable rules. e.g., we have define the function named average and at last we have specified the value and call the function.
* Add parameters to the function: they should be within the parentheses of the function. End your line with a colon.
* End your function with a **return** statement if the function should output something. Without the **return** statement, your function will return an object **None**.


- Example: 1

      def average(a, b, c, d):
          apple = (a + b + c + d)/3
          print(apple)
      
      average(2, 4, 6, 8)
      
      - Example: 2
      
      num1 = 10
      num2 = 20
      
      def add():
          a = num1 + num2
          print(a)
      
      def sub():
          s = num2 - num1
          print(s)
      
      def mul():
          m = num1 * num2
          print(m)

* In both the above codes we did not call the function, hence it will not give any output after running the code, we have to call the function after the defining the function.
* Now, try below code there we have call the function it will give us the output.

      num1 = 10
      num2 = 20
      
      def add():
          a = num1 + num2
          print(a)
      
      def sub():
          s = num2 - num1
          print(s)
      
      def mul():
          m = num1 * num2
          print(m)
      
      add()
      sub()
      mul()



      def average(a, b, c, d):
          apple = (a + b + c + d)/3
          return apple
      
      boat = average(3, 5, 7, 9)
      
      print(boat)

* Module: A module is a group of functions. In example second we have created mulitple function of add, substract and multiple can be called as a module.

- Call the function with **import** keyword.

* We have create another file by the name 'call_the_function.py' and import the function written above in example: 2

    import functions
    
    functions

* Or it can be written as below.


      import functions as advance_calci
      
      advance_calci

<img width="782" height="351" alt="image" src="https://github.com/user-attachments/assets/e8588937-98af-433b-9eec-2f284d522550" />


* Call only one function.

      from functions import add
      
      add()

- Return: Functions take input, perform the required logic and returns the output.

      def mul(num1, num2):
          m = num1 * num2
          return m
      
      print(mul(10, 2))
      
      def sub(num1, num2):
          s = num1 - num2
          return s
      
      print(sub(20, 5))

- **Packages**: Packages are collection of modules. We can download a module from 'python package index' (PYPI)  an artifactory/registry for python packages just like we download a docker image from docker hub.

 * https://pypi.org/  > search 'aws' or 'boto3' you will get commands to install package.
 * Download the package with 'pip' e.g., '**pip install boto3**' '**pip install jira**'
 * Validate the package with '**pip show boto3**'
 * List all the installed packages '**pip list**'


- **Virtual Environment**: Each virtual environment is independent. Packages installed within one virtual environment do not affect other virtual environments or the global Python installation. This prevents version conflicts when different projects require different versions of the same library.

      python -m venv my-project-1    # -m - module | command will be the same for any module you want to install just the module name will be changed, A new folder will created

      source my-project-1/bin/activate    # activate the environment

      deactivate                # out from the virtual env


# Command line arguments & Enviroment variables

* Command line arguments: The arguments that are given after the name of the program in the command line shell are known as Command Line Arguments.
* Example - 'aws s3 ls' here aws is a python program whom we are trying to list the s3 buckets. Passing value in this way are called as Command Line Arguments.

* **Used-case**: Previously we wrote a function and module where we hardcode the values while calling the function, if someone wants to use the function they have to go inside the file and edit the values but in productions thing don't work this way.
* In Python there is a in-built module called '**sys**' which reads the command line arguments inside the program. **sys** is not a PYPI module it is by default comes along with the python installation.


# Lists and Tuples

* Both lists and tuples are indeed sequence data types in Python. This means they are ordered collections of items, and each item can be accessed by its position (index) within the sequence, but they differ fundamentally in their mutability (tendency to change).

- Lists:
* Mutable: Lists are mutable, meaning their contents can be changed after creation. Elements can be added, removed, or modified.
* Syntax: Defined using square brackets [].

- Tuples:
* Immutable: Tuples are immutable, meaning their contents cannot be changed after creation. Once a tuple is defined, its elements cannot be added, removed, or modified.
* Syntax: Defined using parentheses ().

- Indexing:
* Indexing refers to the process of accessing individual elements within a sequence data type, such as strings, lists, or tuples, by their position. Each element in a sequence is assigned a unique numerical index, starting from 0 for the first element.
* The first element of a sequence is always at index 0, the second at index 1, and so on.
* Elements are accessed using square brackets []
* -1: Refers to the last element of the sequence called as negative indexing.

    name = "Anjali"
    print(name[-1])  # it give result as 'i'

* Ex: 2
    s3_bucket = ["sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket"]
    print(s3_bucket)
    print(type(s3_bucket))    # type is list

* Ex: 3
    s3_bucket = ["sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket"]
    print(s3_bucket[0])    # here '0' is first figure that is sunny_bucket, so on 1, 2, and 3

* Ex: 4
    s3_bucket = ("sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket")
    print(type(s3_bucket))    # type is tuple

* Ex: 5
    s3_bucket = ("sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket")
    print(len(s3_bucket[3]))  # length of the 3rd statement is 16

* Ex: 6
  s3_bucket = ("sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket")
  s3_bucket.append("new_s3_bucket")
  print(s3_bucket)    # this throws an error as we cannot append in tuple, tuple is immutable

* Ex: 7
    s3_bucket = ("sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket")
    print(type(s3_bucket))
    print(s3_bucket[1])    # here, 1st value will be 'anjali_s3_bucket'

* Ex: 8
    s3_bucket = ["sunny_s3_bucket", "anjali_s3_bucket", "Micky_s3_bucket", "Saarth_s3_bucket"]
    s3_bucket.append("new_s3_bucket")
    s3_bucket.remove("sunny_s3_bucket")
    print(s3_bucket)    # append and remove 1-1 items




