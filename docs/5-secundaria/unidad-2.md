# 5-Secundaria - Unidad 2

## 1BS06: Introducción a VBA

> **Fecha:** 10 al 14 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Crea un cheatsheet de VBA, imprimelo y colocalo en tu folder<br>

Visual Basic for Applications (VBA) es un lenguaje de programación que se utiliza en conjunto con las aplicaciones de Microsoft Office, como Excel, Word y PowerPoint. Con VBA, los usuarios pueden automatizar tareas repetitivas, crear funciones personalizadas y desarrollar aplicaciones personalizadas que se integran perfectamente con el software de Microsoft. VBA es una herramienta poderosa que permite a los usuarios ampliar la funcionalidad de sus aplicaciones de Office y ahorrar tiempo al automatizar tareas tediosas. Aunque VBA puede parecer intimidante al principio, con un poco de práctica y paciencia, incluso los principiantes pueden comenzar a escribir sus propios códigos. En resumen, VBA es una herramienta invaluable para cualquier persona que desee mejorar su productividad y capacidad de personalización en las aplicaciones de Microsoft Office.


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

<div class="currentTheme">

## 1BS08: Uso estructuras de control para el llenado de datos

> **Fecha:** 24 al 28 de Abril<br> **Programa:** Microsoft Excel 2015 en adelante<br> **Tarea:** Ver lista al final<br> 

Las estructuras de control en VBA son herramientas que permiten controlar el flujo de ejecución de un programa. Estas estructuras permiten la ejecución de bloques de código en función de ciertas condiciones o repeticiones, lo que permite crear programas más complejos y versátiles.

Las estructuras de control más comunes en VBA son:

**Estructuras condicionales:**

- If-Then: Ejecuta un bloque de código si se cumple una condición.
- If-Then-Else: Ejecuta un bloque de código si se cumple una condición y otro bloque de código si no se cumple la condición.

**Estructuras de repetición:**

- For-Next: Repite un bloque de código un número específico de veces.
- For-Each: Repite un bloque de código para cada elemento de una colección de datos.
- Do-While: Repite un bloque de código mientras se cumpla una condición.
- Do-Until: Repite un bloque de código hasta que se cumpla una condición.

Además, VBA también cuenta con estructuras de control más avanzadas como Select-Case, GoTo, Exit, entre otras.

### Ejemplos

#### Estructura condicional If-Then

```visual-basic
Dim edad As Integer
    edad = 25
    
    If edad >= 18 Then
        MsgBox "Eres mayor de edad"
    End If
```

#### Estructura condicional If-Then

```visual-basic
Dim nota As Integer
    nota = 8
    
    If nota >= 10.5 Then
        MsgBox "Aprobaste"
    Else
        MsgBox "Reprobaste"
    End If
```
#### Estructura de repetición For-Next

```visual-basic
    Dim i As Integer
    
    For i = 1 To 10
        MsgBox i
    Next i
```

#### Estructura de repetición Do-While

```visual-basic
Dim num As Integer
    num = 1
    
    Do While num < 10
        MsgBox num
        num = num + 1
    Loop
```

#### Estructura de repetición For-Each

```visual-basic
Dim cell As Range
Dim counter As Integer
 
For Each cell In Range("A1:C5").Cells
    counter = counter + 1
    cell.Value = counter
Next
```

#### Ejercicio de clase

- Basádnote en el ejemplo de ForEach realiza el algoritmo para que el color cambie por fila.

### Ejercicios

- Sumar los números pares de una lista de números ingresados por el usuario en el rango <code>A1:A10</code> utilizando la estructura For-Next.
- Encontrar el número mayor de una lista de números ingresados por el usuario en el rango <code>A1:A10</code> utilizando la estructura While e If Then.
- Calcular el factorial de un número ingresado por el usuario en la celda <code>A1</code> utilizando la estructura Do-While.
- Mostrar los primeros n (La n representa el número que el usuario escribió en la celda <code>A1</code>) números de la serie de Fibonacci utilizando la estructura For-Next.
- Crea una subrutina que use el rango <code>A1:A10</code> y utilice un bucle "For" para encontrar el elemento más grande de la matriz. Luego, muestra el resultado en un mensaje "MsgBox".

Tomar captura a cada código, imprimir y colocar en el folder. Puedes usar una página para embellecer el código, como por ejemplo: [Carbon](https://carbon.now.sh/) escogiendo VB.NET.

</div>
