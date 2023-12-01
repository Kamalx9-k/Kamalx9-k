# Funktion für die Addition
def add(x, y):
    return x + y

# Funktion für die Subtraktion
def subtract(x, y):
    return x - y

# Funktion für die Multiplikation
def multiply(x, y):
    return x * y

# Funktion für die Division
def divide(x, y):
    if y == 0:
        return "Division durch Null nicht möglich"
    return x / y

print("Wähle eine Operation:")
print("1. Addition")
print("2. Subtraktion")
print("3. Multiplikation")
print("4. Division")

while True:
    # Benutzereingabe für die Auswahl der Operation
    choice = input("Gib deine Wahl (1/2/3/4) ein: ")

    # Überprüfung, ob die Eingabe eine der Optionen ist
    if choice in ('1', '2', '3', '4'):
        num1 = float(input("Gib die erste Zahl ein: "))
        num2 = float(input("Gib die zweite Zahl ein: "))

        if choice == '1':
            print(num1, "+", num2, "=", add(num1, num2))

        elif choice == '2':
            print(num1, "-", num2, "=", subtract(num1, num2))

        elif choice == '3':
            print(num1, "*", num2, "=", multiply(num1, num2))

        elif choice == '4':
            print(num1, "/", num2, "=", divide(num1, num2))
        break
    else:
        print("Ungültige Eingabe")
