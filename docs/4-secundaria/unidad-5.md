# 4-Secundaria - Unidad 5

## 3BS01: Creo la interfaz de mi videojuego

> <i class="bi bi-calendar"></i> **Fecha:** 12 al 16 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** CT.JS<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea<br> <i class="bi bi-card-checklist"></i> **Guía:**  <br><i class="bi bi-youtube txt-red"></i> **Videos:** <br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1fLZleIbpRRpYFXfkKEfqo0nErd5gU_cZ?usp=sharing

El HUD (Heads-Up Display) es una parte esencial de cualquier videojuego moderno. Proporciona a los jugadores información vital, como la salud del personaje, la puntuación, el tiempo restante, entre otros datos importantes. En este tutorial, aprenderemos cómo implementar un HUD en nuestro videojuego utilizando Cat.js, una potente y versátil librería de JavaScript diseñada para facilitar el desarrollo de videojuegos.

Para crear nuestro HUD necesitaremos tres cosas:

- **HUD ROOM**: El room con todos los elementos del HUD, como cantidad de vida, monedas, flechas, poderes, etc.
- **WELCOME ROOM**: La pantalla de bienvenida con el botón start para abrir los otros ROOM. <code>rooms.switch("Nombre del room al que se desea ir")</code>.
- **LEVEL ROOM**: Son los ROOM al que se le añadira el room del HUD con el código <code>rooms.append("Nombre del HUD")</code>. Desde el botón EVENTOS al costado del ojo.

## 3BS02: Trabajo con fondos usando Tiles

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** CT.JS<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea<br> <i class="bi bi-card-checklist"></i> **Guía:**  <br><i class="bi bi-youtube txt-red"></i> **Videos:** <br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1fLZleIbpRRpYFXfkKEfqo0nErd5gU_cZ?usp=sharing

En el desarrollo de videojuegos, uno de los desafíos más importantes es la creación de entornos visuales que sean tanto atractivos como funcionales. Los "tiles" (o baldosas) son una solución popular para este problema, ya que permiten construir mundos de juego de manera modular y eficiente. En este tutorial, exploraremos cómo utilizar cat.js para gestionar y mostrar tiles en tus proyectos de videojuegos.

## 3BS03: Añadiendo sistema de puntajes

> <i class="bi bi-calendar"></i> **Fecha:** 26 al 30 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** CT.JS<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea<br> <i class="bi bi-card-checklist"></i> **Guía:** https://ulisesfreitas.itch.io/ctjs-cheatsheet-spanish-es<br><i class="bi bi-youtube txt-red"></i> **Videos:** <br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1fLZleIbpRRpYFXfkKEfqo0nErd5gU_cZ?usp=sharing

El Local Storage es una herramienta poderosa y sencilla en el desarrollo web que permite a los desarrolladores guardar datos de manera persistente en el navegador del usuario. En el contexto de los videojuegos, Local Storage es especialmente útil para almacenar puntajes, configuraciones o cualquier tipo de información que se desee mantener entre sesiones, sin necesidad de configurar una base de datos en un servidor.

A diferencia de las cookies, Local Storage ofrece más capacidad de almacenamiento (alrededor de 5MB por dominio en la mayoría de los navegadores) y es más fácil de usar para datos no sensibles. Además, los datos almacenados en Local Storage persisten incluso cuando el usuario cierra el navegador, lo que significa que los puntajes de los videojuegos se pueden conservar y cargar la próxima vez que el jugador regrese al juego.

## 3BS04: Usando emiters para añadir efectos

> <i class="bi bi-calendar"></i> **Fecha:** 26 al 30 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** CT.JS<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea. Relizar práctica<br> <i class="bi bi-card-checklist"></i> **Guía:** https://img.itch.zone/aW1hZ2UvODEzOTYxLzE0OTkyMTE1LnBuZw==/original/tfoEIH.png<br><i class="bi bi-youtube txt-red"></i> **Videos:** <br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1fLZleIbpRRpYFXfkKEfqo0nErd5gU_cZ?usp=sharing

Imagina un fuego de campamento, una explosión estelar o una cascada de agua. Todos estos efectos, por complejos que parezcan, pueden ser creados en un videojuego utilizando emisores de partículas. Un emisor de partículas es una herramienta que permite generar y controlar una gran cantidad de pequeñas partículas gráficas para simular diversos fenómenos naturales o efectos mágicos.

En cat.js podemos crearlos a partir de una textura y cuando este listo agregamos el siguiente código a nuestro personaje si queremos que el emisor lo siga.

```javascript
emitters.append(this,"nombreEfecto");
```

## 3BS05: Práctica Calificada & Revisión de Folder

> <i class="bi bi-calendar"></i> **Fecha:** Semana 6<br><i class="bi bi-laptop"></i> **Programa:** CT JS

Para esta semana deberás realizar tu práctica calificada que consiste en lo siguiente:

- Crea un juego de tipo parkour con 3 niveles y una pantalla de bienvenida con su respectivo boton de inicio.
- En la pantalla de Bienvenida coloca el titulo del juego "El desafio de <<tunombre>>" y reemplaza la útlima palabra con tu nombre.
- Plus: Añade un sistema de puntajes.

Guarda tu proyecto en USB y lo presentarás en clase, en la semana 6.





