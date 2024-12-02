# 3-Secundaria - Unidad 7

## 4BS01: Instalo Boostrap y sus Iconos en mi proyecto web

> <i class="bi bi-calendar"></i> **Fecha:** 21 al 25 de Octubre<<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Haz una guia en papel sobre como es el proceso de Instalación<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/bootstrap5/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://youtube.com/playlist?list=PLnunbwZjHqMO-JII_HBf5TAzdzaBJP34w&si=RMinwaRy_tXZEQ2R<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

Bootstrap es uno de los frameworks más populares para el desarrollo de sitios web y aplicaciones responsivas. Creado por el equipo de Twitter, Bootstrap ofrece una colección de herramientas basadas en HTML, CSS y JavaScript que permiten a los desarrolladores diseñar interfaces web modernas de manera rápida y eficiente. Con su sistema de rejillas (grid), componentes predefinidos y su enfoque en el diseño adaptativo (responsive), Bootstrap ha simplificado el proceso de creación de sitios web que se ven bien en cualquier dispositivo, desde computadoras de escritorio hasta smartphones.

Instalar Bootstrap en un proyecto es sencillo, y se puede hacer de varias maneras, dependiendo de tus preferencias o del entorno de desarrollo que estés utilizando. Aquí te presentamos algunas de las formas más comunes:

Instalación vía CDN (Content Delivery Network): Esta es la forma más rápida y fácil de usar Bootstrap sin necesidad de descargar archivos. Simplemente insertas un enlace en el <head> de tu archivo HTML y listo. Los archivos CSS y JS se cargan desde servidores externos.

```html

<link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/css/bootstrap.min.css">
<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.0/dist/js/bootstrap.bundle.min.js

```

## 4BS02: Entiendo los contenedores y los breackpoints

> <i class="bi bi-calendar"></i> **Fecha:** 28 de Octubre al 01 de Noviembre<<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Haz una guia en el folder explicando los contenedores y los breakpoints<br> <i class="bi bi-card-checklist"></i> **Guía:** https://www.w3schools.com/bootstrap5/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://youtube.com/playlist?list=PLnunbwZjHqMO-JII_HBf5TAzdzaBJP34w&si=RMinwaRy_tXZEQ2R<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

Bootstrap es un framework de desarrollo web front-end muy popular que proporciona una serie de herramientas y componentes prediseñados para crear sitios web responsivos y atractivos de manera rápida y sencilla. Dos de los conceptos más fundamentales en Bootstrap son los contenedores y los breakpoints.

### ¿Qué son los contenedores en Bootstrap?

Los contenedores en Bootstrap son elementos que sirven como envoltorios para el contenido de tu página. Estos contenedores proporcionan un ancho máximo y un margen interno, lo que ayuda a centrar el contenido y a mantener un diseño consistente en diferentes tamaños de pantalla.

### Tipos de contenedores:

- container: Establece un ancho máximo que se adapta a diferentes tamaños de pantalla.
- container-fluid: Ocupa el 100% del ancho disponible en todas las pantallas.
- container-{breakpoint}: Tiene un ancho máximo específico hasta un determinado breakpoint.

### ¿Qué son los breakpoints en Bootstrap?

Los breakpoints son puntos de inflexión en el diseño de tu sitio web, donde el diseño se adapta automáticamente a diferentes tamaños de pantalla. Bootstrap define varios breakpoints preestablecidos (por ejemplo, extra-small, small, medium, large, extra-large) que corresponden a diferentes anchos de pantalla.

### ¿Para qué sirven los breakpoints?

- Diseño responsivo: Permiten que tu sitio web se ajuste de manera óptima a diferentes dispositivos (móviles, tablets, desktops).
- Organización del contenido: Puedes reorganizar los elementos de tu diseño en función del tamaño de la pantalla.
- Creación de diseños personalizados: Los breakpoints te permiten crear diseños específicos para cada rango de tamaño de pantalla.

