## Abstract
<!-- Context      -->
Linked Data sources can appear in a variety of forms,
going from SPARQL endpoints to Triple Pattern Fragments and data dumps.
<!-- Need         -->
This heterogeneity among Linked Data sources creates an added layer of complexity
when querying or combining results from those sources.
<!-- Task         -->
To ease this problem, we created a modular engine, Comunica,
which has modules for evaluating SPARQL queries and supports heterogeneous interfaces.
Other modules for other query or source types can easily be added.
<!-- Object       -->
In this paper we showcase a Web client that uses Comunica to evaluate federated SPARQL queries
through automatic source type identification and interaction.
