# 3-Secundaria - Unidad 3

<div class="currentTheme">

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

</div>