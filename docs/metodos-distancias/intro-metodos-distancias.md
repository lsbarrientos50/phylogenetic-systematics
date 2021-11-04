---
layout: default
title: Métodos de distancias
nav_order: 4
has_children: true
permalink: /metodos-distancias
---

Métodos de distancias
{: .fs-9 	.text-purple-000}

En los siguientes talleres, analizaremos dos aplicaciones que son útiles para mostrar, editar y manipular árboles filogenéticos: TreeView y FigTree. TreeView 1.6 (http://taxonomy.zoology.gla.ac.uk/rod/treeview.html) es un programa fácil de usar y de libre acceso para la visualización de árboles filogenéticos de alta calidad, como los reconstruidos con Phylip , Mega, Tree-Puzzle o Paup *. El programa también implementa algunas funcionalidades de manipulación de árboles, por ejemplo, la definición de grupos externos y el enraizamiento de árboles. Las versiones de programa disponibles para MacOsX y PC utilizan interfaces casi idénticas. FigTree es una aplicación gratuita para visualización y edición sofisticada de árboles filogenéticos. Los árboles pueden exportarse en formato PDF para obtener cifras de calidad de publicación o guardarse en formato nexus con la información de edición incluida como un bloque FigTree. El programa está escrito en JAVA y tanto los ejecutables de MacOSX como de Windows se pueden descargar desde http://tree.bio.ed.ac.uk/software/figtree/. El programa Mega, también contiene un módulo incorporado para mostrar y manipular árboles filogenéticos. 

Los árboles filogenéticos casi siempre se guardan en uno de dos formatos: NEWICK o NEXUS. El estándar NEWICK para un formato de árbol legible por computadora hace uso de la correspondencia entre árboles y paréntesis anidados; En la figura 1 se muestra un ejemplo de un árbol de cuatro taxones. En esta notación, un árbol es básicamente una cadena de pares de paréntesis balanceados con cada dos paréntesis balanceados que representan un nodo interno. Las longitudes de rama para ramas terminales y nodos internos se escriben después de dos puntos. El formato NEXUS incorpora el formato NEWICK junto con otros comandos y, por lo general, tiene un bloque de definición de taxones separado. 

```
#NEXUS
         Begin trees;
            Translate
	1 A,
	2 B, 
	3 C, 
	4 D,
	;
tree PAUP_1 = [&U] ((1:0.1,2:0.2):0.2,(3:0.3,4:0.4)); 
End; 
```

Figura 1. Árbol hipotético sin raíces de cuatro taxones (A, B, C y D) con números a lo largo de las ramas que indican distancias genéticas estimadas y su descripción en formato NEWICK.
{: .fs-1 .mx-auto }

## Inferencias basadas en distancias en el software PHYLIP

El paquete de software PHYLIP implementa cuatro métodos diferentes de construcción de árboles basados en la distancia: los métodos Neighbor-Joining (NJ) y UPGMA, ejecutados por el programa Neighbor.exe; el método Fitch – Margoliash, realizado por el programa Fitch.exe; y el método Fitch y Margoliash suponiendo un reloj molecular, llevado a cabo por el programa Kitch.exe. El método UPGMA y el algoritmo implementado en el programa Kitch.exe suponen la ultrametricidad de las secuencias en el conjunto de datos, es decir, que las secuencias son contemporáneas y acumulan mutaciones a lo largo del tiempo a un ritmo más o menos constante. Como se discutió anteriormente, los métodos ultramétricos tienden a producir árboles filogenéticos menos confiables cuando las mutaciones ocurren a tasas significativamente diferentes en diferentes linajes.

Los métodos no ultramétricos, como NJ o Fitch-Margoliash, no asumen un reloj molecular y son mejores para recuperar la filogenia correcta en situaciones en las que diferentes linajes exhiben una fuerte heterogeneidad en las tasas evolutivas. Sin embargo, la evaluación estadística del reloj molecular y el modelo de sustitución que mejor se ajustan a los datos requieren el conocimiento de la topología del árbol que relaciona las unidades taxonómicas operativas (UTO, es decir, los taxones) bajo investigación. Por lo tanto, el primer paso en los estudios filogenéticos generalmente consiste en construir árboles usando un modelo evolutivo simple, como el modelo JC69 o el modelo Kimura de 2 parámetros (Kimura, 1980), y algoritmos de construcción de árboles que no suponen un reloj molecular. La confiabilidad de cada clado en el árbol se prueba luego con análisis bootstrap o Jackknifing. De esta manera, es posible inferir uno o más árboles que, aunque no necesariamente son la verdadera filogenia, son hipótesis razonables para los datos. Tales árboles "aproximados" son usualmente apropiados para probar una variedad de hipótesis evolutivas usando métodos de máxima verosimilitud, incluyendo el modelo de sustitución de nucleótidos y el reloj molecular. Además, cuando se conoce una topología "razonable", los parámetros libres de cualquier modelo, por ejemplo, la relación de transición / transversión o el parámetro de forma α de la distribución Γ, pueden estimarse a partir de conjunto de datos por métodos de máxima verosimilitud. 

A continuación, utilizaremos las versiones de PHYLIP, MEGA, TreeView y FigTree. 

Describan los resultados entre los dos métodos UPGMA y NJ. ¿hay conflictos entre ambas inferencias?

Que diferencias hay entre el modelo JC69 y el modelo Kimura de 2 parámetros

De qué manera bootstrap o Jackknifing nos dan soportes de nuestras topologías, que otras medidas de soporte existen. 
