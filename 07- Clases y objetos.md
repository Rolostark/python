# Curso de Python: Clases y Objetos

## Introducción

En Python, las **clases** y los **objetos** son conceptos fundamentales de la programación orientada a objetos. Una **clase** es un molde o plantilla para crear **objetos**, que son instancias de esa clase.

---

## Paso 1: Definir una clase

Para definir una clase en Python, se utiliza la palabra clave `class`.

```python
class Persona:
    pass  # Esto indica una clase vacía
```

---

## Paso 2: Añadir un método constructor

El método `__init__` se llama automáticamente cuando se crea un objeto de la clase.

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad
```

---

## Paso 3: Crear un objeto

Para crear un objeto, simplemente llama a la clase como si fuera una función:

```python
persona1 = Persona("Ana", 30)
```

---

## Paso 4: Acceder a atributos y métodos

Puedes acceder a los atributos y métodos del objeto usando el punto (`.`):

```python
print(persona1.nombre)  # Salida: Ana
print(persona1.edad)    # Salida: 30
```

---

## Paso 5: Añadir métodos a la clase

Puedes definir métodos que realicen acciones utilizando los atributos del objeto:

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        print(f"Hola, mi nombre es {self.nombre} y tengo {self.edad} años.")
```

Ahora puedes usar el método `saludar`:

```python
persona1 = Persona("Ana", 30)
persona1.saludar()
# Salida: Hola, mi nombre es Ana y tengo 30 años.
```

---

## Paso 6: Ejemplo completo

```python
class Persona:
    def __init__(self, nombre, edad):
        self.nombre = nombre
        self.edad = edad

    def saludar(self):
        print(f"Hola, mi nombre es {self.nombre} y tengo {self.edad} años.")

# Crear un objeto
persona1 = Persona("Ana", 30)

# Usar método
persona1.saludar()
```

---

## Resumen

- Una **clase** es una plantilla para crear **objetos**.
- Los **objetos** contienen atributos y métodos.
- El método especial `__init__` inicializa los atributos del objeto.
- Los métodos son funciones definidas dentro de la clase que pueden usar los atributos del objeto.

---

¡Ahora ya sabes cómo crear y usar clases y objetos en Python!