# Curso de Python: List Comprehensions

En este módulo aprenderás qué son las **list comprehensions** en Python, cómo utilizarlas y verás ejemplos prácticos para comprender su uso y ventajas.

---

## 1. ¿Qué es una List Comprehension?

Una **list comprehension** es una forma concisa de crear listas en Python. Permite generar una nueva lista aplicando una expresión a cada elemento de una secuencia, opcionalmente filtrando elementos con una condición.

**Sintaxis básica:**
```python
nueva_lista = [expresión for elemento in iterable]
```

**Con condición:**
```python
nueva_lista = [expresión for elemento in iterable if condición]
```

---

## 2. Ejemplo básico

Crear una lista de los cuadrados de los números del 0 al 9:

```python
cuadrados = [x**2 for x in range(10)]
print(cuadrados)  # [0, 1, 4, 9, 16, 25, 36, 49, 64, 81]
```

---

## 3. Ejemplo con condición

Obtener los números pares de una lista:

```python
numeros = [1, 2, 3, 4, 5, 6, 7, 8, 9, 10]
pares = [n for n in numeros if n % 2 == 0]
print(pares)  # [2, 4, 6, 8, 10]
```

---

## 4. List comprehension con transformación de datos

Convertir una lista de palabras a mayúsculas:

```python
palabras = ["python", "curso", "comprehension"]
mayusculas = [palabra.upper() for palabra in palabras]
print(mayusculas)  # ['PYTHON', 'CURSO', 'COMPREHENSION']
```

---

## 5. List comprehension usando una función

Aplicar una función a cada elemento:

```python
def triple(n):
    return n * 3

numeros = [1, 2, 3, 4]
triples = [triple(x) for x in numeros]
print(triples)  # [3, 6, 9, 12]
```

---

## 6. Ejemplo anidado (doble for)

Generar combinaciones de dos listas:

```python
letras = ['a', 'b']
numeros = [1, 2]
combinaciones = [(letra, numero) for letra in letras for numero in numeros]
print(combinaciones)  # [('a', 1), ('a', 2), ('b', 1), ('b', 2)]
```

---

## 7. Otras comprehensions

Python permite comprehensions con otros tipos de colecciones:

- **Set comprehension:**  
  ```python
  cuadrados = {x**2 for x in range(5)}
  print(cuadrados)  # {0, 1, 4, 9, 16}
  ```

- **Dictionary comprehension:**  
  ```python
  pares = {x: x**2 for x in range(5)}
  print(pares)  # {0: 0, 1: 1, 2: 4, 3: 9, 4: 16}
  ```

---

## 8. Ejercicio práctico

**Crea una lista con los números del 1 al 20, pero solo incluye aquellos que sean múltiplos de 3 o 5.**

```python
resultado = [n for n in range(1, 21) if n % 3 == 0 or n % 5 == 0]
print(resultado)  # [3, 5, 6, 9, 10, 12, 15, 18, 20]
```

---

## 9. Resumen

Las **list comprehensions** hacen tu código más limpio y eficiente para crear listas a partir de otras secuencias o iterables. Practica estos ejemplos y prueba a crear tus propias comprehensions con diferentes condiciones y expresiones.

---