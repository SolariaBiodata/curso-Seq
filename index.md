---
permalink: /index.html
---
![alt text](https://solariabiodata.com.mx/images/solaria_banner.png "Soluciones de Siguiente Generación")
# Curso Online de Análisis de Secuencias
## Sesión 01

### Descripción
En esta sesión haremos algunos ejercicios prácticos sobre lo revisado durante la sesión de presentación
### Requisitos

Para poder realizar este ejercicio, necesitaremos:

1. Datos de Ejemplo:
    - Puedes usar tus propios datos siguiente algunas recomendaciones de este tutorial
    - O puedes usar los datos del respositorio
2. Sofware Recomendable para esta sesión:
    - Navegador Web (Todas las Plataformas)
    - Editor de texto (Windows)



## 1. Bases de datos: NCBI
### Descripción
En este ejercicio veremos cómo accesar a diferentes repositorios de NCBI, utilizando la interfaz gráfica de nuestro navegador.

### Requisitos

Para poder realizar este ejercicio, necesitaremos:
1. Ingresar a la página de NCBI: [https://www.ncbi.nlm.nih.gov/](https://www.ncbi.nlm.nih.gov/)
2. Dar click en `Resource List (A-Z)`
>  El paso anterior nos desplegó una lista de todos los repositorios en NCBI que están disponibles para su consulta.
3. Abrir la Base de datos `Nucleotide`
4. Teclear `Influenza A virus` en el campo de búsqueda

### Ejercicio 1
### 1.1 Búsqueda Avanzada

1. Dar click en ``Advanced``
2. En el Builder, seleccionar ``Organism`` en la primer pestaña
3. Realizar nuevamente la búsqueda de ``Influenza A virus``

###  1.2 Dirigir la búsqueda a una región (o gen) de interés

1. Teclear ``Influenza A virus[Organism] AND human``
> Esta sigue siendo una búsqueda muy general, vamos a hacerla más específica
2. Dar click en ``Advanced``
3. En el historial de búsquedas, aparecen las más recientes, dar click en add en el primer registro
4. En el Builder, seleccionar ``Organism`` en la primer pestaña
5. Seleccionar ``Gene name ``en la segunda pestaña y teclear `` neuraminidase`` en su cuadro de diálogo
6. Realizar la búsqueda nuevamente
7. Añadir a la búsqueda ``AND complete`` para que el término final sea ``(Influenza A virus[Organism])AND human AND neuraminidase[Gene Name] AND complete``
8. Por último, en el menú lateral izquierdo, selecciona `` refseq``

#### Discusión
¿Cuantas secuencias resultaron al final de esta búsqueda específica?

### 1.3 Descarga de secuencias
1. Dar click en ``send to`` 
2. Dar click en ``File`` --> ``Format`` --> ``FASTA``  --> ``Create file``
3. Guardar las secuencias en tu computadora

>Ya tienes tu propia base de datos
