# Curso de Python: Async/Await con `asyncio`

Ejecuta tareas asíncronas y concurrentes de forma sencilla.

---

## Paso 1: Definir funciones asíncronas

```python
import asyncio

async def saludar(nombre):
    await asyncio.sleep(1)
    print(f"Hola, {nombre}")
```

---

## Paso 2: Ejecutar funciones asíncronas

```python
async def main():
    await saludar("Ana")
    await saludar("Luis")

asyncio.run(main())
```

---

## Paso 3: Ejecutar varias tareas en paralelo

```python
async def main():
    tarea1 = asyncio.create_task(saludar("Ana"))
    tarea2 = asyncio.create_task(saludar("Luis"))
    await tarea1
    await tarea2

asyncio.run(main())
```

---

## Resumen

- Usa `async def` y `await` para definir y llamar funciones asíncronas.
- Usa `asyncio.run()` para ejecutar el bucle de eventos.

---