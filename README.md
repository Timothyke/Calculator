import sys

def add(num1, num2):
    return num1 + num2

def subtract(num1, num2):
    return num1 - num2

def multiply(num1, num2):
    return num1 * num2

def divide(num1, num2):
    if num2 == 0:
        print("Error: Cannot divide by zero")
        return sys.exit()
    else:
        return num1 / num2

while True:
    print("\nCalculator Menu")
    print("1. Add")
    print("2. Subtract")
    print("3. Multiply")
    print("4. Divide")
    print("5. Exit")

    choice = int(input("Enter your choice: "))

    if choice == 1:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        result = add(num1, num2)
        print("The sum of", num1, "and", num2, "is", result)
    elif choice == 2:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        result = subtract(num1, num2)
        print("The difference of", num1, "and", num2, "is", result)
    elif choice == 3:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        result = multiply(num1, num2)
        print("The product of", num1, "and", num2, "is", result)
    elif choice == 4:
        num1 = float(input("Enter the first number: "))
        num2 = float(input("Enter the second number: "))
        result = divide(num1, num2)
        print("The quotient of", num1, "and", num2, "is", result)
    elif choice == 5:
        print("Thank you for using my calculator!")
        sys.exit()
    else:
        print("Invalid choice. Please enter a number between 1 and 5.")
# Calculator
