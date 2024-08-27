# 3-Secundaria - Unidad 5

## 3BS01: Creo mis primeras líneas de código

> <i class="bi bi-calendar"></i> **Fecha:** 12 al 16 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Por designar<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/js/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=QoC4RxNIs5M<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

JavaScript es un lenguaje de programación interpretado, orientado a objetos y basado en prototipos. A diferencia de otros lenguajes que requieren compilación, JavaScript se ejecuta directamente en el navegador web del usuario, lo que lo convierte en una herramienta esencial para la creación de sitios web interactivos.

## 3BS02: Reconozco el DOM y su estructura

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Por designar<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/js/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=koiPxFFiqJ4<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

El Document Object Model (DOM) es una interfaz de programación para documentos HTML y XML. Proporciona una representación estructural del documento, permitiendo a los lenguajes de programación manipular su contenido, estructura y estilo. JavaScript, siendo el lenguaje de scripting más utilizado en la web, ofrece una amplia gama de métodos y propiedades para interactuar con el DOM de manera eficiente.

![Alt text](https://miro.medium.com/v2/resize:fit:1358/0*XuuvP2Fzjm5-EXTd "a title")

<div class="currentTheme">

## 3BS03: Uso bucles y condicionales para juegos simples

> <i class="bi bi-calendar"></i> **Fecha:** 26 al 30 de Agosto<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Por designar<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/js/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=XYs3nHEKfeY / https://www.youtube.com/watch?v=7bO5wlqeeEI<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

En la programación, los bucles y las estructuras condicionales son fundamentales para controlar el flujo de un programa. En JavaScript, estas herramientas permiten realizar tareas repetitivas y tomar decisiones basadas en condiciones específicas.

### Bucles en JavaScript

Un bucle es una estructura que permite repetir una serie de instrucciones varias veces. Los bucles son útiles cuando necesitas ejecutar un bloque de código varias veces, como recorrer una lista de elementos o repetir una acción hasta que se cumpla una condición. JavaScript ofrece varios tipos de bucles, entre los más comunes están:

- `for`: Este bucle se utiliza cuando conoces de antemano cuántas veces necesitas repetir el bloque de código.

  ```javascript
  for (let i = 0; i < 5; i++) {
      console.log(i);  // Imprime los números del 0 al 4
  }
  ```
- `while`: Este bucle repite el bloque de código mientras la condición especificada sea verdadera.

  ```javascript
    let i = 0;
    while (i < 5) {
        console.log(i);  // Imprime los números del 0 al 4
        i++;
    }
  ```

- `do...while`: Similar al bucle `while`, pero en este caso el bloque de código se ejecuta al menos una vez antes de verificar la condición.

  ```javascript
  let i = 0;
    do {
        console.log(i);  // Imprime los números del 0 al 4
        i++;
    } while (i < 5);
  ```

### Condicionales en JavaScript

Las estructuras condicionales permiten que un programa tome decisiones en función de condiciones específicas. Estas estructuras evalúan expresiones booleanas (verdadero o falso) y ejecutan bloques de código en consecuencia. Los principales tipos de condicionales en JavaScript son:

- `if...else`: Evalúa una condición y ejecuta un bloque de código si la condición es verdadera. Si la condición es falsa, se puede ejecutar otro bloque de código con else.

  ```javascript
  let edad = 18;
    if (edad >= 18) {
        console.log("Eres mayor de edad");
    } else {
        console.log("Eres menor de edad");
    }
  ```

- `else if`: Se utiliza cuando necesitas evaluar múltiples condiciones.

  ```javascript
  let nota = 85;
    if (nota >= 90) {
        console.log("Excelente");
    } else if (nota >= 70) {
        console.log("Aprobado");
    } else {
        console.log("Reprobado");
    }
  ```

- `switch`: Es útil cuando tienes múltiples opciones posibles para una misma variable. Es una alternativa al uso de múltiples `if...else if`.

  ```javascript
  let dia = 3;
    switch (dia) {
        case 1:
            console.log("Lunes");
            break;
        case 2:
            console.log("Martes");
            break;
        case 3:
            console.log("Miércoles");
            break;
        default:
            console.log("Día no válido");
    }
  ```

### Ejemplos

#### Numeros Pares

   ```javascript
    for (let i = 1; i <= 10; i++) {
        if (i % 2 === 0) {
            console.log(i + " es par");
        } else {
            console.log(i + " es impar");
        }
    }
  ```
#### Imprimir números del 1 al 20, pero solo los múltiplos de 3

   ```javascript
    for (let i = 1; i <= 20; i++) {
        if (i % 3 === 0) {
            console.log(i);
        }
    }
  ```

#### Sumar los números impares del 1 al 50

   ```javascript
    let sum = 0;
    for (let i = 1; i <= 50; i++) {
        if (i % 2 !== 0) {
            sum += i;
        }
    }
    console.log("La suma de los números impares es:", sum);
  ```

#### Encontrar el primer número divisible por 5 en un arreglo

   ```javascript
    let numeros = [12, 18, 21, 7, 9, 25, 14, 30];
    for (let i = 0; i < numeros.length; i++) {
        if (numeros[i] % 5 === 0) {
            console.log("El primer número divisible por 5 es:", numeros[i]);
            break;
        }
    }
  ```

</div>