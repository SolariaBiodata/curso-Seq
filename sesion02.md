---
permalink: /sesion02.html
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
    - SeqTrace v0.9.0
> Los instaladores, se encuentran en la carpeta compartida o bien, puedes descargarlos directo de cualquier buscador web

2. Archivos de secuenciación
    - 8_160_FWD.ab1
    - 8_160_RWD.ab1
> Los archivos, se encuentran en la carpeta compartida, por favor descárgalos a tu computadora

## 1. Edición de secuencias Sanger con Chromas
### Descripción
En este ejercicio, vamos a realizar una edición sencilla de una secuencia (FWD y RWD) obtenida de un secuenciador Sanger.

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

## 2. Edición de secuencias Sanger con SeqTrace
### Descripción
En este ejercicio, revisaremos algunas de las funcionalidades de SeqTrace para realizar secuencias consenso a partir de pares electroferogramas en un solo proyecto. La lógica de editar, y generar las secuencias es muy similar a Chromas.

### 2.1 Extracción del ejecutable
1. Posterior a la descarga del archivo zip de seqtrace, descomprimir en la ruta preferida de trabajo, ésta es indistinta.
2. Para ejecutar SeqTrace, hacer clic en el archivo ```seqtrace.exe```

### 2.2 Apertura de Proyecto y Carga de Archivos
1. Una vez abierto el programa de SeqTrace, ubicar el menú _File_ > _New Project_ o dar clic en el botón de 'hoja blanca' en la barra superior
2. En la ventana abierta, indicar la ubicación de los archivos ab1 en la computadora. Opcionalmente, se puede indicar la secuencia de primers si estos están disponibles. Finalmente, clic en aceptar.
3. Ubicar el menú _Traces_ > _Add trace file(s)_ y elegir todas las secuencias que se van a analizar. Finalmente, clic en aceptar.
4. Basándose en la nomenclatura para los primers F/R, indicar la orientación del electroferograma dependiendo del caso.
> En esta operación, debes asegurar que los electroferogramas vengan en pares, y que el primer Reverse sea el que tenga la flecha naranja invertida.

5. Por cada par de electroferogramas, repetir la siguiente indicación:
  - Seleccionar ambos juegos de Archivos
  - Acceder a _Traces_ > _Group selected forward/reverse files_
  - Indicar el nombre que tendrá este par de secuencias
6. Para comenzar la edición de secuencia, acceder a _Traces_ > _View selected trace file(s)_ o dar clic en el botón de la 'lupa' en la barra superior.

### 2.3 Edición de electroferogramas
1. Usa la barra de desplazamiento horizontal para explorar la concatenación de ambos.
2. Revisa los extremos para posibles disparidades entre los electroferogramas.
3. Para editar  una base o posición, dar clic derecho en la barra blanca debajo de los alineamientos por secuencia y clic en _Modify selected base(s)_
3. Para eliminar  una base o posición, dar clic derecho en la barra blanca debajo de los alineamientos por secuencia y clic en _Delete selected base(s)_
> Si necesitas borrar todas las ediciones, clic derecho y luego clic en _Recalculate working seq_

4. Para guardar cambios, ubica el menú _File_ > _Save working Sequence to project_ o dar clic en el botón de 'diskette' en la barra superior
5. Cierra la ventana para regresar a la ventana principal.

### 2.4 Exportación de Secuencias Consenso

1. Clic en el menu _Sequences_ > _Export sequences_ > _From all trace files_ o clic en el ícono de 'pirámide azul convirtiendose en esfera roja' en la barra superior
2. Indicar la ubicación y el nombre del archivo de exportación. Finalmente Clic en aceptar
3. Corroborar que las secuencias exportadas pueden encontrarse en la ubicación especificada.
