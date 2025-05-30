# Curso de Python: Hilos (`threading`) y Multiprocesamiento (`multiprocessing`)

Aprende a ejecutar tareas en paralelo usando hilos y procesos.

---

## Paso 1: Hilos con `threading`

```python
import threading

def tarea(nombre):
    print(f"Hola desde el hilo {nombre}")

# Crear hilos
hilo1 = threading.Thread(target=tarea, args=("A",))
hilo2 = threading.Thread(target=tarea, args=("B",))

# Iniciar hilos
hilo1.start()
hilo2.start()

# Esperar a que terminen
hilo1.join()
hilo2.join()
```

---

## Paso 2: Multiprocesamiento con `multiprocessing`

```python
import multiprocessing

def tarea(nombre):
    print(f"Hola desde el proceso {nombre}")

if __name__ == '__main__':
    proceso1 = multiprocessing.Process(target=tarea, args=("1",))
    proceso2 = multiprocessing.Process(target=tarea, args=("2",))

    proceso1.start()
    proceso2.start()

    proceso1.join()
    proceso2.join()
```

---

## Resumen

- Usa `threading` para tareas ligeras que compartan memoria.
- Usa `multiprocessing` para aprovechar múltiples núcleos y evitar el GIL.

---