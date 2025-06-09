# 3-Secundaria - Unidad 3

## 2BS01: Instalo Bootstrap en mi página web :id=instalacion-boostrap

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Mayo<br><i class="bi bi-window-desktop"></i> **Programa:** [Visual Studio Code](https://code.visualstudio.com/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Ver al final<br><i class="bi bi-play-btn"></i> **Videos:** [Video 1](https://www.youtube.com/watch?v=WLcAX0KirJ4)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/1sS6GGJK9ZJz4Go2m57zzpjfSGLDMH5jn?usp=sharing)

Puedes agregar Bootstrap 5 a tu proyecto incluyendo los siguientes enlaces en el `<head>` y antes de `</body>` respectivamente.

```html
<!-- CSS de Bootstrap 5  en el head de tu página-->
<link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
```

Con esta otra línea añades el javascript de Boostrap.

```html
<!-- JS de Bootstrap 5. Antes del </body> -->
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
```

Para instalar los iconos de boostrap basta con agregar la siguiente línea de código en el head de tu página.

```html
<!-- Bootstrap Icons -->
<link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.css" rel="stylesheet">
```

#### Ejemplo:

Usa este código para mostrar los estilos básicos de **Boostrap** y sus iconos.

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <meta name="viewport" content="width=device-width, initial-scale=1.0">
  <title>Ejemplo con Bootstrap</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet">
  <link href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.css" rel="stylesheet">
</head>
<body>
  <div class="container text-center mt-5">
    <h1><i class="bi bi-lightning-charge-fill text-warning"></i> ¡Hola, Bootstrap!</h1>
    <p class="lead">Este es un ejemplo usando Bootstrap 5 e íconos de Bootstrap.</p>
    <button class="btn btn-primary">
      <i class="bi bi-hand-thumbs-up"></i> Me gusta
    </button>
  </div>

  <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js"></script>
</body>
</html>
```

### Tarea

Haz una lista ilustrada de los componentes de Boostrap 5. Mira este [ejemplo](https://user-images.githubusercontent.com/17054057/51866907-7e001f00-234a-11e9-8c38-419ae045f9f7.png). Añade una descripción del uso de cada uno.

## 2BS02: Uso el sistema de rejillas en Boostrap (Grid system) :id=grid-system

> <i class="bi bi-calendar"></i> **Fecha:** 19 al 23 de Mayo<br><i class="bi bi-window-desktop"></i> **Programa:** [Visual Studio Code](https://code.visualstudio.com/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Ver al final<br><i class="bi bi-play-btn"></i> **Videos:** [Video 1](https://www.youtube.com/watch?v=p3rW1JJg3C0) / [Video 2](https://www.youtube.com/watch?v=k8ovx51cEBg)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/1sS6GGJK9ZJz4Go2m57zzpjfSGLDMH5jn?usp=sharing)

El sistema de rejilla (grid system) de Bootstrap es una de las herramientas más poderosas y versátiles para construir interfaces web responsivas y bien organizadas. Basado en una estructura de 12 columnas, este sistema permite distribuir y alinear contenido de forma flexible mediante clases predefinidas. Cada fila se divide en columnas que se ajustan automáticamente al tamaño de la pantalla, lo que garantiza que el diseño funcione correctamente en dispositivos móviles, tabletas y computadoras de escritorio. Gracias al grid de Bootstrap, los desarrolladores pueden crear diseños complejos sin necesidad de escribir mucho CSS personalizado, lo que agiliza el proceso de maquetación y asegura coherencia visual en todo el sitio.

### Ejemplo

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Ejemplo de 12 columnas</title>
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="p-4">

  <div class="container">
    <h2 class="mb-4">Ejemplo de Rejilla de 12 Columnas</h2>

    <!-- Una fila con 12 columnas individuales -->
    <div class="row text-center mb-3">
      <div class="col-1 bg-primary text-white">1</div>
      <div class="col-1 bg-secondary text-white">2</div>
      <div class="col-1 bg-success text-white">3</div>
      <div class="col-1 bg-danger text-white">4</div>
      <div class="col-1 bg-warning text-dark">5</div>
      <div class="col-1 bg-info text-white">6</div>
      <div class="col-1 bg-dark text-white">7</div>
      <div class="col-1 bg-primary text-white">8</div>
      <div class="col-1 bg-secondary text-white">9</div>
      <div class="col-1 bg-success text-white">10</div>
      <div class="col-1 bg-danger text-white">11</div>
      <div class="col-1 bg-warning text-dark">12</div>
    </div>

    <!-- Ejemplo de 3 columnas de 4 espacios -->
    <div class="row text-center mb-3">
      <div class="col-4 bg-info text-white">col-4</div>
      <div class="col-4 bg-info text-white">col-4</div>
      <div class="col-4 bg-info text-white">col-4</div>
    </div>

    <!-- Ejemplo de 2 columnas de 6 espacios -->
    <div class="row text-center mb-3">
      <div class="col-6 bg-success text-white">col-6</div>
      <div class="col-6 bg-success text-white">col-6</div>
    </div>

    <!-- Ejemplo de 1 columna que ocupa todo el ancho -->
    <div class="row text-center">
      <div class="col-12 bg-dark text-white">col-12 (una sola columna)</div>
    </div>
  </div>

</body>
</html>
```

### Tarea

Completa el CV de ejemplo en HTML, tomale captura a la página web, imrpimelo y presentálo en folder.

<div class="currentTheme">

## 2BS03: Hago uso de estilos básicos y utilidades :id=bootstrap-estilos-basicos

> <i class="bi bi-calendar"></i> **Fecha:** 02 al 06 de Junio<br><i class="bi bi-window-desktop"></i> **Programa:** [Visual Studio Code](https://code.visualstudio.com/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Ver al final<br><i class="bi bi-play-btn"></i> **Videos:** [Video 1](https://www.youtube.com/watch?v=XXllX0A_9KQ)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/1sS6GGJK9ZJz4Go2m57zzpjfSGLDMH5jn?usp=sharing)

Bootstrap es un framework de desarrollo front-end de código abierto, inmensamente popular, diseñado para facilitar la creación de sitios web y aplicaciones web responsivas y con un enfoque "mobile-first" de manera rápida y eficiente. Proporciona una vasta colección de componentes pre-diseñados y listos para usar, como botones, formularios, barras de navegación, modales, y un potente sistema de rejilla (grid system) que simplifica enormemente la organización del contenido y la adaptación del diseño a diferentes tamaños de pantalla, desde teléfonos móviles hasta grandes escritorios. Al utilizar Bootstrap, los desarrolladores pueden acelerar significativamente el proceso de maquetación, asegurar una mayor consistencia visual y funcional a través de diferentes navegadores y dispositivos, y enfocarse más en la lógica de la aplicación en lugar de en los detalles minuciosos del CSS y JavaScript para la interfaz.

### Ejemplo

```html
<!DOCTYPE html>
<html lang="es">
<head>
  <meta charset="UTF-8">
  <title>Utilidades de Bootstrap 5</title>
  <meta name="viewport" content="width=device-width, initial-scale=1">
  <!-- Bootstrap 5 -->
  <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css" rel="stylesheet">
</head>
<body class="bg-light text-dark">

  <div class="container py-5">

    <h1 class="text-center text-primary mb-5 fw-bold">Demostración de Utilidades en Bootstrap 5</h1>

    <!-- Espaciado y colores -->
    <div class="p-4 mb-4 bg-info text-white rounded">
      <p class="mb-0">Este bloque tiene padding, margen, color de fondo y texto blanco.</p>
    </div>

    <!-- Tipografía -->
    <p class="fs-1 text-center">fs-1</p>
    <p class="fs-3 text-end text-muted fw-light">fs-3, texto a la derecha, color tenue y fuente ligera</p>
    <p class="text-uppercase fw-semibold text-success">Texto en mayúsculas y negrita semibold</p>

    <!-- Flexbox -->
    <div class="d-flex justify-content-between align-items-center bg-warning text-dark p-3 mb-4">
      <div>Izquierda</div>
      <div class="fw-bold">Centro</div>
      <div>Derecha</div>
    </div>

    <!-- Display y visibilidad responsive -->
    <div class="d-none d-md-block alert alert-success">
      Visible solo en pantallas medianas (≥768px) o mayores.
    </div>
    <div class="d-block d-md-none alert alert-danger">
      Visible solo en pantallas pequeñas (&lt;768px).
    </div>

    <!-- Bordes y sombras -->
    <div class="border border-3 border-primary rounded-3 shadow-lg p-3 mb-4">
      Caja con borde azul grueso, bordes redondeados y sombra grande.
    </div>

    <!-- Posicionamiento -->
    <div class="position-relative bg-secondary text-white p-4 mb-4" style="height: 150px;">
      <div class="position-absolute top-0 start-0 bg-danger px-3 py-1 rounded">
        Esquina superior izquierda
      </div>
      <div class="position-absolute bottom-0 end-0 bg-success px-3 py-1 rounded">
        Esquina inferior derecha
      </div>
    </div>

    <!-- Tamaños -->
    <div class="bg-dark text-white p-2 mb-3 w-50 h-100">
      Caja con w-50 (ancho del 50%)
    </div>

    <button class="btn btn-outline-primary w-100">Botón con w-100</button>

    <!-- Grid + utilidades combinadas -->
    <div class="row mt-5">
      <div class="col-md-4 mb-3">
        <div class="bg-light border p-3 text-center rounded shadow-sm h-100">
          <h5 class="text-primary">Caja 1</h5>
          <p class="text-muted">Utiliza columnas, borde, sombra y espaciado.</p>
        </div>
      </div>
      <div class="col-md-4 mb-3">
        <div class="bg-light border p-3 text-center rounded shadow-sm h-100">
          <h5 class="text-primary">Caja 2</h5>
          <p class="text-muted">Responsive con `.col-md-*` y `.h-100`.</p>
        </div>
      </div>
      <div class="col-md-4 mb-3">
        <div class="bg-light border p-3 text-center rounded shadow-sm h-100">
          <h5 class="text-primary">Caja 3</h5>
          <p class="text-muted">Diseño limpio solo con utilidades.</p>
        </div>
      </div>
    </div>

  </div>

</body>
</html>

```

### Tarea

Ve a la documentación de Bootstrap y revisa las utilidades. En una hoja explica y describe el uso de cada uno. Ajuntar en folder.

</div>

## 2BS04: Entiendo los colores, botones y fondos de bootstrap :id=bootstrap-colors-buttons

> <i class="bi bi-calendar"></i> **Fecha:** 09 al 13 de Junio<br><i class="bi bi-window-desktop"></i> **Programa:** [Visual Studio Code](https://code.visualstudio.com/)<br><i class="bi bi-calendar-check"></i> **Tarea:** Sin tarea<br><i class="bi bi-play-btn"></i> **Videos:** [Video](https://www.youtube.com/watch?v=XXllX0A_9KQ)<br><i class="bi bi-briefcase"></i> **Recursos:** [Recursos](https://drive.google.com/drive/folders/1sS6GGJK9ZJz4Go2m57zzpjfSGLDMH5jn?usp=sharing)

En Bootstrap, el uso de colores y botones es fundamental para diseñar interfaces web modernas, visualmente atractivas y funcionales. Este framework incluye una amplia paleta de colores predefinidos (como primary, success, danger, entre otros) que permiten aplicar estilos consistentes y profesionales con solo agregar clases específicas. Los botones, por su parte, se personalizan fácilmente mediante clases como .btn, .btn-primary, .btn-danger, etc., lo que facilita su adaptación a diferentes contextos de uso. Gracias a estas utilidades, los desarrolladores pueden crear botones llamativos, interactivos y accesibles sin necesidad de escribir mucho código CSS, acelerando el desarrollo y manteniendo una apariencia coherente en toda la página.

## 2BS05: Práctica Calificada - Revisión de folder :id=practica-calificada

> <i class="bi bi-calendar"></i> **Fecha:** Semana 6 en hora de clase<br><i class="bi bi-window-desktop"></i> **Programa:** [Visual Studio Code](https://code.visualstudio.com/)

Descarga el archivo de ejemplo de la semana 5, en la carpeta de Recursos. Agrega lo siguiente:

1. Añade las clases de los iconos de Boostrap según corresponda.
2. Agrega las miniaturas correspondientes, según la película, serie, etc. que hayas decidido colocar.
3. Añade las tres lineas de códigos de enlace de Boostrap y sus iconos.
4. Cambia el tema de oscuro a claro.

Una vez terminado, guarda tu archivo y presentálo el día de clases. Puedes llevarlo en USB o enviarlo el profesor colocando tus apellidos en el nombre del archivo, por ejemplo: `PeriquitoDeLosPalotesPepito-3A-youtube.html`

