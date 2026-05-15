print("""---Unit_converter---
---Please unit 1 that show---
1. F = (C * 1.8) + 32 
2. C = (F - 32) / 1.8
3. m = Km * 1000
4. Km = m / 1000
F:fahrenheit
C:celsius
Km:kirometer
m:meter
""")

type_number = int(input("Enter a Number: "))
if type_number == 1 or type_number == 2 or type_number == 3 or type_number == 4:
    if type_number == 1:
        unit = float(input("Enter a Unit (C:celsius): "))
        F = (unit * 1.8) + 32
        print("F = %.2f"% F)
    elif type_number == 2:
        unit = float(input("Enter a Unit (F:fahrenheit): "))
        C = (unit - 32) / 1.8
        print("C = %.2f"% C)
    elif type_number == 3:
        unit = float(input("Enter a Unit (Km:kirometer): "))
        m = unit * 1000
        print("m = %.2f"% m)
    elif type_number == 4:
        unit = float(input("Enter a Unit (m:meter): "))
        Km = unit / 1000
        print("Km = %.2f"% Km)
    else:
        print("Invalid Input")
else:
    print("Sorry, I don't have that unit")
