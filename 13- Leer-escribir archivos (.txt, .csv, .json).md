# Curso de Python: Leer/Escribir Archivos (.txt, .csv, .json)

Aprende a manejar archivos de texto, CSV y JSON en Python.

---

## Paso 1: Leer y escribir archivos de texto (.txt)

```python
# Escribir en un archivo
with open('archivo.txt', 'w') as f:
    f.write("Hola, mundo!\nLínea 2.")

# Leer el archivo
with open('archivo.txt', 'r') as f:
    contenido = f.read()
    print(contenido)
```

---

## Paso 2: Leer y escribir archivos CSV

```python
import csv

# Escribir en un archivo CSV
with open('datos.csv', 'w', newline='') as f:
    writer = csv.writer(f)
    writer.writerow(['Nombre', 'Edad'])
    writer.writerow(['Ana', 25])
    writer.writerow(['Luis', 30])

# Leer el archivo CSV
with open('datos.csv', 'r') as f:
    reader = csv.reader(f)
    for fila in reader:
        print(fila)
```

---

## Paso 3: Leer y escribir archivos JSON

```python
import json

# Escribir en un archivo JSON
datos = {"nombre": "Ana", "edad": 25}
with open('datos.json', 'w') as f:
    json.dump(datos, f)

# Leer el archivo JSON
with open('datos.json', 'r') as f:
    datos_leidos = json.load(f)
    print(datos_leidos)
```

---

## Resumen

1. Los archivos `.txt` se manipulan con `open()`.
2. Los archivos `.csv` se gestionan con el módulo `csv`.
3. Los archivos `.json` se leen y escriben con el módulo `json`.

---