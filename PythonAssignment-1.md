## Assignment Part-1
Q1. Why do we call Python as a general purpose and high-level programming language?
A. It can be used to create a variety of different programs and due to its versatility, along with beginner-friendly programming, It's also called general-purpose programming language. We call it as a High-level language because we are not required to concentratre on activities like memory management.


Q2. Why is Python called a dynamically typed language?
A. We call Python a dynamically typed language because here we are not required to mention the type of data we are assigning to a variable. Lets say, a = 10, Python will automatically select the type as integer.

Q3. List some pros and cons of Python programming language?
A. Pros.
    1. Simple & easy to learn
    2. Free & open source
    3. Dynamically typed
    4. Interpreted 
    5. High level 
    6. Both Procedure oriented & object oriented
    7. Vast library support
  Cons.
    1. Slow speed than compiled languages
    2. Security is not upto the mark
    3. Memory consumption and garbage collection
    4. Multithreading in python(Its not true multithreading due to its global interpreter lock)

Q4. In what all domains can we use Python?
A. 1. Web development
   2. Data Science 
   3. AI & ML
   4. Game development
   5. For IoT
   6. For automate scripting


Q5. What are variable and how can we declare them?
A.  Variables are one kind of identifiers. We can declare variables like we can use 
    (i) alphabet symbols(either lower case or upper case)
    (ii) Digits(0 to 9)
    (iii) underscore symbol (_)

Q6. How can we take an input from the user in Python?
A.  With the help of input function
    like,
    a = input("What is your name :")
    print(a)

Q7. What is the default datatype of the value that has been taken as an input using input() function?
A.  String

Q8. What is type casting?
A.  Type casting is basically changing the data type from one type to another.
    Like, a = 10.34 (float type)
    print(int(a))
It will print 10 (int type)

Q9. Can we take more than one input from the user using single input() function? If yes, how? If no, why?
A.  Yes, We can take multiple inputs from user using single input() with split() function.
    for example,
    a,b,c = input("give 3 numbers:").split(",")
    print("1st number", a)
    print("2nd number", b)
    print("3rd number", c)

Q10. What are keywords?
A.  In python, there are some words are reserved to represent some meaning or functionality. Those are the keywords, also called as reserved keywords. They are 
['False', 'None', 'True', 'and', 'as', 'assert', 'break', 'class', 'continue', 'def', 'del', 'elif', 'else', 
'except', 'finally', 'for', 'from', 'global', 'if', 'import', 'in', 'is', 'lambda', 'nonlocal', 'not', 'or', 
'pass', 'raise', 'return', 'try', 'while', 'with', 'yield']


Q11. Can we use keywords as a variable? Support your answer with reason.
A. No, We cannot.

Q12. What is indentation? What's the use of indentaion in Python?
A.  Indentation refers to the spaces at the beginning of a code line. Python uses indentation to indicate block of code.

Q13. How can we throw some output in Python?
A.  By using print() function

Q14. What are operators in Python?
A.  1. Arithmetic Operators
2. Relational Operators or Comparison Operators
3. Logical operators
4. Bitwise oeprators
5. Assignment operators
6. Special operators

Q15. What is difference between / and // operators?
A.  / means division operator, that always returns float value. But, // means floor division operator, if arguments are int type, then it will return int value. But, if at least one argument is float type, then it will return float value.

Q16. Write a code that gives following as an output.
```
iNeuroniNeuroniNeuroniNeuron
A.  print("iNeuron" * 4)

```

Q17. Write a code to take a number as an input from the user and check if the number is odd or even.
A.  
n = int(input("enter a num:"))
if n % 2 == 0:
    print(n, "is Even")
else:
    print(n, "is Odd")

Q18. What are boolean operator?
A. Boolean opeerators are basically True and False. 

Q19. What will the output of the following?
```
1 or 0

0 and 0

True and False and True

1 or 0 or 0
```
A.  1
    0
    False
    1

Q20. What are conditional statements in Python?
A.  if
    if - elif
    if - elif - else

Q21. What is use of 'if', 'elif' and 'else' keywords?
A. if - We use for checking condition is satisfyong or not. if not satisfying, then it will come to elif and if this condition is not satisfying, it will go for else.
for example,
if 49 % 2 == 0:
    print("divisible by 2")
elif 49 % 7 == 0:
    print("divisible by 7")
else:
    print("It can't be divisible by 7 or 2")

Q22. Write a code to take the age of person as an input and if age >= 18 display "I can vote". If age is < 18 display "I can't vote".
A.  
age = int(input("What is your age :"))
if age >= 18:
    print("I can vote")
else:
    print("I can't vote")
Q23. Write a code that displays the sum of all the even numbers from the given list.
```
numbers = [12, 75, 150, 180, 145, 525, 50]
sum = 0
for i in numbers:
    if i % 2 == 0:
        sum = sum + i
print("Sum of all even numbers :", sum)
```


Q24. Write a code to take 3 numbers as an input from the user and display the greatest no as output.
A.
a = int(input("Enter 1st number :"))
b = int(input("Enter 2nd number :"))
c = int(input("Enter 3rd number :"))
print("a:{}, b:{}, c:{}".format(a, b, c))
if a > b :
    print("a is greater :", a)
elif b > c:
    print("b is greater :", b)
else:
    print("c is greater :", c)

Q25. Write a program to display only those numbers from a list that satisfy the following conditions

- The number must be divisible by five

- If the number is greater than 150, then skip it and move to the next number

- If the number is greater than 500, then stop the loop
```
numbers = [12, 75, 150, 180, 145, 525, 50]
```

A.
numbers = [12, 75, 150, 180, 145, 525, 50]
numbers.sort()
n1 = []
for i in numbers:
    if i > 500:
        break
    elif i > 150:
        continue
    elif i % 5 == 0:
        n1.append(i)

print(n1)