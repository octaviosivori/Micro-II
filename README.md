# Microeconomía II

Apuntes de **Octavio Sivori** para Microeconomía II, Maestría en Economía de la Universidad Torcuato Di Tella.

Los documentos transcriben los apuntes manuscritos en formato artículo. Las slides de la materia se utilizan como referencia para las figuras; no se incorpora su transcripción completa.

## Documentos

| Tema | Fuente LaTeX | PDF | Páginas del PDF |
| --- | --- | --- | ---: |
| Equilibrio General | [TeX](1_Equilibrio_General.tex) | [PDF](1_Equilibrio_General.pdf) | 23 |
| Nash y equilibrios correlacionados | [TeX](2_Nash.tex) | [PDF](2_Nash.pdf) | 19 |
| Equilibrio perfecto en subjuegos (ESP) | [TeX](3_ESP.tex) | [PDF](3_ESP.pdf) | 7 |
| Juegos Repetidos | [TeX](4_Juegos_Repetidos.tex) | [PDF](4_Juegos_Repetidos.pdf) | 4 |

Cada `.tex` es un documento independiente y contiene sus figuras: no requiere imágenes, bibliografía ni archivos de entrada externos.

## Formato

- Artículo de 11 puntos en papel A4, con márgenes de 2,35 cm.
- Encabezado «Octavio Sivori / Micro II» y número de página al pie.
- Secciones por subtemas y cajas rojas con fondo rosa claro para definiciones y resultados.
- Definiciones completas dentro de sus recuadros.
- Figuras en TikZ. En Equilibrio General se conservan los contornos vectoriales de las figuras de las slides y se redibujan cuatro esquemas auxiliares del manuscrito.
- Demostraciones de Equilibrio General delimitadas con un símbolo de cierre al final de cada prueba completa.

## Compilar en Overleaf

1. Creá un proyecto vacío y subí los cuatro archivos `.tex`, o importá este repositorio.
2. En la configuración del proyecto, seleccioná el `.tex` del tema que quieras compilar como **documento principal**.
3. Elegí **pdfLaTeX** como compilador y recompilá.

Para cambiar de tema, seleccioná otro documento principal.

## Compilar localmente

Con una distribución de LaTeX que incluya `pdflatex` y los paquetes utilizados, ejecutá desde la carpeta del repositorio:

```sh
pdflatex -interaction=nonstopmode -halt-on-error 1_Equilibrio_General.tex
pdflatex -interaction=nonstopmode -halt-on-error 1_Equilibrio_General.tex
```

Reemplazá el nombre por `2_Nash.tex`, `3_ESP.tex` o `4_Juegos_Repetidos.tex` para compilar los otros temas. Dos pasadas permiten actualizar las referencias y los marcadores del PDF.

Los PDF incluidos corresponden a las fuentes de este repositorio y fueron compilados con `pdflatex`.
