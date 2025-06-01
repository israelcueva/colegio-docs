# 4-Secundaria - Unidad 3

## 2BS01: Añado funcionalidad de movimiento a mi personaje :id=ctjs-movimiento-a-mi-personaje

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Mayo<br><i class="bi bi-window-desktop"></i> **Programa:** [ct.js](https://ctjs.rocks/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Ver al final<br><i class="bi bi-files"></i> **Cheatsheet:** [Enlace](https://comigo.itch.io/ct-cheat-sheet)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing)

El sistema de movimiento en cat.js lo podemos separar en:

### 1. Background

Primero debemos generar el room donde irá el fondo para nuestro nivel.

1. Insertamos la textura de fondo de la galeria.
2. Activamos la opción <span class="badge badge-secondary"> This is a tiled background?</span> o <span class="badge badge-secondary">¿Usar como fondo?</span> y aplicamos.
3. Creamos un <span class="badge badge-secondary"> Room</span> y le ponemos un nombre <span class="badge badge-secondary"> level_1</span> o similar.
4. Agregamos el fondo usando el botón <span class="badge badge-outline"><i class="bi bi-search icon"></i> Find a tileset</span> o <span class="badge badge-outline"><i class="bi bi-search icon"></i> Encontrar un tileset</span> desde el menú <span class="badge badge-outline">Add tiles</span>.
5. Añadimos una capa con <span class="badge badge-outline">Add a tile layer</span> y le ponemos un número, por ejemplo `0`.
6. En el <span class="badge badge-secondary">Collision Group</span> le ponemos el valor: `Suelo`.

### 2. Agregar acciones

Ahora debemos añadir las acciones que usará nuestro personaje para responder al uso de teclas especiales.

1. Nos vamos a <span class="badge badge-primary"><i class="bi bi-sliders2-vertical icon"></i> Proyecto</span>
2. Luego buscamos la opción: <span class="badge badge-outline"><i class="bi bi-share icon"></i> Catmods</span>
3. Allí vereficamos que ***Keyboard Polyfill*** este activado ✅
4. Ahora nos dirigimos a la opción: <span class="badge badge-outline"><i class="bi bi-cast icon"></i> Acciones y métodos de entrada</span>
5. Agregamos las acciones siguientes:

|**Nombre**      |**Teclas**         |
|----------------|-------------------|
| moverIzquierda | A, ArrowLeft      |
| moverDerecha   | D, ArrowRight     |
| Saltar         | W, Space, ArrowUp |


### 3. El personaje

Debemos añadir el template del personaje que contendrá las físicas del movimiento y agregar los siguientes códigos en los eventos correspondientes:

<span class="badge badge-outline"><i class="bi bi-chevron-bar-left icon"></i> Frame start</span>

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

<span class="badge badge-outline"><i class="bi bi-sun icon"></i> Creation</span>

```javascript
this.jumpSpeed = -600;
this.gravity = 1800;

this.hspeed = 0;
this.vspeed = 0;
```

### Tarea

Revisa el cheatsheet que corresponde a movimiento y añade el código necesario para que si el personaje choca con un enemigo, el juego se dé por pérdido (Cambiar room).

## 2BS02: Entiendo los templates para cada estado de mi personaje :id=ctjs-template-personaje

> <i class="bi bi-calendar"></i> **Fecha:** 26 al 30 de Mayo<br><i class="bi bi-window-desktop"></i> **Programa:** [ct.js](https://ctjs.rocks/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Sin tarea<br><i class="bi bi-files"></i> **Cheatsheet:** [Enlace](https://comigo.itch.io/ct-cheat-sheet)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing)

En un videojuego, las animaciones de personaje son esenciales para transmitir fluidez, realismo y personalidad en cada acción que realiza. Cada estado del personaje —como estar quieto, caminar, correr, saltar, atacar o recibir daño— requiere su propia animación específica para reflejar correctamente el comportamiento y la intención en pantalla. Estas animaciones no solo mejoran la estética visual, sino que también aportan información clave al jugador sobre el estado del personaje y su entorno. Un buen diseño de animaciones por estado asegura una experiencia de juego más inmersiva, coherente y dinámica.

Para poder añadir las animaciones debemos agregar un template para cada estado: Reposo, caminando y saltando. El Reposo será la animación por defecto, mientras que caminando y saltando se activaran si usamos las acciones de teclado.

<span class="badge badge-outline"><i class="bi bi-chevron-bar-left icon"></i> Frame start</span>

```javascript
this.movespeed = 240; 

if (actions.moverIzquierda.down) {
    this.hspeed = -this.movespeed;

    // Añadimos la animación de caminar al presionar flecha izquierda
    if (this.tex !== 'personaje_caminar') {
        this.tex = 'personaje_caminar';
        this.play();
    }
    this.scale.x = -1;

} else if (actions.moverDerecha.down) {
    this.hspeed = this.movespeed;

    // Añadimos la animación de caminar al presionar flecha derecha
    if (this.tex !== 'personaje_caminar') {
        this.tex = 'personaje_caminar';
        this.play();
    }
    this.scale.x = 1;

} else {
    this.hspeed = 0;

    // Si no va a la derecha o izquierda la animación por defecto es
     this.tex = 'personaje_reposo';
}

if (place.occupied(this, this.x, this.y + 1, 'Suelo')) {
    if (actions.Saltar.down) {
        this.vspeed = this.jumpSpeed;
    } else {
        this.vspeed = 0;
    }
}
// Agregamos el else para que cuando este en el aire se muestre el template correcto.
else{
    this.tex = 'personaje_saltar';
}

this.moveSmart('Suelo');
```

<div class="currentTheme">

## 2BS03: Creo un sistema de puntajes para mi videojuego :id=ctjs-sistema-puntajes

> <i class="bi bi-calendar"></i> **Fecha:** 02 al 06 de Junio<br><i class="bi bi-window-desktop"></i> **Programa:** [ct.js](https://ctjs.rocks/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Ver al final<br><i class="bi bi-files"></i> **Cheatsheet:** [Enlace](https://comigo.itch.io/ct-cheat-sheet)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing)

En CAT JS no hay un sistema de puntajes de por si, pero podemos generar uno usando textos.

Pasos:

1. Nos vamos a <span class="badge badge-outline-green"><i class="bi bi-plus-lg icon"></i> New Asset</span> y escogemos uno de tipo <span class="badge badge-outline">Style</span> y escoge las propiedades que tu desees.
2. Crea un template y cambia el tipo a <span class="badge badge-outline"><i class="bi bi-fonts icon"></i> Text</span> y en su **default text** coloca `0`.
3. Dale clic en seleccionar y escoge el estilo creado en el primer paso. Aplica los cambios.
4. Crea una nueva acción de <span class="badge badge-outline"><i class="bi bi-cast icon"></i> Acciones y métodos de entrada</span> en <span class="badge badge-primary"><i class="bi bi-sliders2-vertical icon"></i> Proyecto</span>. Ponle el nombre que desees y asocialo a <span class="badge badge-photoshop"><i class="bi bi-arrow-up icon"></i></span> (ArrowUp).
5. Regresa al template del texto y crea un evento de tipo <span class="badge badge-outline"><i class="bi bi-cast icon"></i>Action press</span>.
6. Escribe el siguiente código:

```javascript
this.text = parseInt(this.text)+1;
```

7. Crea un **room** y agrega el template del texto.

### Tarea

- Escribe y explica los tipos de <span class="badge badge-outline-green"><i class="bi bi-plus-lg icon"></i> New Asset</span> que podemos agregar a nuestro proyecto.
- Escribe y explica los tipos de <span class="badge badge-outline"><i class="bi bi-robot icon"></i> Templates</span> que podemos escoger.

Hazlo todo en una sola hoja y adjuntalo en el folder.

</div>
