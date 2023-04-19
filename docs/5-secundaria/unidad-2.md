# 5-Secundaria - Unidad 2

## 1BS06: Introducción a VBA

> **Fecha:** 10 al 14 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Crea un cheatsheet de VBA, imprimelo y colocalo en tu folder<br>

Visual Basic for Applications (VBA) es un lenguaje de programación que se utiliza en conjunto con las aplicaciones de Microsoft Office, como Excel, Word y PowerPoint. Con VBA, los usuarios pueden automatizar tareas repetitivas, crear funciones personalizadas y desarrollar aplicaciones personalizadas que se integran perfectamente con el software de Microsoft. VBA es una herramienta poderosa que permite a los usuarios ampliar la funcionalidad de sus aplicaciones de Office y ahorrar tiempo al automatizar tareas tediosas. Aunque VBA puede parecer intimidante al principio, con un poco de práctica y paciencia, incluso los principiantes pueden comenzar a escribir sus propios códigos. En resumen, VBA es una herramienta invaluable para cualquier persona que desee mejorar su productividad y capacidad de personalización en las aplicaciones de Microsoft Office.

<div class="currentTheme">

## 1BS07: Elaboro un script básico usando variables y objetos

> **Fecha:** 17 al 21 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Sin tarea<br> 

Las variables en VBA son elementos fundamentales para almacenar y manipular datos en programas de Excel. En VBA, las variables pueden ser de diferentes tipos, como texto, números, fechas o valores lógicos. Además, las variables pueden ser declaradas y asignadas valores en cualquier momento dentro del programa.

En VBA, una variable puede almacenar diferentes tipos de datos, algunos de los tipos de datos más comunes son:

- Texto: Cadena de caracteres alfanuméricos, se declara utilizando la palabra clave "String".
- Números enteros: Se almacenan números enteros positivos o negativos, se declara utilizando la palabra clave "Integer" o "Long".
- Números decimales: Se almacenan números con decimales, se declara utilizando la palabra clave "Single" o "Double".
- Valores lógicos: Se almacenan valores "Verdadero" o "Falso", se declara utilizando la palabra clave "Boolean".
- Fechas: Se almacenan fechas y horas, se declara utilizando la palabra clave "Date".

Además, VBA también tiene otros tipos de datos que pueden ser útiles en diferentes situaciones, tales como: arreglos (Arrays), objetos (Object), variables de referencia (Variant), entre otros.

Es importante tener en cuenta que al declarar una variable, es necesario indicar su tipo de datos para que VBA pueda asignar la cantidad adecuada de memoria para almacenar el valor.

Ejemplo:

```visual-basic
Sub ejemplo_variables()
    
    ' Variables numéricas
    Dim num_entero As Integer
    Dim num_decimal As Double
    
    num_entero = 10
    num_decimal = 5.7
    
    ' Variables de texto
    Dim nombre As String
    Dim apellido As String
    
    nombre = "Juan"
    apellido = "Pérez"
    
    ' Variable lógica
    Dim es_verdadero As Boolean
    es_verdadero = True
    
    ' Variable de fecha
    Dim fecha_actual As Date
    fecha_actual = Date
    
    ' Mostrar los valores de las variables en una celda de Excel
    Range("A1").Value = "Número entero: " & num_entero
    Range("A2").Value = "Número decimal: " & num_decimal
    Range("A3").Value = "Nombre completo: " & nombre & " " & apellido
    Range("A4").Value = "Valor lógico: " & es_verdadero
    Range("A5").Value = "Fecha actual: " & fecha_actual
    
End Sub

```

</div>