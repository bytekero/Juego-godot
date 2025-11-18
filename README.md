# 👾 Dodge the Creeps (Tu Primer Juego 2D)

Este proyecto es un juego arcade 2D desarrollado siguiendo la guía oficial de "Tu primer juego 2D" de la documentación de **Godot Engine (4.x)**. El objetivo es mover al personaje para esquivar a los enemigos que aparecen aleatoriamente y sobrevivir el mayor tiempo posible.

## 🎮 Descripción del Juego
El jugador controla un personaje que debe moverse por la pantalla evitando colisionar con los enemigos ("creeps"). Con cada segundo que sobrevives, tu puntuación aumenta. El juego cuenta con un menú de inicio, un contador de puntuación y detección de "Game Over".

## 🛠️ Conceptos Técnicos Aplicados

Este proyecto implementa los pilares fundamentales del desarrollo en Godot:

* **Motor:** Godot Engine 4.x.
* **Lenguaje:** GDScript.
* **Estructura de Escenas:** Uso de composición de escenas (`Player`, `Mob`, `HUD`, `Main`) para organizar el juego de forma modular.
* **Física y Colisiones (`Area2D`):** Detección de impactos entre el jugador y los enemigos sin usar física rígida compleja, optimizando el rendimiento.
* **Señales (Signals):** Implementación del patrón observador para conectar eventos.
    * Ejemplo: Cuando el `Player` detecta un golpe, emite una señal `hit` que avisa al `Main` para detener el juego.
* **Generación Aleatoria (`PathFollow2D`):** Uso de nodos de ruta para hacer aparecer enemigos en posiciones aleatorias alrededor del borde de la pantalla.
* **Interfaz de Usuario (UI):** Control de botones, etiquetas de texto y anclajes mediante `CanvasLayer` y `Control Nodes`.

## 🕹️ Cómo Jugar

1. Dale al botón **Start**.
2. Usa las **Flechas de dirección** (o WASD) para moverte.
3. ¡No toques a los enemigos!

## 🚀 Instalación y Ejecución

Este proyecto requiere Godot Engine para ejecutarse.

1. Descarga e instala **Godot Engine** (versión 4.x) desde su web oficial.
2. Clona este repositorio o descarga los archivos.
3. Abre Godot y selecciona **"Importar"**.
4. Navega hasta la carpeta del proyecto y selecciona el archivo `project.godot`.
5. Presiona **F5** o el botón de "Reproducir" en la esquina superior derecha.

## 📚 Referencia
Basado en el tutorial oficial de la documentación de Godot:
[Tu primer juego 2D - Godot Engine Docs](https://docs.godotengine.org/es/4.x/getting_started/first_2d_game/index.html)

---
**Autor:** Antonio Muñoz
