# 5-Secundaria - Unidad 2

## 1BS06: Introducción a Latex

> <i class="bi bi-calendar"></i> **Fecha:** 08 al 12 de Abril<br><i class="bi bi-laptop"></i> **Programa:** [Papeeria](https://papeeria.com/ "Title") / [TextStudio](https://www.texstudio.org/)<br><i class="bi bi-clipboard-check"></i> **Tarea:** Usando latex crea el cuento de la Caperucita Roja. <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=99swbZlIxTk<br><i class="bi bi-files"></i> **Recursos:** https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Las matemáticas, con su precisión y rigor, son un lenguaje fundamental en la ciencia, la ingeniería y muchos otros campos académicos y profesionales. Sin embargo, la representación precisa de fórmulas matemáticas en documentos digitales ha sido históricamente un desafío. LaTeX, un sistema de composición de textos especialmente diseñado para la creación de documentos científicos y técnicos, se ha convertido en la herramienta preferida para este propósito. La fortaleza de LaTeX radica en su capacidad para generar fórmulas matemáticas complejas con una calidad tipográfica excepcional, lo que lo hace indispensable para estudiantes, investigadores y profesionales que requieren representar de manera precisa y estética ecuaciones, teoremas y símbolos matemáticos en sus documentos. En esta introducción, exploraremos el uso de LaTeX como una herramienta poderosa y versátil para la escritura de documentos matemáticos, destacando sus características específicas, su flexibilidad y su papel fundamental en la comunicación y presentación de conceptos matemáticos de manera clara y profesional.

## 1BS07: Desarrollo notaciones matemáticas en Látex

> <i class="bi bi-calendar"></i> **Fecha:** 15 al 19 de Abril<br><i class="bi bi-laptop"></i> **Programa:** [CodeGS](https://latex.codecogs.com/eqneditor/editor.php?lang=es-es"CodeGS") / [TextStudio](https://www.texstudio.org/)<br><i class="bi bi-clipboard-check"></i> **Tarea:** Escribe 10 fórmulas matemáticas usando Latex. Muetsra el código y el resultado. <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=Zzn7z5J5-Ak<br><i class="bi bi-files"></i> **Recursos:** https://manualdelatex.com/tutoriales/ecuaciones / https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Una de las características más destacadas de LaTeX es su capacidad para generar ecuaciones matemáticas con una alta calidad tipográfica. Para ello, LaTeX ofrece un conjunto de comandos específicos que permiten escribir ecuaciones de manera sencilla y elegante.

A continuación, se presenta un ejemplo básico de cómo escribir una ecuación en LaTeX:

```latex
\documentclass{article}
\usepackage{amsmath}

\begin{document}

La ecuación de una recta en el plano cartesiano se representa como:

\begin{equation}
y = mx + b
\end{equation}

donde $m$ es la pendiente de la recta y $b$ es la ordenada al origen.

\end{document}
```


En este ejemplo, <code>\begin{equation}</code> y <code>\end{equation}</code> se utilizan para delimitar la ecuación, mientras que *y = mx + b* es la propia ecuación matemática. Además, se ha utilizado el paquete **amsmath** para acceder a funciones y entornos matemáticos adicionales.

## 1BS08: Inserto gráficos usando Látex

> <i class="bi bi-calendar"></i> **Fecha:** 22 al 26 de Abril<br><i class="bi bi-laptop"></i> **Programa:** [Papeeria](https://papeeria.com/) / [TextMaker](https://www.xm1math.net/texmaker/)<br><i class="bi bi-clipboard-check"></i> **Tarea:** Escribe 10 fórmulas matemáticas usando Latex. Muestra el código y el resultado. <br><i class="bi bi-youtube txt-red"></i> **Videos:** https://www.youtube.com/watch?v=oeM1SJTQWOM<br><i class="bi bi-files"></i> **Recursos:** https://es.wikibooks.org/wiki/Manual_de_LaTeX/Inclusi%C3%B3n_de_gr%C3%A1ficos/Gr%C3%A1ficos_con_TikZ / https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

La biblioteca TikZ es una herramienta poderosa y versátil para la creación de gráficos y figuras en LaTeX, el sistema de composición de documentos ampliamente utilizado en la comunidad académica y técnica. TikZ, que significa "TikZ ist kein Zeichenprogramm" (TikZ no es un programa de dibujo) en alemán, permite a los usuarios generar gráficos de alta calidad directamente dentro de sus documentos LaTeX, proporcionando un control preciso sobre cada aspecto de la apariencia y el diseño.

Desde diagramas simples hasta gráficos complejos, TikZ ofrece una amplia gama de capacidades para crear una variedad de elementos visuales, incluidos diagramas de flujo, árboles, diagramas de red, gráficos de dispersión y mucho más. Su integración perfecta con LaTeX garantiza una coherencia estilística y tipográfica en todo el documento.

### Código de clase

```latex

% Esto se coloca al inicio del documento
\usepackage{tikz}


% Ahora usa el paquete despues del inicio del documento \begin{document}
\begin{tikzpicture}

    % Dibujando el triángulo
    \draw (1,1) -- (5,1) -- (1,3) -- cycle;

    % Añadiendo el ángulo recto
    \draw (1,1.5) -- (1.5,1.5) -- (1.5,1);

    % Agregando medidas
    \node at (3,0.5) {8m};
    \node at (3.4,2.4) {10m};

\end{tikzpicture}

```

<div class="currentTheme">

## 1BS09: Insertando la información Látex en Excel

> <i class="bi bi-calendar"></i> **Fecha:** 29 de Abril al 04 de Mayo<br><i class="bi bi-laptop"></i> **Programa:** [Papeeria](https://papeeria.com/) / [TextMaker](https://www.xm1math.net/texmaker/)<br><i class="bi bi-clipboard-check"></i> **Tarea:** Sin tarea <br><i class="bi bi-files"></i> **Recursos:** https://app.box.com/s/jfmtavrh9cphyksxokegrh3p75kkuch5

Integrar LaTeX dentro de Excel permite a los usuarios aprovechar las capacidades de formateo y presentación de LaTeX mientras trabajan con datos y cálculos en una hoja de cálculo. Esto puede ser especialmente útil para aquellos que necesitan presentar resultados complejos o fórmulas matemáticas en sus documentos de Excel de una manera elegante y profesional.

La combinación de LaTeX y Excel puede ofrecer una serie de beneficios, como la capacidad de crear informes técnicos y científicos que incluyan tanto datos numéricos como contenido matemático detallado. Además, LaTeX proporciona un control preciso sobre el formato del texto y las ecuaciones, lo que permite una presentación altamente personalizada y estéticamente atractiva.

</div>

## 1BS10: Práctica Calificada & Revisión de Folder

> <i class="bi bi-calendar"></i> **Fecha:** Semana 10<br><i class="bi bi-laptop"></i> **Programa:** Cualquier intérprete de Latex.

Para esta semana deberás realizar tu práctica calificada que consiste en lo siguiente:

1. Escoge 10 ejercicios de la página 145 -> 146 de tu separata (Trigonometría - Sigo practicando).
2. Usando latex realiza dichas fórmulas, gráficos, etc.
3. Para AD: Haz la resolución de dichos ejercicios usando latex.

Copiar el código a un archivo txt para que el profesor lo copie y lo ejecute en su programa. Enviar dicho archivo por correo a: israel@israelcueva.com

> No habrá extensión de fecha para la práctica.