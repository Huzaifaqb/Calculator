# Calculator
Simple Python Calculator
print("Welcome to HB'S Calculator")

def add(n1, n2):
    return n1 + n2

def subtract(n1, n2):
    return n1 - n2

def multiply(n1,n2):
    return n1 * n2

def divide(n1, n2):
    return n1 % n2

Operations = {
    "+" : add,
    "-" : subtract,
    "*" : multiply,
    "%" : divide
}
num1 = float(input("Enter fist number"))
for symbol in Operations:
    print(symbol)

operation_symbol = input("Pick operation")
num2 = float(input("enter 2nd number"))
answer = Operations[operation_symbol](num1,num2)
print(f"{num1} {operation_symbol} {num2} = {answer}")
