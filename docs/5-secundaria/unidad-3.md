# 5-Secundaria - Unidad 3

## 2BS01: Creo mis propios algoritmos usando variables en Python

> <i class="bi bi-calendar"></i> **Fecha:** 20 al 24 Mayo<br><i class="bi bi-laptop"></i> **Programa:** Editor de código / https://www.online-python.com/<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=numQzIgpOo0<br><i class="bi bi-files"></i> **Recursos:** https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Python es un lenguaje de programación de alto nivel, interpretado y de propósito general, conocido por su simplicidad y legibilidad. Desde su creación por Guido van Rossum en 1991, Python ha ganado popularidad en una amplia gama de aplicaciones, incluyendo desarrollo web, análisis de datos, inteligencia artificial, automatización de tareas y más. Su diseño enfatiza la legibilidad del código y la sintaxis clara, lo que facilita el aprendizaje y el uso tanto para principiantes como para desarrolladores experimentados.

## 2BS02: Uso estructuras de control y funciones en una aplicación simple

> <i class="bi bi-calendar"></i> **Fecha:** 27 al 31 Mayo<br><i class="bi bi-laptop"></i> **Programa:** Editor de código / https://www.online-python.com/<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=9k91jETchkI<br><i class="bi bi-files"></i> **Recursos:** https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Las funciones son uno de los conceptos fundamentales en la programación y desempeñan un papel crucial en la creación de código eficiente, reutilizable y mantenible. Una función es un bloque de código diseñado para realizar una tarea específica. Al usar funciones, los programadores pueden dividir su código en partes más manejables, lo que facilita la lectura, depuración y actualización del programa.

### Tarea

Envia tu propuesta al tema escogido de lo que se te presentó en clase. Usa el formulario siguiente:

https://docs.google.com/forms/d/e/1FAIpQLScquRlyAeqVee3dHC6i56ZJYufCpwTgt3TN6xVSj23-Lt3AGQ/viewform?usp=sf_link

## 2BS03: Entiendo los conjunto de datos y los recorro usando bucles

> <i class="bi bi-calendar"></i> **Fecha:** 03 al 07 de Junio<br><i class="bi bi-laptop"></i> **Programa:** Editor de código / https://www.online-python.com/<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=B10alyprBOc<br><i class="bi bi-files"></i> **Recursos:** https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Las listas son estructuras de datos ordenadas y mutables que pueden almacenar una colección de elementos, los cuales pueden ser de diferentes tipos, como enteros, cadenas de texto, u otras listas. Las listas son extremadamente versátiles y permiten realizar una variedad de operaciones, como agregar, eliminar y modificar elementos.

Una lista en Python se define usando corchetes [], y los elementos se separan por comas.

Los bucles permiten repetir una secuencia de instrucciones varias veces, lo que es esencial para automatizar tareas repetitivas y manejar colecciones de datos. Python ofrece dos tipos principales de bucles: for y while.

<div class="currentTheme">

## 2BS04: Instalo y aprendo el uso de librerías externas

> <i class="bi bi-calendar"></i> **Fecha:** 10 al 14 de Junio<br><i class="bi bi-laptop"></i> **Programa:** Editor de código / https://python-fiddle.com/<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=B10alyprBOc<br><i class="bi bi-files"></i> **Recursos:** https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Python es un lenguaje de programación extremadamente poderoso y versátil, en parte gracias a su vasto ecosistema de librerías externas. Estas librerías, también conocidas como módulos o paquetes, amplían las capacidades de Python al proporcionar funciones y herramientas adicionales que no están incluidas en la biblioteca estándar. Al utilizar librerías externas, los desarrolladores pueden ahorrar tiempo y esfuerzo al aprovechar soluciones ya creadas y probadas para una amplia variedad de tareas y aplicaciones.

### Usando libreria Pandas

```python
import pandas as pd
df = pd.read_csv("https://raw.githubusercontent.com/mwaskom/seaborn-data/master/mpg.csv")
df.head()
```

### Usando libreria request

```python
import requests

datitos = requests.get("https://pokeapi.co/api/v2/pokemon?limit=100000&offset=0")
datosJS = datitos.json()

dataJS = datosJS["results"]

for pokemon in range(1,11):
    nombre = dataJS[pokemon]["name"]
    print(f'Pókemon {pokemon} : {nombre}')
```

</div>

## 2BS05: Práctica Calificada & Revisión de Folder

> <i class="bi bi-calendar"></i> **Fecha:** Semana 05<br><i class="bi bi-laptop"></i> **Programa:** Cualquier editor de código.

Para esta semana deberás realizar tu práctica calificada que consiste en lo siguiente:

1. Guarda una copia de este notebook en tu drive. https://colab.research.google.com/drive/1lZeWUevmhg03ltcOcdG9aosikw2TAQtL?usp=sharing
2. Resuelve los ejercicios propuestos.
3. Copia el enlace de compartir de tu notebook.
4. Haz tu presentación a través del siguiente formulario: https://forms.gle/wd8VU7FauyR1PZC9A

> No habrá extensión de fecha para la práctica.