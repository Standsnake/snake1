# snake1 - snake

# Actividad 2
# Juego Snake

> Este proyecto es una copia de Sna## Funcionalidades Base
**Mecánicas y Controles:**
- Controlar la serpiente mediante las teclas de dirección (`Up`, `Down`, `Left`, `Right`).
- Comer la fruta verde para aumentar la longitud de la serpiente y sumar puntos.
- El juego termina si la serpiente choca contra los bordes o contra su propio cuerpo.

## Funcionalidades agregadas
- La comida ahora se mueve aleatoriamente un paso a la vez en cada turno sin salirse de la ventana.

## Cambios en el código
- Se importó `choice` del módulo `random` para seleccionar una dirección al azar (`vector(10, 0)`, `vector(-10, 0)`, `vector(0, 10)`, `vector(0, -10)`).
- Se implementó la verificación `if inside(food + step): food.move(step)` dentro de la función `move()` para asegurar que la comida no sobrepase los límites de la ventana antes de moverse.

## Requisitos e Instalación
1. Asegurarse de tener Python 3 instalado.
2. Instalar la librería requerida:
```bash
pip install freegameske en Python utilizando las librerías `turtle` y `freegames`.

## Funcionalidades Base
**Movimiento y Controles:**
- Controlar la serpiente mediante las teclas de dirección (Arriba, Abajo, Izquierda, Derecha).
**Mecánica de Juego:**
- Recolectar la comida verde para hacer crecer la serpiente y sumar puntos.
- La partida termina si la serpiente choca contra los bordes de la ventana o contra su propio cuerpo.

## Funcionalidades agregadas
- Se modificó el comportamiento de la comida para que no se quede estática: ahora se mueve aleatoriamente un paso a la vez en cada turno sin salirse de la ventana.

## Cambios en el código
- Se utilizó la función `choice` para seleccionar un vector de movimiento aleatorio (`arriba`, `abajo`, `izquierda`, `derecha`) para la comida en cada turno dentro de `move()`.
- Se implementó la condición `inside(food + step)` antes de aplicar `food.move(step)` para verificar que la nueva posición no sobrepase los límites del tablero.
- Se usó `randint` para reubicar la comida en un punto aleatorio dentro de la cuadrícula cada vez que la serpiente la consume.

## Requisitos e Instalación
1. Asegurarse de tener Python 3 instalado.
2. Instalar la librería requerida:
```bash
pip install freegames
