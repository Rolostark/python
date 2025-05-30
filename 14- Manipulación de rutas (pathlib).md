# Curso de Python: Manipulación de Rutas con `pathlib`

Organiza y manipula rutas de archivos de forma moderna y sencilla.

---

## Paso 1: Importar `pathlib`

```python
from pathlib import Path
```

---

## Paso 2: Crear rutas y comprobar existencia

```python
ruta = Path('ejemplo.txt')

# Verificar si existe
print("¿Existe?", ruta.exists())

# Obtener carpeta padre
print("Carpeta padre:", ruta.parent)
```

---

## Paso 3: Listar archivos en un directorio

```python
carpeta = Path('.')
for archivo in carpeta.iterdir():
    print(archivo)
```

---

## Paso 4: Crear directorios y archivos

```python
# Crear un directorio
nueva_carpeta = Path('mi_carpeta')
nueva_carpeta.mkdir(exist_ok=True)

# Crear un archivo dentro
nuevo_archivo = nueva_carpeta / 'nuevo.txt'
nuevo_archivo.write_text("Contenido de prueba")
```

---

## Paso 5: Leer y escribir archivos con `pathlib`

```python
archivo = Path('archivo.txt')

# Escribir texto
archivo.write_text("Hola desde pathlib!")

# Leer texto
contenido = archivo.read_text()
print(contenido)
```

---

## Resumen

1. Usa `Path` para trabajar con rutas y archivos.
2. Manipula, crea y lee archivos de forma sencilla y multiplataforma.

---