# Curso de Python: NumPy y Pandas

Trabaja con datos y realiza análisis numéricos de forma eficiente.

---

## Paso 1: NumPy - Arreglos y operaciones

```python
import numpy as np

# Crear un arreglo
a = np.array([1, 2, 3])
print("Arreglo:", a)

# Operaciones
print("Suma:", a + 2)
print("Media:", np.mean(a))
```

---

## Paso 2: Pandas - DataFrames y manipulación de datos

```python
import pandas as pd

# Crear un DataFrame
datos = {'Nombre': ['Ana', 'Luis'], 'Edad': [25, 30]}
df = pd.DataFrame(datos)
print(df)

# Leer un CSV
# df = pd.read_csv('datos.csv')

# Filtrar datos
print(df[df['Edad'] > 25])
```

---

## Resumen

- Usa `numpy` para cálculos numéricos y arreglos eficientes.
- Usa `pandas` para manipular y analizar datos tabulares.

---