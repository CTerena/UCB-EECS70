## 1.Grpah Threory: An Introduction  
One of the fundamental ideas in computer science is the notion of *abstraction*: capturing the essence or the core of some complex situation by a simple model.  

In some large and complex entities, there are underlying "network" or *graph* that captures the important features that help us understand these entities more deeply.  

In the case of the internet, this networkk or graph specifies how web pages link to one another. In the case of the brain, it's the interconnection network between neurons.  

We can describe these ideas in the beautiful framework of *graph theory*. And Leonhard Euler is hailed as the inventor of graph theory.  

## 2.Formal definition 
Formally, a(undirected) graph is deined by a set of vertices $V$ and a set of edges $E$. For a simple example, $V$={$A$,$B$,$C$,$D$} and $E$={{$A$,$B$},{$A$,$C$},{$B$,$C$},{$B$,$D$},{$C$,$D$}}.   
Between any pair of vertices there is either 0 or 1 edge. If there are multiple edges between a pair of vertices, then we collapse them into a single edge.  
More generally, we also define directed graphs, where each edge has a *direction* specified by an arrow. Such graphs are useful in modeling one-way relationships, such as one-way streets between two locations, and are called *directed*. On the other hand, if each edge goes in both directions, then we call the graph *undirected*. For simplicity, we omit the arrowheads when drawing edges in undirected graphs.  

We conclude that a graph is thus formally specified as an ordered pair $G = (V,E)$, where $V$ is the vertex set and $E$ is the edge set.   

*degree(u)* = $|{v\in V:{u,v}\in E}|$.  

A vertex *u* whose degree is 0 is called an *isolated* vertex, since there is no edge which connects *u* to the rest of the graph.  

A directed graph, on the other hand, has two different notions of degree due to the directions on the edges. Specifically, the *in-degree( of a vertex *u* is the number of edges from other vertices to *u*, and the *out-degree* of *u* is the number of edges from *u* to other vertices.  

Finally, our definition of a graph thus far allows edges of the form ${u, u}$, called *self-loop*.  

**Path**: a *path* in a graph is a sequence of edges {$v_1$, $v_2$}, {$v_2$, $v_3$},...,{$v_{n-2}$, $v_{n-1}$},{$v_{n-1}$,$v_n$}$. In this case we say that there is a path *between v_1 and v_n*.  
**Cycle**:a *cycle* is a sequence of edges ${$v_1$, $v_2$}, {$v_2$, $v_3$},...,{$v_{n-2}$, $v_{n-1}$},{$v_{n-1}$,$v_n$},{$v_n$, $v_1$}$, where $v_1,...,v_n$ are distinct.  
**Walk**: a sequence of edges with repeated vertices.  
**Tour**: a walk which starts and ends at the same vertex.  
**Connectivity**: A graph is said to be *connected* if there's a path between any two distinct vertices.  
Note that *any* graph always consists of a collection of *connected components*.  

Euler's Theorem(1736): *An undirected graph G = (V,E) has an Eulerian tour iff G is even degree, and connected(except possibly for isolaated verices)*   

**Tree**: A graph is a *tree* if it's connected and acyclic. Another definition: a connected graph where the number of vertices is one more than the number of edges. Or, a connected graph that if you delete any edge it becomes disconnected.  
**Planar Graphs**: A graph is *planar* if it can be possibly drawn on the plane without crossings.      
**Face**: the faces are the regions into which the graph subdivides the plane, denoted $f$.  
One basic and important fact about planar graphs is *Euler's formula*, $v+f=e+2$.  
