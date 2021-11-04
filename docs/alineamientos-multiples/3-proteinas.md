---
layout: default
title: Secuencias de aminoacidos
parent: Alineamientos Múltiples
permalink: /alineamientos-multiples/proteinas
nav_order: 3
---

Alineamiento de proteínas al de nucleótidos 
{: .fs-9 	.text-purple-000 .fw-300}

Los programas de alineamiento múltiple que se han mencionado generalmente rompen el marco de lectura cuando se alinean secuencias de nucleótidos. Esto invalidaría, por ejemplo, análisis posteriores basados en codones, y necesitarían de una buena dosis de edición manual para restaurar los marcos de lectura. Para evitar esto, podemos usar el alineamiento basado en las secuencias de proteínas para generar el alineamiento correspondiente de nucleótidos. Este procedimiento también tiene la ventaja de que los alineamientos de proteínas son menos ambiguos y mas rápidos de calcular. 

¿Porqué son más rápidos de calcularlos?
{: .fs-4 	 .fw-300 	.text-center}

Vamos a crear el alineamiento de las secuencias de ADN de usando la herramienta RevTrans (Wernersson and Pedersen, 2003). Siga el enlace http://www.cbs.dtu.dk/services/RevTrans/ y cargue el archivo con las secuencias de nucleótidos y uno de los alineamientos de proteínas. Revise que la opción Match DNA and peptide sequences by sea igual a Name. 

¿Qué característica tienen los gaps en el alineamiento de las secuencias de ADN?
{: .fs-4 	 .fw-300 	.text-center}
