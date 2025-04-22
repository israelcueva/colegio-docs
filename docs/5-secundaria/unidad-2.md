# 5-Secundaria - Unidad 2

## 1BS06: Uso macros en Excel para llenar una formulario

> <i class="bi bi-calendar"></i> **Fecha:** 07 al 11 de Abril<br><i class="bi bi-laptop"></i> **Programa:** Microsoft Excel<br><i class="bi bi-clipboard-check"></i> **Tarea:** Ver el final<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/shorts/mwpfxs-wKzg<br> <i class="bi bi-backpack"></i> **Recursos:** https://drive.google.com/drive/folders/1IAVg1vC0uFupTV1WnKcwjR4tm0hwY9Hj?usp=sharing

Las macros en Excel son una poderosa herramienta que permite automatizar tareas repetitivas, ahorrando tiempo y reduciendo errores. Una macro es básicamente una serie de instrucciones grabadas que Excel puede ejecutar automáticamente, como si alguien las hiciera paso a paso por ti.

Por ejemplo, si todos los días copias datos de una hoja, los ordenas, aplicas formato y generas un informe, puedes grabar todos esos pasos una vez como una macro y luego ejecutarlos con un solo clic o atajo de teclado.

Las macros se escriben utilizando VBA (Visual Basic for Applications), el lenguaje de programación integrado en Excel. Sin embargo, no necesitas saber programar para empezar: puedes grabar tus acciones con la herramienta de grabación de macros y Excel generará el código por ti.

**¿Para qué sirven las macros?**

- Automatizar procesos largos o rutinarios.
- Crear botones personalizados en tus hojas de cálculo.
- Estandarizar reportes o formatos.
- Aumentar la eficiencia al trabajar con grandes volúmenes de datos.

**¿Cómo se graba una macro?**

1. Ve a la pestaña Vista o Desarrollador.
2. Haz clic en Grabar macro.
3. Realiza las acciones que deseas automatizar.
4. Detén la grabación.

¡Listo! Puedes volver a ejecutar la macro cuando lo necesites.

Las macros son especialmente útiles en entornos laborales donde se manejan datos constantemente. Aprender a usarlas abre la puerta a un nivel más avanzado y profesional del uso de Excel.

### Tarea

Escribe el código creado por la Macro y añade un `MsgBox` al final, con la leyenda **Dato agregado correctamente**. Presentar dicho trabajo escrito en el folder.

## 1BS07: Usando variables para almacenar valores

> <i class="bi bi-calendar"></i> **Fecha:** 14 al 18 de Abril<br><i class="bi bi-laptop"></i> **Programa:** Microsoft Excel<br><i class="bi bi-clipboard-check"></i> **Tarea:** Crea un cheatsheet de VBA a mano.<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=FwjzdAKMwzA<br> <i class="bi bi-backpack"></i> **Recursos:** https://drive.google.com/drive/folders/1IAVg1vC0uFupTV1WnKcwjR4tm0hwY9Hj?usp=sharing

En VBA (Visual Basic for Applications), una **variable** es un espacio en la memoria que se utiliza para almacenar datos que pueden cambiar durante la ejecución de un programa. Usar variables permite que tu código sea más flexible y fácil de mantener.

Para declarar una variable en VBA, se utiliza la palabra clave `Dim`, seguida del nombre de la variable y, opcionalmente, el tipo de dato. Por ejemplo:

```vba
Dim edad As Integer
Dim nombre As String
```

Los tipos de datos comunes en VBA incluyen:

- `Integer`: para números enteros.
- `Double`: para números con decimales.
- `String`: para cadenas de texto.
- `Boolean`: para valores True o False.

Asignar un valor a una variable es sencillo:

```vba
edad = 25
nombre = "Luis"
```
<div class="currentTheme">

## 1BS08: Uso controles de flujo para repetir instrucciones

> <i class="bi bi-calendar"></i> **Fecha:** 21 al 25 de Abril<br><i class="bi bi-laptop"></i> **Programa:** Microsoft Excel<br><i class="bi bi-clipboard-check"></i> **Tarea:** Ver al final<br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=dTTCh0DrfdE / https://www.youtube.com/watch?v=5Ag_sGZk3pw<br> <i class="bi bi-backpack"></i> **Recursos:** https://drive.google.com/drive/folders/1IAVg1vC0uFupTV1WnKcwjR4tm0hwY9Hj?usp=sharing

En VBA (Visual Basic for Applications), los controles de flujo son estructuras fundamentales que permiten dirigir el orden de ejecución de las instrucciones dentro de un programa. Gracias a estos controles, es posible tomar decisiones, repetir acciones o ejecutar código solo cuando se cumplen ciertas condiciones. Entre los más utilizados se encuentran las estructuras condicionales como `If...Then...Else` y `Select Case`, así como los bucles `For...Next`, `Do...Loop` y `While...Wend`. Comprender y dominar estos elementos es esencial para escribir macros eficientes y adaptables dentro del entorno de Microsoft Office. A lo largo de este documento, exploraremos cada uno de estos controles de flujo con ejemplos prácticos y recomendaciones para su uso adecuado.

---

### Ejemplo de If...Then...Else
```vba
Dim edad As Integer
edad = 18

If edad >= 18 Then
    MsgBox "Eres mayor de edad."
Else
    MsgBox "Eres menor de edad."
End If
```

### Ejemplo de Select Case
```vba
Dim dia As Integer
dia = 3

Select Case dia
    Case 1
        MsgBox "Lunes"
    Case 2
        MsgBox "Martes"
    Case 3
        MsgBox "Miércoles"
    Case Else
        MsgBox "Otro día"
End Select
```

### Ejemplo de For...Next
```vba
Dim i As Integer
For i = 1 To 5
    MsgBox "Número: " & i
Next i
```

### Ejemplo de Do...Loop
```vba
Dim contador As Integer
contador = 1

Do While contador <= 3
    MsgBox "Contador: " & contador
    contador = contador + 1
Loop
```

### Ejemplo de While...Wend
```vba
Dim j As Integer
j = 1

While j <= 3
    MsgBox "Valor de j: " & j
    j = j + 1
Wend
```

---

**Tarea:**

Escribe dos ejemplos de cada uno y adjuntalo en tu folder. Usa los colores por defecto del editor de Excel.

</div>