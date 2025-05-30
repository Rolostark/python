# Curso de Python: Métodos Mágicos (`__init__`, `__str__`)

## Introducción

En Python, los *métodos mágicos* (también llamados *dunder methods* por “double underscore”) son funciones especiales que permiten definir el comportamiento de los objetos cuando interactúan con las operaciones básicas del lenguaje (creación, impresión, operadores, etc.).

En este ejemplo, aprenderás dos de los métodos mágicos más usados: `__init__` y `__str__`.

---

## 1. ¿Qué es `__init__`?

- Es el método que se ejecuta automáticamente cuando creas una nueva instancia de una clase.
- Sirve para inicializar los atributos del objeto (constructor).

### Ejemplo:

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

# Crear un objeto:
persona1 = Persona("Ana", 30)
print(persona1.nombre)  # Salida: Ana
print(persona1.edad)    # Salida: 30
```

---

## 2. ¿Qué es `__str__`?

- Es el método que define cómo se representa el objeto como una cadena de texto.
- Se ejecuta cuando usas `print(objeto)` o `str(objeto)`.

### Ejemplo:

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
    
    def __str__(self):
        return f"{self.nombre} tiene {self.edad} años"

persona1 = Persona("Ana", 30)
print(persona1)  # Salida: Ana tiene 30 años
```

---

## 3. Ejemplo completo

```python
class Libro:
    def __init__(self, titulo, autor):
        self.titulo = titulo
        self.autor = autor

    def __str__(self):
        return f"'{self.titulo}' escrito por {self.autor}"

libro1 = Libro("Cien años de soledad", "Gabriel García Márquez")
print(libro1)
# Salida: 'Cien años de soledad' escrito por Gabriel García Márquez
```

---

## 4. Resumen

- `__init__`: Se usa para inicializar los nuevos objetos.
- `__str__`: Se usa para definir la representación en texto del objeto.

Estos métodos te permiten construir clases más útiles y fáciles de usar en tus proyectos de Python.

---

## Ejercicio Propuesto

Crea una clase llamada `Coche` que tenga los atributos `marca` y `modelo`. 
- Inicializa estos atributos con `__init__`.
- Define `__str__` para que al imprimir el objeto muestre: `"Coche: {marca} - Modelo: {modelo}"`.

```python
# Tu solución aquí
```