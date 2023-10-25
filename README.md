[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12577995&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Informally:
By the definition of isomorphism, for each node in one graph, the other graph must have a corresponding node. If the number of nodes is not the same, then in the graph with more nodes, some of its nodes will not have corresponding nodes in the other graph.

Formally:
Consider two graphs, $G_1=(V_1 , E_1)$ and $G_2=(V_2 , E_2)$, where the number of nodes in $V_2 > V_1$. Now, assume these graphs are isomorphic.
If these graphs are isomorphic, that means there exists a one-to-one and onto function  $f: V_1 \rightarrow V_2$ such that $(u,v) \in E_1$ iff $(f(u),f(v)) \in E_2$.
Since $f$ is onto, for each node in $V_1$, it must map to a node $V_2$. Since $f$ is a function, it cannot map to multiple values in $V_2$. However, there are more nodes in $V_2$ than $V_1$, so not all nodes in $V_2$ correspond to a node in $V_1$, so f is not onto.
This is a contradiction, so the assumption that these two graphs are isomorphic must be incorrect.
Similarly, as if the number of nodes in $V_2 < V_1$, the function $f$ is not one-to-one, because you would have to assign multiple nodes in $V_1$ to at least one node in $V_2$, which violates the definition of one-to-one.
Therefore, if two graphs do not have the same number of nodes, they cannot be isomorphic.



# References
Used this to quickly review what one-to-one and onto meant in this context
https://testbook.com/maths/one-to-one-and-onto-function#:~:text=Define%20one%2Dto%2Done%20and,one%20element%20in%20the%20domain