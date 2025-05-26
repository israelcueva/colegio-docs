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

<div class="currentTheme">

## 2BS02: Uso el sistema de rejillas en Boostrap (Grid system)

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

</div>
