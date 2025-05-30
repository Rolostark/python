# Curso de Python: Funciones y Manejo de Errores

## 1. Funciones

Las funciones permiten reutilizar código y organizarlo mejor.

### Definir una función

```python
def saludar(nombre):
    print("Hola,", nombre)

saludar("Ana")  # Imprime: Hola, Ana
```

### Función con retorno de valor

```python
def sumar(a, b):
    return a + b

resultado = sumar(3, 5)
print(resultado)  # Imprime: 8
```

### Parámetros por defecto

```python
def saludar(nombre="amigo"):
    print("Hola,", nombre)

saludar()           # Imprime: Hola, amigo
saludar("Carlos")   # Imprime: Hola, Carlos
```

---

## 2. Manejo de Errores (Excepciones)

Las excepciones permiten manejar errores sin que el programa se detenga.

### try - except

```python
try:
    numero = int(input("Ingresa un número: "))
    print("El doble es:", numero * 2)
except ValueError:
    print("¡Eso no es un número!")
```

### else y finally

```python
try:
    resultado = 10 / 2
except ZeroDivisionError:
    print("No se puede dividir por cero.")
else:
    print("La división fue exitosa.")
finally:
    print("Esto se ejecuta siempre.")
```

---

¡Listo! Ahora sabes cómo usar funciones y manejar errores en Python.