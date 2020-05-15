---
permalink: /sesion03.html
---
![alt text](https://solariabiodata.com.mx/images/solaria_banner.png "Soluciones de Siguiente Generación")
# Curso Online de Análisis de Secuencias - Sesión 03

## 1. Alineamiento Local
### Descripción
En este ejercicio veremos cómo utilizar los diferentes tipos de BLAST, utilizando la interfaz gráfica de nuestro navegador.

### Requisitos

Para poder realizar este ejercicio, necesitaremos:
1. Ingresar a la página de BLAST: [https://blast.ncbi.nlm.nih.gov/Blast.cgi](https://blast.ncbi.nlm.nih.gov/Blast.cgi)

### Ejercicio 1

1. Ingresar a NCBI y en la base de datos  `Nucleotide` y buscar el No. de Acceso: `NM_079602.5`
2. En el registro, buscar el No. de acceso de la proteína para la cual codifica
3. Ingresar a los diferentes BLAST y pegar la secuencia (NT o AA segú requiera el programa)

BLASTN: NT vs NT
BLASTP: P vs P
BLASTX: NT (antes los traduce) vs P
TBLASTN: P vs NT (antes los traduce).
TBLASTX: NT vs NT traduciendo todas las secuencias.

>Vamos a modificar algunas opciones del programa en general para todos los BLAST que hagamos

4. En la parte de `Database`, cambiar a `RefSeq mRNA` o `RefSeq Protein` según lo requiera el programa
5. En la sección de `Organism` colocar `Vertebrata (taxid:7742)`
6. Bajar en la ventana y dar click en `Algorithm Parameters`
7. Modificar `Max target sequences` al valor máximo (20000)

> Vamos a correr los 5 BLAST diferentes y esperar los resultados

### Ejercicio 2

## 2. Alineamiento Global

### Descripción
Repasaremos lo que hemos aprendido respecto a los métodos de alineamiento múltiple de secuencias, utilizando el algoritmo de alineamiento global con las secuencias  que ya hemos descargado previamente.

### Instrucciones (Parte 1)
1. Dirigirse a la herramienta de [ClustalW](https://www.ebi.ac.uk/Tools/msa/clustalo/)
2. Seleccionar el tipo de molécula a DNA.
3. Pegar el contenido del archivo de secuencias o cargarlo desde la ventana que se abre al dar clic en 'Examinar'.
4. Seleccionar el formato de salida a Pearson/FASTA.
5. Clic en el botón de 'Submit' y esperar a los resultados.
6. Descargar el alineamiento resultante dando clic derecho y 'Guardar Como... '
7. Daremos clic en el botón 'Result Viewers' y después en `MView`
8. Descargaremos también la visualización.

### Instrucciones (Parte 2)
1. Dirigirse a la herramienta de [MUSCLE](https://www.ebi.ac.uk/Tools/msa/muscle/)
2. Repetiremos los pasos 3 al 8 de la Parte 1 de este mismo ejercicio.

### Instrucciones (Parte 3)
1. Dirigirse a la herramienta de [MAFFT](https://www.ebi.ac.uk/Tools/msa/mafft/)
2. Repetiremos los pasos 3 al 8 de la Parte 1 de este mismo ejercicio.

### Instrucciones (Parte 4)
1. Dirigirse a la herramienta de [TCOFFEE](https://www.ebi.ac.uk/Tools/msa/tcoffee/)
2. Repetiremos los pasos 3 al 8 de la Parte 1 de este mismo ejercicio.
