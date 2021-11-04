---
layout: default
title: Alineamientos Múltiples 
nav_order: 3
has_children: true
permalink: /alineamientos-multiples
---

Alineamientos múltiples 
{: .fs-9 	.text-purple-000}

En teoría los algoritmos de programación dinámica que se describieron anteriormente para el caso de alineamientos pareados se pueden extender para el caso de un número arbitrario de secuencias. En la práctica, esto resulta muy costoso computacionalmente, por lo que se han desarrollado otros algoritmos que implementan atajos en la búsqueda de los alineamientos óptimos (heurísticas). El desarrollo de algoritmos para el alineamiento múltiple de secuencias es una de las áreas más dinámicas de la bioinformática. Actualmente existen decenas de programas que implementan diferentes algoritmos (vea: Notredame, 2007 y Lemey et al., 2009 para una revisión del tema). 


En esta sesión vamos a desarrollar la práctica que se presenta en el capítulo 3 de Lemey et al., 2009. 
En este ejercicio vamos a alinear las secuencias de los genes COI y EF1α que limpiaron la clase pasada. Estos datos son parte de un trabajo en sistemática y biogeografía de mariposas de la tribu Satirinae de la familia Nimphalidae. Vamos a usar métodos de alineamiento progresivo (ClustalX), basado en consistencias (T-coffee y MAFT) y de refinamiento iterativo (Muscle) para crear alineamientos múltiples de proteínas para el gen COI. Vamos a crear los alineamientos de las secuencias de las proteínas, vamos a comparar los diferentes métodos y vamos a generar el alineamiento correspondiente a nivel de nucleótidos, terminando con la inspección y refinamiento manual del alineamiento. 

