# Trabajo práctico: SIMD

A continuación se deja una copia de la sección enunciado del tp extraído del archivo del mismo nombre (`enunciado.pdf`). Para información sobre el contenido de cada carpeta leer dicho archivo:

## Introducción

Este trabajo práctico consiste en implementar filtros gráficos utilizando el modelo de 
procesamiento [SIMD](https://es.wikipedia.org/wiki/SIMD). El TP consta de dos componentes igualmente importantes. En primer lugar
aplicaremos lo estudiado en clase programando de manera vectorizada un conjunto de filtros.
Luego, considerando las características de microarquitectura del procesador, se pedirá realizar
un análisis experimental del funcionamiento de los filtros. Estos serán codificados en lenguaje
ensamblador y lenguaje C.
La etapa de experimentación se deberá realizar con un carácter científico y una metodología
clara. Resulta fundamental entonces, la rigurosidad y exhaustividad del análisis que realicen.

## Filtros

Los tres filtros a implementar se denominarán Ocultar,Descubrir y Zig-Zag. El primer par
de filtros permitirán ocultar una imagen dentro de otra y recuperar la imagen oculta. El filtro
Zig-Zag por su parte generar un efecto de corrimiento en la imagen.

## Objetivos
- Aprendizaje del modelo SIMD; instrucciones y uso de registros XMMX.
- Mediante experimentación, realizar medidas que permitan comparar la performance de los filtros escritos en C vs. los mismos escritos en ASM. Los resultados fueron explayados mediante la realización de un informe (`informe.pdf`).

--------------------------------------------------------------------------------------------------------------------------------

La carpeta `src/filters` contiene tanto las implementaciones en C como las de ASM.
