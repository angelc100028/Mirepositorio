
# Estructura de un Grafo #
¡Hola! Para crear una estructura de código para un grafo en C++, puedes utilizar la clase `Graph` de la biblioteca Boost Graph Library (BGL) ¹. La BGL es una biblioteca de gráficos de C++ que proporciona estructuras de datos y algoritmos para trabajar con gráficos.

Aquí hay un ejemplo de cómo crear un grafo no dirigido utilizando la clase **`Graph`** de BGL:

```
#include <boost/graph/adjacency_list.hpp>
#include <iostream>

using namespace boost;

int main()
{
    // Define the graph type
    typedef adjacency_list<vecS, vecS, undirectedS> Graph;

    // Create a graph object
    Graph g;

    // Add vertices to the graph
    add_vertex(g);
    add_vertex(g);
    add_vertex(g);

    // Add edges to the graph
    add_edge(0, 1, g);
    add_edge(1, 2, g);

    // Print the number of vertices and edges in the graph
    std::cout << "Number of vertices: " << num_vertices(g) << std::endl;
    std::cout << "Number of edges: " << num_edges(g) << std::endl;

    return 0;
}
```

En este ejemplo, se crea un grafo no dirigido utilizando la clase `adjacency_list` de BGL. La plantilla `adjacency_list` toma tres argumentos: el tipo de almacenamiento del contenedor para los vértices, el tipo de almacenamiento del contenedor para los bordes y el tipo de gráfico (dirigido o no dirigido). En este caso, se utilizan vectores para almacenar los vértices y bordes y se crea un grafo no dirigido.

Luego, se agregan tres vértices al grafo utilizando la función `add_vertex()`. Después, se agregan dos bordes al grafo utilizando la función `add_edge()`. Finalmente, se imprime el número de vértices y bordes en el grafo utilizando las funciones `num_vertices()` y `num_edges()`.

Espero que esto te ayude. ¡Házmelo saber si tienes alguna otra pregunta!

Origen: Conversación con Bing, 12/10/2023
(1) Ejemplos de Grafo en C++ (Cpp) - HotExamples. https://cpp.hotexamples.com/es/examples/-/Grafo/-/cpp-grafo-class-examples.html.
(2) Que es un grafo en C++? – La-Respuesta.com. https://la-respuesta.com/consejos-utiles/que-es-un-grafo-en-c/.
(3) Código de Java - Grafo - La Web del Programador. https://www.lawebdelprogramador.com/codigo/Java/6589-Grafo.html.
(4) Implementación de gráficos en C++ (sin usar STL) - Techie Delight. https://www.techiedelight.com/es/graph-implementation-c-without-using-stl/.
(5) Explicación de algoritmos y estructuras de datos de grafos con Ejemplos .... https://www.freecodecamp.org/espanol/news/explicacion-de-algoritmos-y-estructuras-de-datos-de-grafos-con-ejemplos-en-java-y-c/.
