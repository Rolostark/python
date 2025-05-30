# Curso de Python: APIs con Requests y FastAPI

Aprende a consumir y crear APIs en Python.

---

## Paso 1: Consumir APIs con `requests`

```python
import requests

respuesta = requests.get('https://api.agify.io?name=ana')
if respuesta.status_code == 200:
    datos = respuesta.json()
    print(datos)
```

---

## Paso 2: Crear una API básica con FastAPI

1. Instala FastAPI y Uvicorn:

```bash
pip install fastapi uvicorn
```

2. Crea el archivo `main.py`:

```python
from fastapi import FastAPI

app = FastAPI()

@app.get("/")
def leer_raiz():
    return {"mensaje": "Hola, mundo!"}
```

3. Ejecuta el servidor:

```bash
uvicorn main:app --reload
```

Abre http://127.0.0.1:8000/ en tu navegador.

---

## Resumen

- Usa `requests` para consumir APIs fácilmente.
- Usa `FastAPI` para crear APIs rápidas y modernas.

---