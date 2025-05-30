# Curso de Python: Visualización con Matplotlib y Seaborn

Crea gráficos y visualizaciones de datos fácilmente.

---

## Paso 1: Gráficos básicos con Matplotlib

```python
import matplotlib.pyplot as plt

x = [1, 2, 3, 4]
y = [10, 20, 25, 30]

plt.plot(x, y)
plt.title("Gráfico de Línea")
plt.xlabel("Eje X")
plt.ylabel("Eje Y")
plt.show()
```

---

## Paso 2: Visualizaciones avanzadas con Seaborn

```python
import seaborn as sns
import pandas as pd

# Datos de ejemplo
df = pd.DataFrame({'x': [1,2,3,4], 'y': [10,20,25,30], 'categoria': ['A','A','B','B']})

sns.barplot(x='x', y='y', hue='categoria', data=df)
plt.title("Barplot con Seaborn")
plt.show()
```

---

## Resumen

- Usa `matplotlib` para gráficos personalizados.
- Usa `seaborn` para visualizaciones estadísticas y atractivas.

---