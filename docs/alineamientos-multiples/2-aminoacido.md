---
layout: default
title: Secuencias de aminoacidos
parent: Alineamientos Múltiples
permalink: /reconstruccion-evolutiva/estado-caracteres
nav_order: 1
---

Alineando las secuencias de aminoácidos de COI
{: .fs-9 	.text-purple-000 .fw-300}

Exporten sus secuencias limpias en formato fasta. 

## ClustalX 

Descarguen e Inicie el programa ClustalX o inícielo localmente en su computador que lo tiene localmente instalado en geneious (Thompson et al., 1994). En ClustalX abra el archivo con las secuencias usando File−→Load sequences . La interfaz gráfica le permite al usuario navegar sobre las secuencias. Seleccione Alignment −→ Do complete alignment. ClustalX lleva a cabo el alineamiento progresivo y crea como salidas el árbol guía (con extensión dnd) y el alineamiento en formato Clustal (con extensión aln). Es posible escoger un formato diferente de salida para el alineamiento, siguiendo el menú Alignment−→Output Format, seleccionando por ejemplo el formato Phylip que puede ser leído por muchos paquetes para inferencia filogenética. 
Recuerde que el árbol guía construido por ClustalX no debe ser usado para sacar conclusiones sobre las relaciones evolutivas entre los grupos que se están estudiando. 

Describa las características del formato Phyllip y Nexus.
¿por qué este árbol guia generado por ClustalX no debe ser usado con este fin?
{: .fs-4 	.text-purple-000 .fw-300 	.text-center}

ClustalX tambíen permite cambiar algunos de los parámetros del alineamiento (```Alignment −→ Alignment Parameters```). 
Desafortunadamente no existen reglas generales para escoger el mejor conjunto de parámetros en un caso particular. 
La mejor opción consiste en ensayo y error. 
Si un alineamiento tiene, por ejemplo, muchos gaps largos, el usuario podría intentar incrementar la penalización para abrir gaps y rehacer el alineamiento. 
ClustalX indica el grado de conservación, revise la parte de abajo de la ventana del alineamiento, ese nivel de conservación puede ser usado para evaluar el alineamiento. 
Seleccionando ```Quality−→Calculate Low Scoring Segment6 y Quality−→Show Low Scoring Segment```, es posible visualizar aquellas regiones del alineamiento que no son confiables, que podrían removerse o refinarse manualmente. 
Salve el alineamiento usando ```File−→Save Sequences``` y selecciones Fasta como formato de salida, asegúrese de cambiar el nombre del archivo de salida para evitar sobre-escribir el archivo original. 
