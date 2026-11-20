# Calculator-
# SMART CALCULATOR
# Mini Project - First Year Engineering

print("================================")
print("       SMART CALCULATOR")
print("================================")

while True:
    print("\nChoose an Operation:")
    print("1. Addition (+)")
    print("2. Subtraction (-)")
    print("3. Multiplication (*)")
    print("4. Division (/)")
    print("5. Modulus (%)")
    print("6. Exit")

    choice = input("\nEnter your choice (1-6): ")

    if choice == '6':
        print("Thank you for using Calculator!")
        break

    if choice in ['1', '2', '3', '4', '5']:
        num1 = float(input("Enter first number: "))
        num2 = float(input("Enter second number: "))

        if choice == '1':
            print("Result =", num1 + num2)

        elif choice == '2':
            print("Result =", num1 - num2)

        elif choice == '3':
            print("Result =", num1 * num2)

        elif choice == '4':
            if num2 != 0:
                print("Result =", num1 / num2)
            else:
                print("Error! Cannot divide by zero.")

        elif choice == '5':
            if num2 != 0:
                print("Result =", num1 % num2)
            else:
                print("Error! Cannot divide by zero.")

    else:
        print("Invalid choice! Try again.")
