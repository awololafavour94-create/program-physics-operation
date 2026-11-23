# Program for 5 More Physics Operations

# Function 1: Calculate Potential Energy
def potential_energy():
    mass = float(input("Enter mass (kg): "))
    gravity = 9.8
    height = float(input("Enter height (metres): "))
    result = mass * gravity * height
    print("Potential Energy =", result, "Joules")


# Function 2: Calculate Density
def density():
    mass = float(input("Enter mass (kg): "))
    volume = float(input("Enter volume (m³): "))
    result = mass / volume
    print("Density =", result, "kg/m³")


# Function 3: Calculate Pressure
def pressure():
    force = float(input("Enter force (Newtons): "))
    area = float(input("Enter area (m²): "))
    result = force / area
    print("Pressure =", result, "Pascals")


# Function 4: Calculate Momentum
def momentum():
    mass = float(input("Enter mass (kg): "))
    velocity = float(input("Enter velocity (m/s): "))
    result = mass * velocity
    print("Momentum =", result, "kg m/s")


# Function 5: Calculate Power
def power():
    work = float(input("Enter work done (Joules): "))
    time = float(input("Enter time (seconds): "))
    result = work / time
    print("Power =", result, "Watts")


# Main Program
while True:
    print("\n===== PHYSICS CALCULATOR 2 =====")
    print("1. Potential Energy")
    print("2. Density")
    print("3. Pressure")
    print("4. Momentum")
    print("5. Power")

    choice = input("Choose an operation (1-5): ")

    if choice == "1":
        potential_energy()

    elif choice == "2":
        density()

    elif choice == "3":
        pressure()

    elif choice == "4":
        momentum()

    elif choice == "5":
        power()

    else:
        print("Invalid choice. Please select 1-5.")

    again = input("\nDo you want to continue? (yes/no): ")

    if again.lower() != "yes":
        print("Thank you for using the Physics Calculator!")
        break