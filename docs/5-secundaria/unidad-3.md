# 5-Secundaria - Unidad 3

## 2BS01: Instalando Wordpress por primera vez

> **Fecha:** 22 al 26 de Mayo<br> **Programa:** [Xampp](https://www.apachefriends.org/es/index.html)<br> **Tarea:** Ver al final<br> **Archivo:** [Wordpress](https://wordpress.org/download/)

En este clase veremos como instalar Wordpress en nuestras computadoras.

- Instalación de Xampp: https://www.youtube.com/watch?v=xXkKeojOb1A
- Instalación de Wordpress: https://www.youtube.com/watch?v=VN4EitfYf0o


### Tarea semana 1:

Instala Xampp en tu computadora y luego instala Wordpress. Tomar captura de los pasos (En una sola hoja), imprimir y adjuntar en el folder. Recuerda que las capturas deben ser las 6 siguientes:

- Pantalla final del programa de instalación de Xampp.
- Panel de control de Xampp con los servicios que necesitamos iniciados (Apache y MySql).
- Panel de control de phpmyadmin con la base de datos para wordpress creada.
- Configuración de la base de datos (Nombres de la base de datos, host, usuario, etc).
- Configuración del sitio de Wordpress ( Nombre del sitio, correo, etc).
- Panel de Control de Wordpress.

## 2BS02: Aprendo sobre los Temas y plugins en wordpress.

> **Fecha:** 29 de Mayo al 02 de Junio<br> **Programa:** Wordpress<br> **Tarea:** Ver al final. **Archivo:** [Deep Theme](https://github.com/israelcueva/colegio-docs/blob/93fac6d65ad9b07e8061eb1e433e9cd5d6d09414/docs/5-secundaria/archivos/Unidad3/deep.zip ':include :type=code') 

En este clase veremos como usar los plugins iniciales y los temas de Wordpress.

- Mejores temas gratuitos Wordpress: https://www.youtube.com/watch?v=F1DC2k7YHNM

Para nuestros ejemplos usaremos el tema Deep Theme. https://webnus.net/deep-wordpress-theme/

### Tarea semana 2:

Añade el tema escogido, crea la página de Inicio (Home) y la primera entrada (Bienvenida) en tu sitio web.

## 2BS03: Escojo un constructor de sitios

> **Fecha:** 05 al 09 de Junio<br> **Programa:** Wordpress<br> **Tarea:** Ver al final.<br> **Archivos:** [Elementor](https://github.com/israelcueva/colegio-docs/blob/2168a6b79bbb40e9c453db8ae2e39f3559ba9176/docs/5-secundaria/archivos/Unidad3/S02/elementor.3.13.4.zip)<br>

En esta clase aprenderemos a usar el constructor escogido: **Elementor**.

### Tarea semana 3:

Usa el constructor de sitios para crear una página de ejemplo.

!> Importante<br>Realizar lo siguiente para evitar problemas a la hora de instalar los plugins

#### Archivo PHP.ini

?> **Ubicación:** Xampp Control Panel-> Config (Apache) -> PHP (php.ini)

- <code>max_execution_time=120</code> cambiar a <code>max_execution_time=180</code>
- <code>;max_input_vars = 1000</code> cambiar a <code>max_input_vars = 10000</code>
- <code>memory_limit=128M</code> cambiar a <code>memory_limit=512M</code>
- <code>post_max_size=40M</code> cambiar a <code>post_max_size=1024M</code>
- <code>upload_max_filesize=40M</code> cambiar a <code>upload_max_filesize=1024M</code>
- <code>;extension=zip</code> cambiar a <code>extension=zip</code>

#### Archivo wp_config.php

?> **Ubicación:** "**C:\xampp\htdocs\wordpress**" En este caso la carpeta se llama Wordpress, toma en cuenta esto si le pusiste otro nombre.

A este archivo, antes del mensaje: **That's all, stop editing! Happy publishing.** ( ¡Eso es todo, deja de editar! Feliz blogging) Agrega el código: <code>define('WP_MEMORY_LIMIT','256M');</code>. Es decir que debe quedar así:

```
/* Add any custom values between this line and the "stop editing" line. */

define( 'WP_MEMORY_LIMIT', '256M' );
/* That's all, stop editing! Happy publishing. */
```

## 2BS04: Añado contenido a mi sitio web

> **Fecha:** 12 al 16 de Junio<br> **Programa:** Wordpress<br> **Tarea:** Sin tarea<br>

### Entradas

Las entradas de un blog se dividen en categorías, además pueden llevar etiquetas para que sea más fácil su organización. Veamos un ejemplo.

Tengo un blog donde comparto recetas de cocina, las categorías serían postres, sopas, segundos, etc. Las etiquetas de los postres podrían ser: Piña, Horno, Congelado, Licuado, etc Como se ve las categorías sirven para estructurar el contenido y las etiquetas para darle contexto a la receta.

Para tu blog deberás añadir un total de 11 entradas. Con las características siguientes.

-	Una entrada de Bienvenida con la categoría saludos.
-	9 entradas de temas varios y múltiples categorías. Estas entradas puedes copiarlo de Internet, sin embargo, al final coloca de donde fue copiado.
-	Una entrada original con la categoría editorial.

A cada entrada añade las etiquetas que creas conveniente.

### Añadiendo páginas

Las páginas serían como las secciones del sitio. Las páginas que crearemos serán:

-	Inicio/Home/Principal: Página con el contenido inicial del sitio.
-	Acerca de: Página con información acerca del autor imaginario del sitio.
-	Blog: Donde aparecerán las entradas o publicaciones del sitio. Esta página debe estar vacía.
-	Contacto: Una sección donde se pueda contactar al autor del sitio.

Todas ellas las diseñaremos usando elementor. 

Recuerda que desde los ajustes de lectura debe estar configurado para que la portada sea una página estática (Inicio) y la página de entradas sea blog.

<div class="currentTheme">

## 2BS05: Práctica Calificada & Revisión de folder

> **Fecha:** 19 al 23 de Junio<br> **Programa:** Wordpress<br>

### Práctica Calificada

Para tu práctica tu sitio de Wordpress debe tener lo siguiente:

- **11 Entradas:** Una entrada de bienvenida, una entrada original del tema y 9 entradas que pueden ser copiados de otros sitios. Cada entrada con su respectiva categoría y etiquetas.
- **4 Páginas:** La página de inicio (Diseñada con Elementor), Acerca de (Donde hablarás del autor), Blog (Donde se mostraran las entradas), Contacto (Donde iran los datos de contacto).

### Folder de Computación

Para este folder debes tener lo pedido en esta [sección](/?id=_3-folder-de-computación). También puedes tomar este folder de ejemplo:

- [Folder de María](https://www.canva.com/design/DAFldtCOBV0/ew9MmLRIBdJD38lYJ7Lrjg/view?utm_content=DAFldtCOBV0&utm_campaign=designshare&utm_medium=link&utm_source=publishsharelink)


</div>