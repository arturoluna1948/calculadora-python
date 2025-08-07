# Calculadora en Python

Este es un proyecto básico de calculadora hecho en Python como parte de mi bootcamp de soporte IT.  
Primero cumple con la instrucción obligatoria de sumar dos números, y después ofrece operaciones extra.

## Código

```python
# Calculadora en Python para principiantes

# Parte obligatoria: suma de dos números
numero1 = float(input("Ingresa el primer número: "))
numero2 = float(input("Ingresa el segundo número: "))
resultado = numero1 + numero2
print("La suma de los dos números es:", resultado)

# Extras: otras operaciones
print("\n¿Quieres hacer otra operación?")
print("1. Resta")
print("2. Multiplicación")
print("3. División")
print("4. Módulo (resto)")
print("5. Suma de 3 números")
print("6. Operación combinada (ej: 2 + 4 - 3)")

opcion = input("Escribe el número de la opción que quieras usar: ")

if opcion == "1":
    a = float(input("Ingresa el primer número: "))
    b = float(input("Ingresa el segundo número: "))
    print("Resultado:", a - b)

elif opcion == "2":
    a = float(input("Ingresa el primer número: "))
    b = float(input("Ingresa el segundo número: "))
    print("Resultado:", a * b)

elif opcion == "3":
    a = float(input("Ingresa el primer número: "))
    b = float(input("Ingresa el segundo número: "))
    if b != 0:
        print("Resultado:", a / b)
    else:
        print("No se puede dividir entre cero.")

elif opcion == "4":
    a = int(input("Ingresa el primer número (entero): "))
    b = int(input("Ingresa el segundo número (entero): "))
    print("Resultado del módulo:", a % b)

elif opcion == "5":
    a = float(input("Número 1: "))
    b = float(input("Número 2: "))
    c = float(input("Número 3: "))
    print("Resultado:", a + b + c)

elif opcion == "6":
    operacion = input("Escribe una operación como 2 + 4 - 3 * 2: ")
    try:
        resultado = eval(operacion)
        print("Resultado:", resultado)
    except:
        print("La operación no es válida.")

else:
    print("Opción no válida.")
