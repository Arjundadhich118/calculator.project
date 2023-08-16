# calculator.project
Experience quick and simple calculations with our Basic Calculator program in Python. This user-friendly tool allows you to perform essential arithmetic operations such as addition, subtraction, multiplication, and division effortlessly.

def add(x, y):
   
    return x + y

def subtract(x, y):
   
    return x - y

def multiply(x, y):

    return x * y

def divide(x, y):
  
     return x / y

def calculator():
   
    print("Welcome to the calculator!")
    print("Select operation:")
    print("1. Addition")
    print("2. Subtraction")
    print("3. Multiplication")
    print("4. Division")

    choice = input("Enter choice (1/2/3/4): ")

    num1 = float(input("Enter first number: "))
    num2 = float(input("Enter second number: "))

    if choice == '1':
        print(num1, "+", num2, "=", add(num1, num2))
    elif choice == '2':
        print(num1, "-", num2, "=", subtract(num1, num2))
    elif choice == '3':
        print(num1, "*", num2, "=", multiply(num1, num2))
    elif choice == '4':
        if num2 == 0:
            print("Error: division by zero is not allowed")
        else:
            print(num1, "/", num2, "=", divide(num1, num2))
    else:
        print("Invalid input")

calculator()
