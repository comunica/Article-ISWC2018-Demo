## Abstract
<!-- Context      -->
Linked Data sources can appear in a variety of forms,
going from SPARQL endpoints to Triple Pattern Fragments and data dumps.
<!-- Need         -->
This creates an added layer of complexity when querying or combining results from those sources.
<!-- Task         -->
To ease this problem, we created a modular client, Comunica,
that has modules for solving SPARQL queries and supports heterogeneous interfaces.
Other modules for other query or source types can easily be added.
<!-- Object       -->
In this paper we showcase the web client that uses Comunica to solve federated SPARQL queries
and can automatically detect the types of the sources covered.
