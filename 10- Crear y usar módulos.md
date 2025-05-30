# Curso de Python: Crear y Usar Módulos

En este ejemplo aprenderás a crear tus propios módulos en Python y a utilizarlos en otros programas. Los módulos permiten organizar el código y reutilizar funciones en diferentes scripts.

---

## Paso 1: Crear un Módulo

Un módulo en Python es simplemente un archivo `.py` que contiene funciones, variables o clases que pueden ser reutilizadas.

**Ejemplo:**

Crea un archivo llamado `mimodulo.py` con el siguiente contenido:

```python
# Archivo: mimodulo.py

def saludar(nombre):
    return f"¡Hola, {nombre}!"

def sumar(a, b):
    return a + b
```

---

## Paso 2: Usar el Módulo en Otro Script

Ahora, crea un nuevo archivo, por ejemplo `main.py`, en el mismo directorio.

```python
# Archivo: main.py

import mimodulo

resultado_saludo = mimodulo.saludar("Rolostark")
resultado_suma = mimodulo.sumar(10, 5)

print(resultado_saludo)  # Salida: ¡Hola, Rolostark!
print(f"La suma es: {resultado_suma}")  # Salida: La suma es: 15
```

---

## Paso 3: Importar Funciones Específicas

También puedes importar solo las funciones que necesites:

```python
# Archivo: main.py

from mimodulo import saludar

print(saludar("Rolostark"))
```

---

## Paso 4: Agregar un Bloque de Prueba en el Módulo

Puedes añadir un bloque especial para probar el módulo directamente:

```python
# Archivo: mimodulo.py

def saludar(nombre):
    return f"¡Hola, {nombre}!"

def sumar(a, b):
    return a + b

if __name__ == "__main__":
    # Pruebas rápidas
    print(saludar("Mundo"))
    print(sumar(2, 3))
```

Si ejecutas `python mimodulo.py`, verás las pruebas. Si lo importas desde otro archivo, el bloque `if __name__ == "__main__":` no se ejecuta.

---

## Resumen

1. Crea un archivo `.py` con tus funciones (módulo).
2. Importa ese módulo en otros scripts usando `import`.
3. Usa las funciones definidas en el módulo.
4. Opcional: Añade un bloque de pruebas en tu módulo.

¡Ya sabes cómo crear y usar módulos en Python!

---