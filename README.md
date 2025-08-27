# conversor_temperatura.py

def celsius_para_fahrenheit(c):
    return (c * 9/5) + 32

def celsius_para_kelvin(c):
    return c + 273.15

def fahrenheit_para_celsius(f):
    return (f - 32) * 5/9

def fahrenheit_para_kelvin(f):
    return (f - 32) * 5/9 + 273.15

def kelvin_para_celsius(k):
    return k - 273.15

def kelvin_para_fahrenheit(k):
    return (k - 273.15) * 9/5 + 32

def main():
    while True:
        print("\n=== Conversor de Temperatura ===")
        print("1. Celsius → Fahrenheit/Kelvin")
        print("2. Fahrenheit → Celsius/Kelvin")
        print("3. Kelvin → Celsius/Fahrenheit")
        print("4. Sair")
        
        opcao = input("Escolha uma opção: ")
        
        if opcao == "1":
            c = float(input("Digite a temperatura em Celsius: "))
            print(f"Fahrenheit: {celsius_para_fahrenheit(c):.2f}")
            print(f"Kelvin: {celsius_para_kelvin(c):.2f}")
        elif opcao == "2":
            f = float(input("Digite a temperatura em Fahrenheit: "))
            print(f"Celsius: {fahrenheit_para_celsius(f):.2f}")
            print(f"Kelvin: {fahrenheit_para_kelvin(f):.2f}")
        elif opcao == "3":
            k = float(input("Digite a temperatura em Kelvin: "))
            print(f"Celsius: {kelvin_para_celsius(k):.2f}")
            print(f"Fahrenheit: {kelvin_para_fahrenheit(k):.2f}")
        elif opcao == "4":
            print("Saindo...")
            break
        else:
            print("Opção inválida!")

if __name__ == "__main__":
    main()

