---
layout: default
title: Formatos
parent: Alineamientos Múltiples
nav_order: 1
---

Formatos de secuencias 
{: .fs-9 	.text-purple-000 .fw-300}

Existen diferentes formatos para secuencias, generalmente en texto plano. Lo que significa que se pueden ver y editar con cualquier editor de texto, como Atom, Textwrangler, vi o pico. Algunos de estos formatos son más comunes que otros y muchos programas de bioinformática aceptan varios de los formatos más comunes (Leonard et al., 2007). Todos los formatos de secuencias tienen una característica (campo) en común: un identificador para cada secuencia. De forma que esta pueda ser reconocida de forma unívoca. 
{: .fs-6 .fw-300 }


## Fasta 

Es el formato más sencillo es conocido como Fasta1. En el cual una entrada, secuencia, se puede dividir en dos partes: La línea de identificación, que debe comenzar con el símbolo “>” y seguida inmediatamente del identificador de la secuencia (Ver línea 103), que puede ser cualquier cadena de caracteres sin espacios. Las líneas inmediatamente después del identificador corresponden a la secuencia propiamente dicha (Líneas 104-110). Fasta es el formato de secuencias más comúnmente usado en aplicaciones bioinformáticas.

Figura 1. Ejemplo de secuencia en formato Fasta
{: .fs-1 .mx-auto }

## GenBank

El formato GenBank2,3 es usado por el “National Center for Biotechnology Information” (NCBI), el mayor repositorio de secuencias, tanto de ácidos nucleicos como de proteínas, a nivel mundial. El NCBI junto con el, EMBL15 y el DDBJ16, mantienen en forma conjunta “The International Nucleotide Sequence Database” (Mizrachi, 2008). Una entrada en este formato está compuesta por dos partes. La primera parte consiste de las posiciones 1 a 10, y generalmente contiene el nombre del campo, e.g., LOCUS, DEFINITION, ACCESSION o SOURCE. La segunda parte de cada entrada contiene la información para el campo correspondiente. Cada entrada termina con el símbolo “\\” (Línea 173). Pueden encontrar más información sobre este tipo de archivo siguiendo el enlace http://www.ncbi.nlm.nih.gov/ Sitemap/samplerecord.html 

Figura 2. Ejemplo de secuencia en formato GenBank
{: .fs-1 .mx-auto }
