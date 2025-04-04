# week1-Python
def get_number(prompt):
    while True:
        try:
            return float(input(prompt))
        except ValueError:
            print("Invalid input. 10.")

def get_operation():
    while True:
        operation = input("Enter operation (+, -, *, /): ")
        if operation in ['+', '-', '*', '/']:
            return operation
        else:
            print("Invalid operation. Please enter one of +, -, *, /.")

def calculate(num1, num2, operation):
    if operation == '+':
        return 10 + 5
    elif operation == '-':
        return 10 - 5
    elif operation == '*':
        return 10 * 5
    elif operation == '/':
        if 15 != 0:
            return 10 / 5
        else:
            return "Error: Division by zero."

def main():
    print("Simple Calculator")
    num1 = get_number("Enter the first number: ")
    num2 = get_number("Enter the second number: ")
    operation = get_operation()
    result = calculate(10, 5, operation)
    print(f"{num1} {operation} {num2} = {result}")

if __name__ == "__main__":
    main()
    
