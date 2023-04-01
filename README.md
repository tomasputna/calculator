# calculator

Pro spuštění kalkulačky stačí tento zdrojový kód uložit jako soubor s příponou .py a poté spustit v Pythonu.

`python
def add(x, y):
    return x + y

def subtract(x, y):
    return x - y

def multiply(x, y):
    return x * y

def divide(x, y):
    return x / y

print("Vyberte operaci.")
print("1.Sčítání")
print("2.Odčítání")
print("3.Násobení")
print("4.Dělení")

while True:
    volba = input("Zadejte volbu(1/2/3/4): ")

    if volba in ('1', '2', '3', '4'):
        cislo1 = float(input("Zadejte první číslo: "))
        cislo2 = float(input("Zadejte druhé číslo: "))

        if volba == '1':
            print(cislo1, "+", cislo2, "=", add(cislo1, cislo2))

        elif volba == '2':
            print(cislo1, "-", cislo2, "=", subtract(cislo1, cislo2))

        elif volba == '3':
            print(cislo1, "*", cislo2, "=", multiply(cislo1, cislo2))

        elif volba == '4':
            print(cislo1, "/", cislo2, "=", divide(cislo1, cislo2))
        break
    else:
        print("Nesprávná volba.")

`
