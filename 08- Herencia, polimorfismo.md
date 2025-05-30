# Curso Básico de Python: Herencia y Polimorfismo

## 1. Introducción

En este curso aprenderás dos conceptos fundamentales de la programación orientada a objetos en Python: **herencia** y **polimorfismo**. Estos conceptos te permitirán reutilizar código y hacer tus programas más flexibles y escalables.

---

## 2. Herencia

La **herencia** permite crear una nueva clase utilizando las características de una clase existente.

### Ejemplo Básico

```python
# Clase base o padre
class Animal:
    def __init__(self, nombre):
        self.nombre = nombre

    def hablar(self):
        print("El animal hace un sonido.")

# Clase hija que hereda de Animal
class Perro(Animal):
    def hablar(self):
        print(f"{self.nombre} dice: ¡Guau!")

# Clase hija que hereda de Animal
class Gato(Animal):
    def hablar(self):
        print(f"{self.nombre} dice: ¡Miau!")

# Uso de las clases
mi_perro = Perro("Rex")
mi_gato = Gato("Luna")

mi_perro.hablar()  # Output: Rex dice: ¡Guau!
mi_gato.hablar()   # Output: Luna dice: ¡Miau!
```

**¿Qué está pasando?**
- `Perro` y `Gato` heredan de `Animal`.
- Ambas redefinen el método `hablar()`.

---

## 3. Polimorfismo

El **polimorfismo** permite que diferentes clases respondan de distinta manera a un mismo método o mensaje.

### Ejemplo de Polimorfismo

```python
animales = [Perro("Rex"), Gato("Luna")]

for animal in animales:
    animal.hablar()
```
**Output:**
```
Rex dice: ¡Guau!
Luna dice: ¡Miau!
```

**¿Qué está pasando?**
- Aunque `animales` contiene objetos de diferentes clases (`Perro` y `Gato`), ambos pueden llamarse con el método `hablar()`.
- Python llama al método correspondiente según la clase del objeto.

---

## 4. Resumen

| Concepto     | ¿Qué es?                                                   | Ejemplo                   |
|--------------|------------------------------------------------------------|---------------------------|
| Herencia     | Una clase hereda atributos y métodos de otra clase         | `Perro(Animal)`           |
| Polimorfismo | Objetos diferentes pueden compartir métodos con diferentes implementaciones | `animal.hablar()`         |

---

## 5. Ejercicio Propuesto

Crea una clase `Ave` que herede de `Animal` y sobrescribe el método `hablar` para que diga "Pío".

```python
class Ave(Animal):
    def hablar(self):
        print(f"{self.nombre} dice: ¡Pío!")
```

¡Ahora prueba crear una lista con instancias de `Perro`, `Gato` y `Ave` y recórrela usando polimorfismo!

---

¿Listo para seguir aprendiendo? Continúa con clases abstractas y métodos especiales (`__str__`, `__repr__`, etc.).