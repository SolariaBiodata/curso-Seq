---
![alt text](https://solariabiodata.com.mx/images/solaria_banner.png "Soluciones de Siguiente Generación")
# Curso Online de Análisis de Secuencias
## Sesión 02

### Descripción
En esta sesión haremos algunos ejercicios prácticos sobre lo revisado durante la sesión de presentación
### Requisitos

Para poder realizar este ejercicio, necesitaremos:

1. Programas Instalados:
    - Chromas v2.6.6
    - BioEdit v7.2.5
> Los instaladores, se encuentran en la carpeta compartida o bien, puedes descargarlos directo de cualquier buscador web

2. Archivos de secuenciación
    - 8_160_FWD.ab1
    - 8_160_RWD.ab1
> Los archivos, se encuentran en la carpeta compartida, por favor descárgalos a tu computadora

## 1. Edición de secuencias Sanger con Chromas
### Descripción
En este ejercicio, vamos a realizar una edición sencilla de una secuencia (FWD y RWD) obtenida de un secuenciador Sanger

1. Abrir 2 programas Chromas y dividirlos a la mitad de la pantalla de forma horizontal
2. En uno de las ventanas, dar click en ``Open`` y cargar el archivo ``8_160_FWD.ab1``
3. En la otra ventana, dar click en ``Open`` y cargar el archivo ``8_160_RWD.ab1``
4. En la ventana donde está el archivo ``8_160_FWD.ab1`` dar click en el botón de ``Reverse``

###  1.1 Edición de secuencias

1. Buscar una región donde los electroferográmas se vean con buenas calidades en la ventana con el archivo ``8_160_FWD.ab1``
2. En la segunda ventana, dar click en ``Find`` e ingresar de forma manual la secuencia antes encontrada
3. Emparejar los electroferogramas y empezar a revisar ambos hacia el lado izquierdo de la pantalla
4. Realizar las ediciones necesarias a criterio de cada uno.
> Es recomendable hacer las menos ediciones posibles y realizarlas basados en la calidad de la base secuenciada así como en su contraparte en la otra secuencia.
5. Una vez terminado el lado izquierdo, continuar con el proceso hacia el lado derecho hasta el final de ambas secuencias

###  1.2 Extracción de secuencias

1. Al terminar la edición, dar click en la primer ventana en ``Edit > Copy Sequence > Plain Text``
2. Abir un bloc de notas y colocar como header ``>8FWD`` y en la linea siguiente, pegar la secuencia copiada
3. En la segunda ventana de Chromas, realizar el mismo procedimiento para copiar la secuencia
4. En el mismo bloc de notas, colocar como segundo header ``>8RWD`` y en la linea siguiente, pegar la segunda secuencia copiada
5. Guardar el archivo como  ``Consenso8.fasta ``

###  1.3 Obtención de secuencia consenso

1. Abrir el programa BioEdit, dar click en  ``Open `` y cargar el archivo  ``Consenso8.fasta ``
2. Seleccionar con el mouse ambas secuencias del lado izquierdo de la pantalla
3. Dar click en el menú  `` Accesory Application  >  ClustalW Multiple Alignment``
4. En la ventana que abre, dar click en  `` Run ClustalW `` y esperar a que el programa termine
5. Una vez realizado el alineamiento, habilitar el botón  `` View conservation by plotting identities``
6. Identificar la región donde la secuencia es compartida y seleccionarla
7. Una vez seleccionada, dar click en el menú  ``Edit > Copy Sequence ``
> Ya tienes tu secuencia consenso en el portapapeles, puedes pegarla en un bloc de notas y guardarla o ir directo a BLAST

