# 4-Secundaria - Unidad 3

<div class="currentTheme">

## 2BS01: Añado funcionalidad de movimiento a mi personaje :id=ctjs-movimiento-a-mi-personaje

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Mayo<br><i class="bi bi-window-desktop"></i> **Programa:** [ct.js](https://ctjs.rocks/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Ver al final<br><i class="bi bi-files"></i> **Cheatsheet:** [Enlace](https://comigo.itch.io/ct-cheat-sheet)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing)

El sistema de movimiento en cat.js lo podemos separar en:

### 1. Background

Primero debemos generar el room donde irá el fondo para nuestro nivel.

1. Insertamos la textura de fondo de la galeria.
2. Activamos la opción <span class="badge badge-secondary"> This is a tiled background?</span> o <span class="badge badge-secondary">¿Usar como fondo?</span> y aplicamos.
3. Creamos un <span class="badge badge-secondary"> Room</span> y le ponemos un nombre <span class="badge badge-secondary"> level_1</span> o similar.
4. Agregamos el fondo usando el botón <span class="badge badge-outline"><i class="bi bi-search"></i> Find a tileset</span> o <span class="badge badge-outline"><i class="bi bi-search"></i> Encontrar un tileset</span> desde el menú <span class="badge badge-outline">Add tiles</span>.
5. Añadimos una capa con <span class="badge badge-outline">Add a tile layer</span> y le ponemos un número, por ejemplo `0`.
6. En el <span class="badge badge-secondary">Collision Group</span> le ponemos el valor: `Suelo`.

### 2. Agregar acciones

Ahora debemos añadir las acciones que usará nuestro personaje para responder al uso de teclas especiales.

1. Nos vamos a <span class="badge badge-primary"><i class="bi bi-sliders2-vertical"></i> Proyecto</span>
2. Luego buscamos la opción: <span class="badge badge-outline"><i class="bi bi-share"></i> Catmods</span>
3. Allí vereficamos que ***Keyboard Polyfill*** este activado ✅
4. Ahora nos dirigimos a la opción: <span class="badge badge-outline"><i class="bi bi-cast"></i> Acciones y métodos de entrada</span>
5. Agregamos las acciones siguientes:

|**Nombre**      |**Teclas**         |
|----------------|-------------------|
| moverIzquierda | A, ArrowLeft      |
| moverDerecha   | D, ArrowRight     |
| Saltar         | W, Space, ArrowUp |


### 3. El personaje

Debemos añadir el template del personaje que contendrá las físicas del movimiento y agregar los siguientes códigos en los eventos correspondientes:

<span class="badge badge-outline"><i class="bi bi-chevron-bar-left"></i> Frame start</span>

```javascript
this.movespeed = 240; 

if (actions.moverIzquierda.down) {
    this.hspeed = -this.movespeed;
} else if (actions.moverDerecha.down) {
    this.hspeed = this.movespeed;
} else {
    this.hspeed = 0;
}

if (place.occupied(this, this.x, this.y + 1, 'Suelo')) {
    if (actions.Saltar.down) {
        this.vspeed = this.jumpSpeed;
    } else {
        this.vspeed = 0;
    }
}

this.moveSmart('Suelo');
```

<span class="badge badge-outline"><i class="bi bi-sun"></i> Creation</span>

```javascript
this.jumpSpeed = -600;
this.gravity = 1800;

this.hspeed = 0;
this.vspeed = 0;
```

### Tarea

Revisa el cheatsheet que corresponde a movimiento y añade el código necesario para que si el personaje choca con un enemigo, el juego se dé por pérdido (Cambiar room).

</div>