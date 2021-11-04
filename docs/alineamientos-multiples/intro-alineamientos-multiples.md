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

## Referencias 
- Abascal, F., R. Zardoya, and D. Posada, 2005 ProtTest: selection of best-fit models of protein evolution. Bioinformatics 21: 2104–2105. 
- Edgar, R. C., 2004 Muscle: a multiple sequence alignment method with reduced time and space complexity. BMC Bioinformatics 5: 113. 
- Lemey, P., M. Salemi, and A.-M. Vandamme, editors, 2009 The Phylogenetic Handbook. Cam- bridge University Press. 
- Leonard, S. A., T. G. Littlejohn, and A. D. Baxevanis, 2007 Common file formats. Curr Protoc Bioinformatics Appendix 1: Appendix 1B. 
- Mizrachi, I. K., 2008 Managing sequence data. Methods Mol Biol 452: 3–27.
- Morgenstern B, Goel S, Sczyrba A, Dress A. AltAVisT: comparing alternative multiple sequence alignments. Bioinformatics. 2003 Feb 12;19(3):425-6.
- Notredame, C., D. G. Higgins, and J. Heringa, 2000 T-coffee: A novel method for fast and accurate multiple sequence alignment. J Mol Biol 302: 205–217. 
- Notredame, C., 2007 Recent evolutions of multiple sequence alignment algorithms. PLoS Comput Biol 3: e123. 
- Posada, D., 2006 Modeltest server: a web-based tool for the statistical selection of models of nucleotide substitution online. Nucleic Acids Res 34: W700–W703. 
- Posada, D., and K. Crandall, 1998 MODELTEST: testing the model of DNA substitution. Bioinformatics 14: 817–8. 
- Posada, D., and K. Crandall, 2001 Selecting models of nucleotide substitution: an application to human immunodeficiency virus 1 (HIV-1). Mol Biol Evol 18: 897–906. 
- Sawyer, S. L., L. I. Wu, M. Emerman, and H. S. Malik, 2005 Positive selection of primate trim5alpha identifies a critical species-specific retroviral restriction domain. Proc Natl Acad Sci U S A 102: 2832–2837. 
- Sullivan, J., and P. Joyce, 2005 MODEL SELECTION IN PHYLOGENETICS. Annual Review of Ecology, Evolution, and Systematics 36: 445–466. 
- Thompson, J. D., D. G. Higgins, and T. J. Gibson, 1994 CLUSTAL W: improving the sen- sitivity of progressive multiple sequence alignment through sequence weighting, position-specific gap penalties and weight matrix choice. Nucleic Acids Res 22: 4673–4680. 
- Wernersson, R., and A. G. Pedersen, 2003 Revtrans: Multiple alignment of coding dna from aligned amino acid sequences. Nucleic Acids Res 31: 3537–3539. 



