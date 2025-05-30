# Curso de Python: Estructuras de Control

¡Bienvenido a este curso paso a paso sobre las estructuras de control en Python! Aquí aprenderás a usar condicionales (`if`) y bucles (`for`, `while`) con ejemplos prácticos.

---

## 1. ¿Qué son las Estructuras de Control?

Las estructuras de control permiten modificar el flujo de ejecución de tu programa, permitiendo tomar decisiones o repetir acciones.

---

## 2. Condicionales: `if`, `elif`, `else`

### Sintaxis básica

```python
if condición:
    # Bloque si la condición es verdadera
elif otra_condición:
    # Bloque si la otra condición es verdadera
else:
    # Bloque si ninguna condición es verdadera
```

### Ejemplo

```python
edad = 18
if edad >= 18:
    print("Eres mayor de edad.")
else:
    print("Eres menor de edad.")
```

**Salida:**  
`Eres mayor de edad.`

---

## 3. Bucle `for`

El bucle `for` se utiliza para iterar sobre una secuencia (lista, tupla, string, etc.).

### Sintaxis básica

```python
for variable in secuencia:
    # Código a ejecutar en cada iteración
```

### Ejemplo

```python
frutas = ['manzana', 'banana', 'cereza']
for fruta in frutas:
    print(fruta)
```

**Salida:**  
```
manzana
banana
cereza
```

**Ejemplo con rango de números:**

```python
for i in range(5):
    print(i)
```

**Salida:**  
```
0
1
2
3
4
```

---

## 4. Bucle `while`

El bucle `while` ejecuta un bloque de código mientras una condición sea verdadera.

### Sintaxis básica

```python
while condición:
    # Código a ejecutar mientras la condición es verdadera
```

### Ejemplo

```python
contador = 0
while contador < 3:
    print("Contador:", contador)
    contador += 1
```

**Salida:**  
```
Contador: 0
Contador: 1
Contador: 2
```

---

## 5. Ejercicio Práctico

### Problema

Pide al usuario un número y muestra si es par o impar usando una estructura `if`, y luego imprime todos los números del 0 al número ingresado usando un bucle `for`.

### Solución

```python
n = int(input("Introduce un número: "))

if n % 2 == 0:
    print("El número es par.")
else:
    print("El número es impar.")

print("Números del 0 al", n)
for i in range(n + 1):
    print(i)
```

---

## 6. Resumen

- Usa `if`, `elif`, `else` para tomar decisiones.
- Usa `for` para iterar una cantidad conocida de veces.
- Usa `while` para repetir mientras una condición sea verdadera.

---

## 7. Siguiente paso

Practica creando tus propios ejemplos y combinando las estructuras de control. ¡La práctica te ayudará a dominar estos conceptos!

---

¿Listo para el siguiente módulo? ¡Avísame si quieres seguir aprendiendo!