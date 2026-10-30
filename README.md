# Actividad 2
# Juego Snake
> Este proyecto es una copia de snake en Python utilizando las librerías `turtle` y `freegames`.

## Funcionalidades Base
**Movimiento y Controles:**
- Controlar la serpiente mediante las teclas de dirección (Arriba, Abajo, Izquierda, Derecha).
**Mecánica de Juego:**
- Recolectar la comida para hacer crecer la serpiente y sumar puntos.
- La partida termina si la serpiente choca contra los bordes de la ventana o contra su propio cuerpo.
## Funcionalidades agregadas
- Se modificó el comportamiento de la comida para que no se quede estática: ahora se mueve aleatoriamente un paso a la vez en cada turno sin salirse de la ventana.
- Cada vez que se ejecuta el juego, la serpiente y la comida reciben colores aleatorios de una lista de 5 opciones permitidas, expluyendo al rojo y evitando que compartan el mismo color.

## Cambios en el código
- Se utilizó la función `choice` para seleccionar un vector de movimiento aleatorio (`arriba`, `abajo`, `izquierda`, `derecha`) para la comida en cada turno dentro de `move()`.
- Se implementó la condición `inside(food + step)` antes de aplicar `food.move(step)` para verificar que la nueva posición no sobrepase los límites del tablero.
- Se usó `randint` para reubicar la comida en un punto aleatorio dentro de la cuadrícula cada vez que la serpiente la consume.
- Se creó una lista de `COLORES` con 5 colores permitidos.
- Se utilizó `random.sample(COLORES, 2)` para asignar aleatoriamente un color a `snake_color` y otro a `food_color`.
- Dentro de la función `move()`, se reemplazo el color fijo `'black'` por `snake_color` y el color fijo `'green'` por `food_color`.

## Requisitos e Instalación
1. Asegurarse de tener Python 3 instalado.
2. Instalar la librería requerida:
```bash
pip install freegames
