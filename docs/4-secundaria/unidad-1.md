# 3-Secundaria - Unidad 1

## 1BS01: Creo mis propios algoritmos usando variables en Javascript

> <i class="bi bi-calendar"></i> **Fecha:** 03 al 07 de Marzo<br><i class="bi bi-laptop"></i> **Programa:** Cualquier editor de código <br><i class="bi bi-clipboard-check"></i> **Tarea:** Busca e imprime un cheatsheet de Javascript <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=8GTaO9XhA5M<br> <i class="bi bi-backpack"></i> **Recursos:** https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing / https://htmlcheatsheet.com/js/

En **JavaScript**, las variables son contenedores que almacenan datos. Son fundamentales en la programación, ya que nos permiten guardar valores, manipular información y hacer que nuestro código sea dinámico.  

### 📌 ¿Qué es una variable?
Una variable es un espacio en memoria que almacena un valor que puede cambiar durante la ejecución del programa. En JavaScript, podemos declarar variables usando tres palabras clave principales:  

- **`var`** (obsoleta en la mayoría de los casos).  
- **`let`** (recomendada para valores que pueden cambiar).  
- **`const`** (para valores que no deben cambiar).  

### 🔹 Declaración de variables  

En JavaScript, podemos declarar una variable de la siguiente manera:  

```javascript
let nombre = "Juan"; // Variable que puede cambiar
const PI = 3.1416;   // Constante, su valor no puede cambiar
var edad = 25;       // Forma antigua de declarar variables (no recomendada)
```
## 1BS02: Uso funciones y estructuras de control para un juego simple

> <i class="bi bi-calendar"></i> **Fecha:** 10 al 14 de Marzo<br><i class="bi bi-laptop"></i> **Programa:** Cualquier editor de código <br><i class="bi bi-clipboard-check"></i> **Tarea:** No aplica <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=8GTaO9XhA5M<br> <i class="bi bi-backpack"></i> **Recursos:** https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing / https://htmlcheatsheet.com/js/

### Funciones en Javascript

Las funciones son bloques de código reutilizables que ejecutan una tarea específica. Permiten mejorar la legibilidad del código, evitar la repetición y hacer que sea más modular.  

#### ✨ Declaración de Funciones  

Existen varias formas de definir funciones en JavaScript:  

##### 1️⃣ Función Tradicional  

```javascript
function saludar(nombre) {
    return `Hola, ${nombre}!`;
}
console.log(saludar("Juan")); // Salida: Hola, Juan!
```

##### 2️⃣ Función Anónima

```javascript
const despedir = function(nombre) {
    return `Adiós, ${nombre}!`;
};
console.log(despedir("María")); // Salida: Adiós, María!
```
##### 3️⃣ Función de Flecha (Arrow Function)

```javascript
const sumar = (a, b) => a + b;
console.log(sumar(3, 7)); // Salida: 10
```

##### 4️⃣ Función con Valores por Defecto

```javascript
function presentar(nombre = "Invitado") {
    return `Bienvenido, ${nombre}!`;
}
console.log(presentar()); // Salida: Bienvenido, Invitado!
```

### Estructuras de control

Las estructuras de control permiten ejecutar diferentes bloques de código dependiendo de condiciones específicas o repetir acciones varias veces.

#### 🏷️ Condicionales

##### 🔸 if, else if, else

```javascript
let edad = 18;

if (edad < 18) {
    console.log("Eres menor de edad.");
} else if (edad === 18) {
    console.log("Tienes exactamente 18 años.");
} else {
    console.log("Eres mayor de edad.");
}
```

##### 🔸 Operador Ternario

```javascript
let mensaje = edad >= 18 ? "Mayor de edad" : "Menor de edad";
console.log(mensaje);
```

##### 🔸 switch (Alternativa a múltiples if-else)

```javascript
let dia = "lunes";

switch (dia) {
    case "lunes":
        console.log("Inicio de la semana.");
        break;
    case "viernes":
        console.log("Casi fin de semana.");
        break;
    default:
        console.log("Es un día cualquiera.");
}
```
### 🔁 Bucles

Los bucles permiten ejecutar un bloque de código varias veces de manera eficiente.

##### 🔸 Bucle for (Iteración controlada)

```javascript
for (let i = 0; i < 5; i++) {
    console.log(`Iteración ${i}`);
}
```

##### 🔸 Bucle while (Se ejecuta mientras la condición sea true)

```javascript
let contador = 0;
while (contador < 5) {
    console.log(`Contador: ${contador}`);
    contador++;
}
```

##### 🔸 Bucle do-while (Se ejecuta al menos una vez)

