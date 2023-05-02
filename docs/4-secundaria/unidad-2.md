# 4-Secundaria - Unidad 2

## 1BS06: Uso de filtros para separar información

> **Fecha:** 10 al 14 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Ver lista al final, imprimir y adjuntar en el folder.<br> **Archivo:** [Dataset](https://data.apps.fao.org/catalog/dataset/rlc-peru-datos ':include :type=code')

Los filtros en Excel son una herramienta útil que permite a los usuarios ver y analizar datos específicos en una hoja de cálculo. Los filtros pueden ayudar a los usuarios a encontrar rápidamente la información que necesitan, lo que puede ahorrar tiempo y hacer que el proceso de análisis de datos sea más eficiente. Con los filtros, los usuarios pueden ocultar o mostrar filas o columnas de datos basados en criterios específicos, como valores numéricos, fechas, texto o incluso por color de celda.

**Tareas:**

1. Usa filtros para mostrar de mayor a menor, según el total de viviendas, los distritos de la provincia de Islay en el departamento de Arequipa.
2. Usa filtros para mostrar los distritos con mayor población rural del Perú.

## 1BS07: Inserto tablas y gráficos dinámicos avanzados

> **Fecha:** 17 al 21 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Ver lista al final, imprimir y adjuntar en el folder.<br> **Archivo:** [Dataset](https://github.com/israelcueva/colegio-docs/blob/b9ce4087a5ccf48709f4b1597e7f180f254482c3/docs/4-secundaria/archivos/Unidad2/pisa2009test.csv ':include :type=code')

Las tablas dinámicas permiten a los usuarios resumir y analizar grandes conjuntos de datos, mientras que los gráficos dinámicos permiten a los usuarios visualizar los datos en forma de gráficos interactivos. Con las tablas dinámicas, los usuarios pueden arrastrar y soltar campos de datos en filas, columnas y valores para crear resúmenes de datos personalizados. Los gráficos dinámicos permiten a los usuarios crear gráficos interactivos que se actualizan automáticamente a medida que se agregan o eliminan datos. Los usuarios también pueden aplicar filtros y segmentaciones de datos para refinar aún más los resultados de sus análisis. Las tablas y gráficos dinámicos son una herramienta esencial para cualquier persona que trabaje con grandes conjuntos de datos en Excel y necesite resumir y analizar información de manera rápida y efectiva.

**Tareas**

- Crear una tabla dinámica que muestre los promedios de lectura por tipo de institución: Pública y Privada. Además debe tener un filtro para seleccionar el grado.
- Crear una tabla dinámica que muestre los promedios de lectura por raza. Además debe tene run filtro para seleccionar por sexo.

## 1BS08: Diseño un dashboard en Excel

> **Fecha:** 24 al 28 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Crea tu diseño de Dashboard<br> **Archivo:** [Dataset](https://github.com/israelcueva/colegio-docs/blob/e0ca72b62504f2e37c45b4e0f53350febd5083a3/docs/4-secundaria/archivos/Unidad2/Marks.csv ':include :type=code') | [Dataset](https://github.com/israelcueva/colegio-docs/blob/e0ca72b62504f2e37c45b4e0f53350febd5083a3/docs/4-secundaria/archivos/Unidad2/Marks.csv ':include :type=code')

Un dashboard (o panel de control en español) es una herramienta de visualización de datos que presenta información clave de manera clara y concisa en una sola pantalla. Los dashboards se utilizan comúnmente en entornos empresariales para mostrar métricas y KPIs (indicadores clave de rendimiento) relevantes para un área específica de la empresa.

### Procedimiento:

#### 1. Preparación de los datos fuente

1. Dividir texto de CSV en columnas: [Video](https://www.youtube.com/results?search_query=dividir+csv+excel)
2. Colocar nombres a los rangos de la hoja:
    1. Seleccionar todas las columnas: [Video](https://www.youtube.com/watch?v=tOtXDGUTolk)
    2. Colocar nombres automáticos a columnas seleccionadas desde: **Fórmulas** --> **Crear desde Selección** [Video](https://www.youtube.com/watch?v=UfCl4feinP8)
    3. Seleccionar TODAS las columnas y colocarle nombre desde el cuadro de nombres (No olvides presionar enter): [Video](https://www.youtube.com/shorts/ldEtNi7xeB4)
3. Crear una nueva hoja y ponerle de nombre **Estadisticas**(Sin tilde) [Video](https://www.youtube.com/watch?v=rNWij7nxATU)
    1. En la celda A1 de la misma colocar el encabezado "Promedio_General".
    2. En la celda A2 colocar la fórmula: "=PROMEDIO(" y al abrir paréntesis seleccionar la primera hoja y seleccionar las notas del primer alumno, cerrar paréntesis y presionar enter; o simplemente escribir la fórmula: <code>=PROMEDIO(Marks!E2:BX2)</code> en esa celda.
    3. Vuelve a seleccionar la celda A2 y desde la esquina (Cuadradito verde) arrastra hasta la fila 10001 para que se completen el resto de promedios. [Video1](https://youtu.be/ufDGnFVTbWE?t=10)
    4. Selecciona toda la columna A y ponle nombre usando **Crear desde selección**.

#### 2. Hoja Dashborad

##### Llenando Datos

- Crear un hoja llamada **Dashboard**
- En la celda **B2** hacer una validación de datos(Datos->Validación de datos) de tipo Lista; siendo el ORIGEN la columna <code>Apellidos</code>. No escribas el nombre usa la opción **Utilizar en fórmula** de la ficha Fórmulas. Si no te aparece nada no hiciste el paso 2 de la preparación de datos. Si lo haz hecho bien aparecerá una flecha en la celda que al presionar nos mostrará todos los apellidos de la primera hoja.
- En la celda **D1** coloca la fórmula: <code>=COINCIDIR(B2;Apellidos;0)</code> y presiona ENTER, descuida, saldra un error, el cual se areglará seleccionado un nombre de la lista en la celda B2. La fórmula busca lo que escribas o selecciones en la celda B2 dentro del rango Apellidos con una coincidencia excacta (0).
- En la celda **E1** esribe la fórmula: <code>=INDICE(Promedio_General;D1;1)</code>. La fórmula anterior es para obtener el valor que se encuentra en el rango **Promedio_general** (Paso 3.4 de la preparación) en al fila que nos de la celda D1 y en la columna 1.
- En la celda **F1** Dividimos la nota promedio que sacó(Celda E1) con el total (20), por ende, escribe la fórmula <code>=E1/20</code>. Obtendrás un decimal, el cuál debes convertir a porcentaje con el botón porcentaje que se encuentra en la ficha Inicio.
- En la celda **G1** restaremos el porcentaje resultante de la nota(Celda F1) y el total del 100%, por ello escribe la fórmula siguiente: <code>=100%-F1</code>.

##### Colocando el gráfico circular

- Desde la ficha Insertar->Formas añade una rectángulo redondeado.
- Selecciona dicho rectángulo y en la barra de fórmulas([Referencia](https://www.accessyexcel.com/wp-content/uploads/2013/01/Excel-02_07-La-barra-de-formulas.jpg)) haz referencia a la celda donde se encuentra el porcentaje que representa la nota(F1). Lo que debería quedar así: <code>=F1</code>, luego presionamos la tecla F4 para añadir una referencia absoluta (O solo coloca el simbolo del dolar) y quedaría de esta manera: <code>=$F$1</code>
- Finalmente seleccionamos los dos porcentajes (F1:G1) y nos vamos a la ficha Insertar, escogemos gráficos recomendados y pulsamos en el gráfico circular.
- Ahora solo te falta eliminar el fondo del gráfico, eliminar cualquier elemento extra y colocarlo encima de tu rectángulo redondeado.

<div class="currentTheme">

## 1BS09: Añado funciones en mi dashboard

> **Fecha:** 01 al 05 de Mayo<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Sin tarea<br> **Archivo:** [Dataset](https://github.com/israelcueva/colegio-docs/blob/7c5a6b9b6366fd9a031b9f11f1774241878108e1/docs/4-secundaria/archivos/Unidad2/Marks.xlsx ':include :type=code') 

En esta semana completaremos nuestro Dashboard iniciado en la semana 8.

</div>