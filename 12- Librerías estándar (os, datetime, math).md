# Curso de Python: Librerías Estándar (`os`, `datetime`, `math`)

Aprende a utilizar algunas de las librerías estándar más útiles en Python.

---

## Paso 1: Usar la librería `os` para interactuar con el sistema operativo

```python
import os

# Obtener el directorio actual
directorio_actual = os.getcwd()
print("Directorio actual:", directorio_actual)

# Listar archivos en el directorio actual
archivos = os.listdir('.')
print("Archivos:", archivos)

# Crear una carpeta nueva
os.mkdir('nueva_carpeta')
```

---

## Paso 2: Usar la librería `datetime` para manejar fechas y horas

```python
import datetime

# Obtener la fecha y hora actual
ahora = datetime.datetime.now()
print("Fecha y hora actual:", ahora)

# Crear una fecha específica
fecha = datetime.date(2025, 5, 29)
print("Fecha específica:", fecha)

# Sumar días a una fecha
nueva_fecha = fecha + datetime.timedelta(days=10)
print("Fecha + 10 días:", nueva_fecha)
```

---

## Paso 3: Usar la librería `math` para operaciones matemáticas

```python
import math

# Calcular la raíz cuadrada
print("Raíz cuadrada de 16:", math.sqrt(16))

# Calcular el seno de 90 grados (radianes)
print("Seno de 90°:", math.sin(math.radians(90)))

# Redondear números
print("Redondear 3.7 hacia abajo:", math.floor(3.7))
print("Redondear 3.7 hacia arriba:", math.ceil(3.7))
```

---

## Resumen

1. La librería `os` permite interactuar con el sistema de archivos.
2. La librería `datetime` facilita el manejo de fechas y horas.
3. La librería `math` ofrece funciones matemáticas avanzadas.

---