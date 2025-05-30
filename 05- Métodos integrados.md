# Curso de Python: Métodos Integrados

En este curso aprenderás sobre los métodos integrados (built-in methods) más utilizados en Python, cómo usarlos y ejemplos prácticos de cada uno.

---

## 1. ¿Qué son los métodos integrados?

Los métodos integrados en Python son funciones que ya vienen definidas en el lenguaje. Pueden ser funciones globales (como `print()` o `len()`) o métodos asociados a tipos de datos (como `.append()` en listas).

---

## 2. Ejemplos de métodos integrados

### 2.1. Métodos de cadenas (`str`)

```python
texto = "hola mundo"

# .upper() - Convierte todo el texto a mayúsculas
print(texto.upper())  # HOLA MUNDO

# .capitalize() - Capitaliza la primera letra
print(texto.capitalize())  # Hola mundo

# .replace() - Reemplaza una subcadena por otra
print(texto.replace("mundo", "Python"))  # hola Python
```

---

### 2.2. Métodos de listas (`list`)

```python
numeros = [1, 2, 3]

# .append() - Agrega un elemento al final
numeros.append(4)
print(numeros)  # [1, 2, 3, 4]

# .remove() - Elimina la primera aparición de un elemento
numeros.remove(2)
print(numeros)  # [1, 3, 4]

# .reverse() - Invierte el orden de la lista
numeros.reverse()
print(numeros)  # [4, 3, 1]
```

---

### 2.3. Métodos de diccionarios (`dict`)

```python
persona = {"nombre": "Ana", "edad": 25}

# .keys() - Devuelve las claves
print(persona.keys())  # dict_keys(['nombre', 'edad'])

# .values() - Devuelve los valores
print(persona.values())  # dict_values(['Ana', 25])

# .get() - Obtiene el valor de una clave
print(persona.get("nombre"))  # Ana
```

---

## 3. Funciones integradas útiles

- `print()`: Imprime en pantalla.
- `len()`: Cuenta la longitud de un objeto.
- `type()`: Devuelve el tipo de dato.
- `range()`: Genera una secuencia de números.

```python
mi_lista = [1, 2, 3]
print(len(mi_lista))      # 3
print(type(mi_lista))     # <class 'list'>
print(list(range(5)))     # [0, 1, 2, 3, 4]
```

---

## 4. Ejercicio práctico

**Crea una lista de palabras y realiza lo siguiente:**
- Convierte todas las palabras a mayúsculas.
- Agrega una palabra nueva.
- Elimina la primera palabra.
- Imprime la lista final.

```python
palabras = ["python", "curso", "métodos"]
palabras = [p.upper() for p in palabras]
palabras.append("INTEGRADOS")
palabras.pop(0)
print(palabras)  # ['CURSO', 'MÉTODOS', 'INTEGRADOS']
```

---

## 5. Resumen

Los métodos integrados te ayudan a trabajar eficientemente con los principales tipos de datos en Python. Practica con estos ejemplos y prueba otros métodos consultando la [documentación oficial de Python](https://docs.python.org/3/library/stdtypes.html).

---