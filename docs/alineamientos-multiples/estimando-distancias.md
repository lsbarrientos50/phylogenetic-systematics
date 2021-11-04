---
layout: default
title: Estimando distanias
parent: Alineamientos Múltiples
permalink: /alineamientos-multiples/estimando-distancias
nav_order: 5
---

Estimando distancias entre las secuencias 
{: .fs-9 	.text-purple-000 .fw-300}

Cuando el objetivo es inferir las relaciones evolutivas entre las secuencias (o los organismos representados por las secuencias) a partir del alineamiento múltiple y usando un método de distancia9, es necesario estimar una distancia evolutiva entre ellas. Hay muchos modelos para estimar las distancias evolutivas entre las secuencias, ya sean estas de ADN o de proteínas, por lo tanto, es necesario escoger aquel modelo que mejor se ajuste a los datos (Posada and Crandall, 2001; Sullivan and Joyce, 2005). Se han desarrollado aplicaciones para automatizar y ayudar en la selección del mejor modelo siguiendo estrategias estadísticas; para secuencias de ADN existe ModelTest (Posada and Crandall, 1998; Posada, 2006) y para secuencias de proteínas ProtTest (Abascal et ̃al., 2005). Estos métodos los vamos a ver más adelante.

Para ahorrar tiempo, para este ejercicio vamos solo a estimar la distancia p entre las secuencias que corresponde a la proporción de posiciones diferentes entre cada par de secuencia. En la realidad la distancia p subestima el número real de sustituciones, ya que ignora el fenómeno de hits múltiples, i.e., que una posición dada puede haber sido sustituida mas de una vez. Los modelos que se mencionaron anteriormente implementan diferentes tipos de correcciones para tener esto en cuenta. 

Vamos a usar la aplicación protdist de Phylip, un paquete para la inferencia de relaciones evolutivas, que está disponible en http://mobyle.pasteur.fr/ o en https://evolution.genetics.washington.edu/phylip/getme-new1.html . Siga el enlace anterior y busque la aplicación protdist, selecciones la opción File y cargue el archivo con su alineamiento múltiple de proteínas. Seleccione Similarity table para el parámetro Distance Model, los demás parámetros los usamos con sus valores por defecto. Los valores en la matriz resultante indican la proposición de posiciones idénticas para cada par de secuencias. Para obtener la distancia, i.e., la proporción de posiciones diferentes entre cada par se secuencias, solo tenemos que restar el valor de la matriz a la unidad. Otra opción podría ser usar, por ejemplo, el programa MEGA4 (Tamura et ̃al., 2007)10, que puede calcular directamente la proporción de posiciones diferentes. 

Identifique el par de mariposas mas cercanas y el par mas lejano. ¿Cuáles son los valores en la matriz de distancia en los dos casos? 
{: .fs-4 	 .fw-300 	.text-center}

