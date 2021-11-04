---
layout: default
title: Secuencias de aminoacidos
parent: Alineamientos Múltiples
permalink: /alineamientos-multiples/aminoacidos
nav_order: 2
---

Alineando las secuencias de aminoácidos de COI
{: .fs-9 	.text-purple-000 .fw-300}

Exporten sus secuencias limpias en formato fasta. 

## ClustalX 

Descarguen e Inicie el programa ClustalX o inícielo localmente en su computador que lo tiene localmente instalado en geneious (Thompson et al., 1994). En ClustalX abra el archivo con las secuencias usando ```File−→Load sequences```. La interfaz gráfica le permite al usuario navegar sobre las secuencias. Seleccione ```Alignment −→ Do complete alignment```. ClustalX lleva a cabo el alineamiento progresivo y crea como salidas el árbol guía (con extensión dnd) y el alineamiento en formato Clustal (con extensión aln). Es posible escoger un formato diferente de salida para el alineamiento, siguiendo el menú ```Alignment−→Output Format```, seleccionando por ejemplo el formato Phylip que puede ser leído por muchos paquetes para inferencia filogenética. 
Recuerde que el árbol guía construido por ClustalX no debe ser usado para sacar conclusiones sobre las relaciones evolutivas entre los grupos que se están estudiando. 

- Describa las características del formato Phyllip y Nexus.
- ¿Por qué este árbol guia generado por ClustalX no debe ser usado con este fin?
{: .fs-4 	 .fw-300 	.text-center}

ClustalX tambíen permite cambiar algunos de los parámetros del alineamiento (```Alignment −→ Alignment Parameters```). 
Desafortunadamente no existen reglas generales para escoger el mejor conjunto de parámetros en un caso particular. 
La mejor opción consiste en ensayo y error. 
Si un alineamiento tiene, por ejemplo, muchos gaps largos, el usuario podría intentar incrementar la penalización para abrir gaps y rehacer el alineamiento. 
ClustalX indica el grado de conservación, revise la parte de abajo de la ventana del alineamiento, ese nivel de conservación puede ser usado para evaluar el alineamiento. 
Seleccionando ```Quality−→Calculate Low Scoring Segment6 y Quality−→Show Low Scoring Segment```, es posible visualizar aquellas regiones del alineamiento que no son confiables, que podrían removerse o refinarse manualmente. 
Salve el alineamiento usando ```File−→Save Sequences``` y selecciones Fasta como formato de salida, asegúrese de cambiar el nombre del archivo de salida para evitar sobre-escribir el archivo original. 

## T-Coffee 
Aunque el programa T-Coffee se puede instalar localmente en sus computadores, para desarrollar este ejercicio vamos a usar un servidor web. Siga el enlace http://www.tcoffee.org/ . Seleccione el formulario de envío regular para T-Coffee, allí cargue su archivo, usando ```Upload File``` o pegue las secuencias en la caja de texto de envío. Asegúrese que la opción ```Computation mode``` está en regular. Recuerde que los alineamientos con T-Coffee son más costosos desde el punto de vista computacional, ya que usa un método basado en consistencias, y por lo tanto puede tomar más tiempo que un alineamiento con ClustalX (Notredame et ̃al., 2000). Presiona el boton ```Submit``` para ejecutar el programa. Cuando el procedimiento de alineamiento halla terminado sera direccionado a una nueva página con enlaces a los archivos de salida. Salve el alineamiento en formato fasta en su computador. El archivo ```score_pdf``` contiene una versión del alineamiento coloreada dependiendo de la calidad, este archivo también está disponible en formato html. 

## Muscle 
Para obtener el alineamiento por el método de refinamiento iterativo vamos a usar el programa Muscle (Edgar, 2004). Este programa también puede ser instalado localmente en su computador, en esta ocasión vamos a usar el servidor web disponible en el EBI, siga el enlace http://www.ebi.ac.uk/Tools/muscle/index.html, allí puede cargar su archivo de secuencias usando la opción Upload a file. Asegúrese que la salida aparecerá en formato Fasta. Guarde el archivo de salida en formato fasta en su computador. 

## MAFT 
Para obtener el alineamiento por el método de refinamiento iterativo vamos a usar también el programa MAFT (Katoh, 2019). Este programa también puede ser instalado localmente en su computador, en esta ocasión vamos a usar el servidor web disponible en el enlace https://mafft.cbrc.jp/alignment/server/ 


## Comparando los programas

Haga todas las comparaciones entre los alineamientos que obtuvo anteriormente, y describa brevemente las diferencias que observa. 

¿Qué métodos de alineamientos presentan las mayores diferencias entre si? ¿Qué métodos las menores? Explique su respuesta, Si es posible busque un programa que le permita hacer comparaciones múltiples AltAVisT.  