```
<!doctype html>
<html>
  <head>
    <meta charset="utf-8" />
    <title>El título de mi página</title>
    <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-QWTKZyjpPEjISv5WaRU9OFeRpok6YctnYmDr5pNlyT2bRjXh0JMhjY6hW+ALEwIH" crossorigin="anonymous">
    <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.11.3/font/bootstrap-icons.min.css">

  <body>
    <!-- Aquí empieza el encabezado principal que se mantendrá en todas las páginas del sitio web -->

    <header>
      <h1>Encabezado</h1>
    </header>

    <nav>
      <ul>
        <li><a href="#">Inicio</a></li>
        <li><a href="#">Nuestro equipo</a></li>
        <li><a href="#">Proyectos</a></li>
        <li><a href="#">Contacto</a></li>
      </ul>

      <!-- Un formulario de búsqueda es una forma no-lineal de hacer búsquedas en un sitio web. -->

      <form>
        <input type="search" name="q" placeholder="Buscar" />
        <input type="submit" value="¡Vamos!" />
      </form>
    </nav>

    <!-- Aquí está el contenido principal de nuestra página -->
    <main>
      <!-- Contiene un artículo -->
      <article>
        <h2>Título del artículo</h2>

        <p>
          Lorem ipsum dolor sit amet, consectetur adipisicing elit. Donec a diam
          lectus. Set sit amet ipsum mauris. Maecenas congue ligula as quam
          viverra nec consectetur ant hendrerit. Donec et mollis dolor. Praesent
          et diam eget libero egestas mattis sit amet vitae augue. Nam tincidunt
          congue enim, ut porta lorem lacinia consectetur.
        </p>

        <h3>Subsección</h3>

        <p>
          Donec ut librero sed accu vehicula ultricies a non tortor. Lorem ipsum
          dolor sit amet, consectetur adipisicing elit. Aenean ut gravida lorem.
          Ut turpis felis, pulvinar a semper sed, adipiscing id dolor.
        </p>

        <p>
          Pelientesque auctor nisi id magna consequat sagittis. Curabitur
          dapibus, enim sit amet elit pharetra tincidunt feugiat nist imperdiet.
          Ut convallis libero in urna ultrices accumsan. Donec sed odio eros.
        </p>

        <h3>Otra subsección</h3>

        <p>
          Donec viverra mi quis quam pulvinar at malesuada arcu rhoncus. Cum
          soclis natoque penatibus et manis dis parturient montes, nascetur
          ridiculus mus. In rutrum accumsan ultricies. Mauris vitae nisi at sem
          facilisis semper ac in est.
        </p>

        <p>
          Vivamus fermentum semper porta. Nunc diam velit, adipscing ut
          tristique vitae sagittis vel odio. Maecenas convallis ullamcorper
          ultricied. Curabitur ornare, ligula semper consectetur sagittis, nisi
          diam iaculis velit, is fringille sem nunc vet mi.
        </p>
      </article>

      <!-- el contenido aparte también se puede anidar dentro del contenido principal -->
      <aside>
        <h2>Relacionado</h2>

        <ul>
          <li><a href="#">Oh, me gusta estar junto al mar</a></li>
          <li><a href="#">Oh, me gusta estar junto al mar</a></li>
          <li><a href="#">Aunque en el norte de Inglaterra</a></li>
          <li><a href="#">Nunca deja de llover</a></li>
          <li><a href="#">Oh, bueno...</a></li>
        </ul>
      </aside>
    </main>

    <!-- Y aquí está nuestro pie de página principal que se utiliza en todas las páginas de nuestro sitio web -->

    <footer>
      <p>©Copyright 2050 de nadie. Todos los derechos revertidos.</p>
    </footer>


    <script src="https://cdn.jsdelivr.net/npm/bootstrap@5.3.3/dist/js/bootstrap.bundle.min.js" integrity="sha384-YvpcrYf0tY3lHB60NNkmXc5s9fDVZLESaAA55NDzOxhy9GkcIdslK1eN7N6jIeHz" crossorigin="anonymous"></script>
  </body>
</html>

```

## 4BS03: Configuro mi diseño a una grilla de 12

> <i class="bi bi-calendar"></i> **Fecha:** 04 al 08 de Noviembre<<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea<br> <i class="bi bi-card-checklist"></i> **Guía:** https://getbootstrap.com/docs/5.3/layout/columns/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=k8ovx51cEBg<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

La grilla de 12 columnas de Bootstrap es uno de los pilares fundamentales del framework y una herramienta poderosa para crear diseños web responsivos de manera rápida y sencilla. Basada en el sistema de rejillas (grid), esta estructura permite dividir el espacio en hasta 12 columnas iguales, lo que facilita la organización del contenido y la adaptación a diferentes tamaños de pantalla.

El sistema de grilla de Bootstrap se basa en tres elementos principales:

- Contenedores (container): establecen el ancho general del diseño. Pueden ser fijos o fluidos.
- Filas (row): agrupan columnas y aseguran una alineación adecuada.
- Columnas (col): dividen el espacio en proporciones que suman hasta 12 por fila

Por ejemplo, puedes crear un diseño donde el contenido se distribuya uniformemente en tres columnas para pantallas grandes y en una sola columna para dispositivos móviles con unas pocas líneas de código:

```
<div class="container">
  <div class="row">
    <div class="col-md-4 col-sm-12">Columna 1</div>
    <div class="col-md-4 col-sm-12">Columna 2</div>
    <div class="col-md-4 col-sm-12">Columna 3</div>
  </div>
</div>
```


## 4BS04: Uso los componentes para añadir navegación a mi proyecto

> <i class="bi bi-calendar"></i> **Fecha:** 04 al 08 de Noviembre<<br><i class="bi bi-laptop"></i> **Programa:** Editor de código<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea<br> <i class="bi bi-card-checklist"></i> **Guía:** https://getbootstrap.com/docs/5.3/components/navbar/<br> <i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=lcUWpoAKUYk<br><i class="bi bi-files"></i> **Recursos:** https://drive.google.com/drive/folders/1f5XXULPLeC_Jkl5-BNCa_qJhQESG-K8y?usp=sharing

La barra de navegación (o navbar) de Bootstrap es un componente versátil y personalizable que facilita la creación de menús de navegación modernos, funcionales y responsivos. Es una herramienta esencial en el diseño web, ya que permite a los usuarios navegar entre las diferentes secciones de un sitio de manera intuitiva, adaptándose automáticamente a dispositivos de cualquier tamaño

## 4BS05: Práctica Calificada & Revisión de Folder

> <i class="bi bi-calendar"></i> **Fecha:** Hora de clase correspondiente a la semana 6<br><i class="bi bi-laptop"></i> **Programa:** Editor de código


### Indicaciones

Sigue el siguiente video y crea tu propio navbar: https://www.youtube.com/watch?v=h5apE3E72wY

Guardar en USB, replit, codepen, etc. Y presentar en hora de clase.

