# Curso de Python: Depuración con `pdb`

Encuentra y corrige errores paso a paso en tus programas.

---

## Paso 1: Insertar un breakpoint

```python
import pdb

a = 2
b = 3
pdb.set_trace()  # El programa se detendrá aquí
c = a + b
print(c)
```

---

## Paso 2: Comandos básicos de `pdb`

- `n` (next): Ejecuta la siguiente línea.
- `c` (continue): Continúa hasta el siguiente breakpoint.
- `l` (list): Muestra el código fuente.
- `p variable`: Imprime el valor de una variable.
- `q` (quit): Sale del depurador.

---

## Paso 3: Ejecutar un script con pdb desde la terminal

```bash
python -m pdb mi_script.py
```

---

## Resumen

- Usa `pdb` para depurar y analizar el flujo de tu código.
- Inserta `pdb.set_trace()` donde quieras pausar la ejecución.

---