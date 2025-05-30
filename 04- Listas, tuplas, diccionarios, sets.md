# Curso Básico de Python: Estructuras de Datos

## 1. Listas

Las listas son colecciones ordenadas y mutables. Se definen usando corchetes `[]`.

```python
# Crear una lista
frutas = ["manzana", "banana", "cereza"]
print(frutas)

# Acceder a un elemento
print(frutas[1])  # banana

# Modificar un elemento
frutas[0] = "kiwi"
print(frutas)

# Agregar un elemento
frutas.append("naranja")
print(frutas)

# Eliminar un elemento
frutas.remove("banana")
print(frutas)
```

---

## 2. Tuplas

Las tuplas son colecciones ordenadas e inmutables. Se definen usando paréntesis `()`.

```python
# Crear una tupla
coordenadas = (10, 20)
print(coordenadas)

# Acceder a un elemento
print(coordenadas[0])  # 10

# Las tuplas no se pueden modificar
# coordenadas[0] = 15  # Esto dará error
```

---

## 3. Diccionarios

Los diccionarios almacenan pares clave-valor. Se definen usando llaves `{}`.

```python
# Crear un diccionario
persona = {"nombre": "Ana", "edad": 25}
print(persona)

# Acceder a un valor
print(persona["nombre"])  # Ana

# Modificar un valor
persona["edad"] = 26
print(persona)

# Agregar un nuevo par clave-valor
persona["ciudad"] = "Madrid"
print(persona)

# Eliminar un par clave-valor
del persona["nombre"]
print(persona)
```

---

## 4. Sets (Conjuntos)

Los sets son colecciones desordenadas de elementos únicos. Se definen usando llaves `{}` o la función `set()`.

```python
# Crear un set
numeros = {1, 2, 3, 4}
print(numeros)

# Agregar un elemento
numeros.add(5)
print(numeros)

# Eliminar un elemento
numeros.remove(3)
print(numeros)

# No permite elementos duplicados
numeros.add(2)
print(numeros)  # El 2 no se repite
```

---

## Resumen

- **Listas**: Ordenadas, mutables, permiten duplicados.
- **Tuplas**: Ordenadas, inmutables, permiten duplicados.
- **Diccionarios**: Pares clave-valor, mutables, claves únicas.
- **Sets**: Desordenados, mutables, solo elementos únicos.

¡Practica estos ejemplos para dominar las estructuras de datos básicas en Python!