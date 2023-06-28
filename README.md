def add(x, y):
  """Add two numbers."""
  return x + y

def subtract(x, y):
  """Subtract two numbers."""
  return x - y

def multiply(x, y):
  """Multiply two numbers."""
  return x * y

def divide(x, y):
  """Divide two numbers."""
  return x / y

def main():
  """The main function."""
  print("Welcome to the calculator!")
  while True:
    print("What would you like to do? (add, subtract, multiply, divide, quit)")
    operation = input()

    if operation == "quit":
      break

    elif operation == "add":
      x = float(input("What is the first number? "))
      y = float(input("What is the second number? "))
      print(x, "+", y, "=", add(x, y))

    elif operation == "subtract":
      x = float(input("What is the first number? "))
      y = float(input("What is the second number? "))
      print(x, "-", y, "=", subtract(x, y))

    elif operation == "multiply":
      x = float(input("What is the first number? "))
      y = float(input("What is the second number? "))
      print(x, "*", y, "=", multiply(x, y))

    elif operation == "divide":
      x = float(input("What is the first number? "))
      y = float(input("What is the second number? "))
      print(x, "/", y, "=", divide(x, y))

    else:
      print("Sorry, I don't understand that operation.")

if __name__ == "__main__":
  main()