```javascript
let num = 0;
do {
    console.log(`Número: ${num}`);
    num++;
} while (num < 3);
```

<div class="currentTheme">

## 1BS03: Hago uso de eventos para manejar el DOM

> <i class="bi bi-calendar"></i> **Fecha:** 17 al 21 de Marzo<br><i class="bi bi-laptop"></i> **Programa:** Cualquier editor de código <br><i class="bi bi-clipboard-check"></i> **Tarea:** No aplica <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=8GTaO9XhA5M<br> <i class="bi bi-backpack"></i> **Recursos:** https://drive.google.com/drive/folders/19UQ_kuY8V0xU3Kd8aMDtbcXS7qQDOJ98?usp=sharing / https://htmlcheatsheet.com/js/

JavaScript es un lenguaje que permite interactuar con las páginas web de manera dinámica a través del **DOM (Document Object Model)** y el uso de **eventos**. Gracias a estas características, podemos modificar elementos, responder a interacciones del usuario y crear experiencias web interactivas.  

### 🔹 ¿Qué es el DOM?  

El **DOM (Modelo de Objetos del Documento)** es una representación estructurada de una página web. Cada elemento HTML se convierte en un nodo dentro de este modelo, permitiendo que JavaScript acceda y modifique su contenido, estructura y estilos.  

#### 📄 Ejemplo de Estructura del DOM  

Si tenemos este código HTML:  

```html
<!DOCTYPE html>
<html lang="es">
<head>
    <title>Ejemplo DOM</title>
</head>
<body>
    <h1 id="titulo">¡Hola, mundo!</h1>
    <button id="boton">Haz clic</button>
</body>
</html>
```

Podemos acceder y modificar estos elementos con JavaScript:

```javascript
let titulo = document.getElementById("titulo");
titulo.textContent = "¡Bienvenido a JavaScript!";
```

#### 🔹 Selección de Elementos en el DOM

Para manipular el DOM, primero debemos seleccionar los elementos. Hay varias formas de hacerlo en JavaScript:

##### 🔸 getElementById() (Por ID)

```javascript
let elemento = document.getElementById("titulo");
console.log(elemento.textContent);
```

##### 🔸 getElementsByClassName() (Por clase)

```javascript
let elementos = document.getElementsByClassName("clase-ejemplo");
console.log(elementos[0]);
```
##### 🔸 getElementsByTagName() (Por etiqueta)

```javascript
let parrafos = document.getElementsByTagName("p");
console.log(parrafos.length);
```

##### 🔸 querySelector() (Primer elemento que coincide con un selector CSS)

```javascript
let boton = document.querySelector("#boton");
console.log(boton);
```

##### 🔸 querySelectorAll() (Todos los elementos que coinciden con un selector CSS)

```javascript
let items = document.querySelectorAll(".lista-item");
console.log(items);
```
---

### 🔹 Eventos en JavaScript

Los eventos permiten detectar e interactuar con acciones del usuario, como clics, movimientos del mouse y pulsaciones del teclado.

#### 📌 Manejo de Eventos

##### 🔸 1. Usando el atributo HTML onclick (No recomendado)

```javascript
<button onclick="alert('¡Hola!')">Haz clic</button>
```

##### 🔸 2. Usando addEventListener() (Recomendado)

```javascript
let boton = document.getElementById("boton");
boton.addEventListener("click", function() {
    alert("¡Botón clickeado!");
});
```

##### 🔸 3. Usando una función externa

```javascript
function mostrarMensaje() {
    alert("¡Evento activado!");
}
boton.addEventListener("click", mostrarMensaje);
```

#### 🔹 Tipos de Eventos en JavaScript

Algunos de los eventos más utilizados en JavaScript son:

| **Evento**   | **Descripción** |
|-------------|---------------|
| `click`     | Se activa cuando el usuario hace clic en un elemento. |
| `mouseover` | Se activa cuando el mouse pasa sobre un elemento. |
| `mouseout`  | Se activa cuando el mouse sale de un elemento. |
| `keydown`   | Se activa cuando se presiona una tecla. |
| `keyup`     | Se activa cuando se suelta una tecla. |
| `load`      | Se activa cuando la página ha terminado de cargar. |
| `submit`    | Se activa cuando un formulario es enviado. |

##### Ejemplo: Cambiar el color de un elemento al pasar el mouse

```javascript
let titulo = document.getElementById("titulo");

titulo.addEventListener("mouseover", function() {
    titulo.style.color = "red";
});
titulo.addEventListener("mouseout", function() {
    titulo.style.color = "black";
});
```

</div>