# Curso de Python: Pruebas Unitarias (`unittest`, `pytest`)

Asegura la calidad de tu código con pruebas automáticas.

---

## Paso 1: Pruebas con `unittest`

```python
import unittest

def sumar(a, b):
    return a + b

class TestSumar(unittest.TestCase):
    def test_suma(self):
        self.assertEqual(sumar(2, 3), 5)

if __name__ == '__main__':
    unittest.main()
```

---

## Paso 2: Pruebas con `pytest`

1. Instala pytest:

```bash
pip install pytest
```

2. Crea un archivo `test_suma.py`:

```python
from suma import sumar

def test_suma():
    assert sumar(2, 3) == 5
```

3. Ejecuta las pruebas:

```bash
pytest
```

---

## Resumen

- Usa `unittest` para pruebas incluidas en la librería estándar.
- Usa `pytest` para una sintaxis más simple y potente.

---