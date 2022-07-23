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
