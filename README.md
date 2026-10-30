# Actividad 2
# Juego Snake


> Este proyecto es una copia de snake en Python utilizando las librerías `turtle` y `freegames`.

> Este proyecto es una copia de snake.py Funcionalidades Base
**Mecánicas y Controles:**
- Controlar la serpiente mediante las teclas de dirección (`Up`, `Down`, `Left`, `Right`).
- Comer la fruta verde para aumentar la longitud de la serpiente y sumar puntos.
- El juego termina si la serpiente choca contra los bordes o contra su propio cuerpo.

## Funcionalidades agregadas
- La comida ahora se mueve aleatoriamente un paso a la vez en cada turno sin salirse de la ventana.

## Cambios en el código
- Se genero la funcion def move: [vector(10, 0), vector(-10, 0), vector(0, 10), vector(0, -10)] con estas funcionalidades y un randrange(4) es una funcion nueva
- Se llamo a la funcion antes del clear, moviendo la comida de forma aleatoria

## Requisitos e Instalación
1. Asegurarse de tener Python 3 instalado.
2. Instalar la librería requerida:
```bash
pip install freegames
