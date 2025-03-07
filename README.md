# NP-Completo

## Historia y Contexto

El concepto de **NP-completo** fue introducido en 1971 por **Stephen Cook** en su famoso **Teorema de Cook**, donde demostró que el problema **SAT** (Satisfacción Booleana) es NP-completo. A partir de este resultado, otros problemas fueron demostrados como NP-completos mediante **reducciones polinómicas**.

Los problemas NP-completos son relevantes porque aparecen en muchas aplicaciones prácticas y teóricas. Se cree ampliamente que **P ≠ NP**, lo que implica que no existen soluciones eficientes para estos problemas en el peor caso, aunque aún no se ha demostrado formalmente.

![Stephen Cook](https://upload.wikimedia.org/wikipedia/commons/6/68/Prof.Cook.jpg)

---

## Definición de NP-Completitud

Un problema se considera **NP-completo** si cumple dos condiciones:

1. **Pertenencia a NP**: Se puede verificar una solución dada en tiempo polinómico.
2. **NP-duro**: Cualquier otro problema en NP puede ser reducido a este problema en tiempo polinómico.

Los problemas **NP-duros** (también llamados **NP-hard**) son aquellos al menos tan difíciles como los problemas más difíciles de NP, pero no necesariamente pertenecen a NP.

Si se encontrara un algoritmo polinómico para resolver cualquier problema NP-completo, significaría que **P = NP**, lo que implicaría que todos los problemas en NP pueden resolverse eficientemente.

--
## Conceptos Claves

### **Tiempo Polinómico**
El tiempo polinómico se refiere al tiempo en que un algoritmo computacional resuelve un problema. Se dice que un algoritmo tiene tiempo polinomial si su complejidad es \( O(n^k) \), donde:

- \( n \) es el tamaño de la entrada.
- \( k \) es una constante.

---

## Importancia de los Problemas NP-Completos

El estudio de los problemas NP-completos es clave en la computación teórica y aplicada. Dado que no existe (hasta ahora) una solución eficiente para estos problemas en todos los casos, se han desarrollado diversas estrategias para enfrentarlos:

- **Algoritmos aproximados**: Proporcionan soluciones cercanas a la óptima en un tiempo razonable.
- **Algoritmos heurísticos**: Estrategias como búsqueda local, algoritmos genéticos y redes neuronales pueden ofrecer soluciones aceptables en muchos casos.
- **Algoritmos de programación dinámica o backtracking**: Para instancias pequeñas, estos métodos pueden ser efectivos.
- **Reducciones y transformaciones**: Para demostrar que un nuevo problema es NP-completo, se reduce a otro ya conocido.

---

## Clases de Complejidad

### **P (Tiempo Polinómico)**
P es el conjunto de problemas de decisión que pueden ser resueltos en tiempo polinómico por una **Máquina de Turing determinista**. 

Ejemplo: El problema del **camino más corto** en un grafo ponderado con pesos no negativos se resuelve en tiempo polinomial mediante el **algoritmo de Dijkstra**.

### **NP (Tiempo No Determinista Polinómico)**
NP es el conjunto de problemas de decisión cuyas soluciones pueden ser **verificadas** en tiempo polinómico por una **Máquina de Turing determinista**.

Ejemplo: La **factorización de números enteros** es un problema NP porque, dado un conjunto de factores candidatos, podemos verificar en tiempo polinómico si son correctos.

### **NP-Hard (NP-Duro)**
Es el conjunto de problemas al menos tan difíciles como los problemas más difíciles de NP. Un problema es NP-Hard si **todos los problemas en NP pueden ser reducidos a él en tiempo polinómico**. 

### **NP-Complete (NP-Completo)**
Un problema es NP-completo si **pertenece a NP** y es **NP-duro**. Algunos ejemplos conocidos de problemas NP-completos incluyen:

- **3-SAT** (Satisfacción Booleana)
- **Problema de la Mochila (Knapsack Problem)**
- **Problema del Camino Hamiltoniano (Hamiltonian Path)**

![P, NP, NP-COMPLETO](https://upload.wikimedia.org/wikipedia/commons/thumb/7/79/Complexity_classes_es.svg/260px-Complexity_classes_es.svg.png)

---

## Reducciones y Transformaciones

Las **reducciones** son técnicas fundamentales en la teoría de la computación, ya que permiten demostrar que un problema es NP-completo transformándolo en otro problema ya conocido de esta clase.

Algunas propiedades clave de las reducciones:

- **Transforman instancias de un problema en instancias de otro problema.**
- **Mantienen la validez de las soluciones** (instancias positivas y negativas).
- **Permiten comparar la complejidad de distintos problemas**.

Ejemplo: Para demostrar que un problema \(X\) es NP-completo, se puede reducir un problema ya conocido como **3-SAT** al problema \(X\) en tiempo polinómico.

---

## Relación con P vs NP

La pregunta central de la teoría de la complejidad es si **P = NP**, es decir, si los problemas cuya solución puede verificarse en tiempo polinómico también pueden resolverse en tiempo polinómico. 

Si **P = NP**, todos los problemas en NP podrían resolverse en tiempo polinómico. Esto tendría un impacto enorme en la informática, la criptografía y muchas otras áreas.

Si **P ≠ NP**, significaría que existen problemas en NP que pueden verificarse en tiempo polinómico pero no resolverse eficientemente.

---

## Conclusión

Los problemas NP-completos representan el núcleo de los problemas computacionalmente difíciles. Aunque aún no se sabe si existen soluciones eficientes para todos ellos, su estudio ha dado lugar a importantes avances en **algoritmos, optimización y teoría de la computación**.

