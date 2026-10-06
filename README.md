# 🎨 Triqui del Color

Desarrollo de un juego de **triqui** (tres en línea) con interfaz gráfica y una dinámica especial: antes de cada jugada, el jugador debe **adivinar un color secreto**.

## ¿De qué se trata?

El triqui clásico se juega en un tablero de 3×3 donde dos jugadores (X y O) se turnan para marcar casillas. Gana quien primero completa una línea de tres (horizontal, vertical o diagonal). En esta versión, tener el turno no basta: hay que ganárselo adivinando el color.

## Reglas del juego

1. Al inicio de cada turno el juego elige al azar un **color secreto**: rojo, azul, verde o amarillo.
2. El jugador en turno elige el color que cree que es.
   - **Acierta:** puede marcar la casilla que quiera.
   - **Falla:** se revela el color y **pierde el turno**.
3. Gana quien complete tres en línea. Si el tablero se llena sin ganador, es empate.
4. **Solo se juega una ronda.** Al terminar, no se puede iniciar un nuevo juego.

## Modos de juego

- **Jugador vs Jugador:** dos personas en el mismo equipo.
- **Jugador vs Computador:** el computador adivina colores al azar y, cuando acierta, juega con una estrategia sencilla: gana si puede, bloquea al rival, y si no toma el centro o una esquina.

## Cómo ejecutarlo

No requiere instalación ni dependencias. Abre el archivo `triqui.html` en cualquier navegador moderno (doble clic, o arrastrándolo al navegador).

## Tecnologías

- HTML, CSS y JavaScript en un único archivo (`triqui.html`).
- Python (`generar_readme.py`) para generar este README.

## Estructura del proyecto

```
Triqui/
├── triqui.html         # Juego completo (interfaz y lógica)
├── generar_readme.py   # Script que genera este README
└── README.md           # Este documento
```

## Limitaciones conocidas

- La restricción de una sola ronda se mantiene mientras la página esté abierta; al recargar el navegador se puede jugar de nuevo.
