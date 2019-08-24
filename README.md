# Ejemplo Graphviz ABB

**Curso Estructuras de datos Seccion B Segundo semestre 2019** 

*Desarrollado por Aux de catedra Fernando Antonio Hernandez*



Los puntos mas importantes del archivo son los siguientes.

 - Configuracion del grafo
 - Configuracion del nodo
 - Forma declarar el nodo
 - Forma de enlazar el nodo

## Configurar el grafo

    rankdir=TB;
    graph [splines=ortho, nodesep=0.5];

 - La primer linea que es para que la imagen se expanda tanto para ambos lados, como tambien para arriba y abajo.
 - splines = ortho es para que decirle que las uniones trate que sean lineas rectas
 - nodesep = 0.5 es que tanto va a guardar su distancia un nodo de otro


## Configurar el nodo

    node [shape = record, style=filled, fillcolor=seashell2,width=0.7,height=0.2];
    

|Propiedad|Valor  |Descripcion|
|--|--|--|
|Shape|record|forma que tenda el nodo en este caso rectangular|
|style|filled|Le indicamos que tendra un color o esta conteniendo una imagen|
|fillcolor|seash112|Color que tendran todos los nodos, el valor puede ser hexadecimal
|width|0.7|Ancho del nodo
|height|0.2|Altura del nodo





## Forma de declarar del nodo

    nodo[ label ="<C0>|valor|<C1>"];
Donde:

 1.  C0 es el lado izquierdo pueden cambiarle el nombre
 2. C1 es el lado derecho pueden cambiarle el nombre
 3. Valor es el dato que tendremos que mostrar en el nodo 

## Forma de enlazar el nodo

    nodo:C0->nodoizquierdo;
    nodo:C1->nododerecho;
De esta manera enlazamos el nodo seguido de ":" y luego el lado del cual saldra la flecha


