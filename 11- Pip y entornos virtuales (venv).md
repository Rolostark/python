# Curso de Python: Pip y Entornos Virtuales (venv)

En este capítulo aprenderás a gestionar paquetes y dependencias en Python utilizando **pip** y a crear entornos virtuales con **venv** para mantener tus proyectos organizados y aislados.

---

## Paso 1: ¿Qué es pip?

**pip** es el gestor de paquetes por defecto en Python. Permite instalar, actualizar y desinstalar librerías de terceros desde [PyPI (Python Package Index)](https://pypi.org/).

---

## Paso 2: ¿Qué es un entorno virtual?

Un **entorno virtual** es una carpeta que contiene una instalación independiente de Python y sus propias librerías. Esto permite aislar las dependencias de diferentes proyectos para evitar conflictos.

---

## Paso 3: Crear un entorno virtual con venv

1. Abre una terminal.
2. Navega hasta el directorio de tu proyecto.
3. Ejecuta el siguiente comando:

```bash
python -m venv env
```

Esto crea una carpeta llamada `env` (puedes cambiar el nombre) donde estará el entorno virtual.

---

## Paso 4: Activar el entorno virtual

- **En Windows:**

```bash
env\Scripts\activate
```

- **En macOS/Linux:**

```bash
source env/bin/activate
```

Verás que el prompt de tu terminal cambia, mostrando el nombre del entorno (por ejemplo, `(env)`).

---

## Paso 5: Instalar paquetes con pip

Con el entorno virtual activado, puedes instalar paquetes que solo afectarán a este proyecto.

```bash
pip install requests
```

Esto instalará la librería `requests` solo en el entorno virtual.

---

## Paso 6: Listar y guardar dependencias

- **Listar paquetes instalados:**

```bash
pip list
```

- **Guardar dependencias en un archivo:**

```bash
pip freeze > requirements.txt
```

Este archivo puede ser usado para replicar el entorno en otra máquina.

---

## Paso 7: Instalar dependencias desde un archivo

Si tienes un archivo `requirements.txt`, puedes instalar todas las dependencias con:

```bash
pip install -r requirements.txt
```

---

## Paso 8: Desactivar el entorno virtual

Cuando termines de trabajar, puedes salir del entorno virtual con:

```bash
deactivate
```

---

## Resumen

1. Usa `venv` para crear entornos virtuales y aislar proyectos.
2. Activa el entorno antes de trabajar.
3. Instala paquetes con `pip` dentro del entorno.
4. Usa `requirements.txt` para compartir dependencias.
5. Desactiva el entorno al finalizar.

¡Ahora puedes gestionar proyectos Python de manera profesional usando pip y entornos virtuales!

---