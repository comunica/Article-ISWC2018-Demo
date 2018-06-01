## Comunica
{:#comunica}

[Comunica](cite:cites comunica) is a modular meta engine
that enables instantiation of specific engines with the functionality described by the modules
through semantic configuration files.
We released [80+ modules](https://github.com/comunica/comunica){:.mandatory}
that can be combined to fully replicate all features of the original
[TPF client](https://github.com/LinkedDataFragments/Client.js){:.mandatory}.
Comunica is not limited to simply solving SPARQL queries:
new modules can be added to solve new problems and add additional features.
Similarly, existing functionality can easily be switched out for others
to quickly compare different implementations and ideas.

Every module consists of two parts: the source code and its semantic description.
The second part is a collection of Linked Data documents
describing the functionality of the corresponding module.
These are used by the [Components.js](cite:cites componentsjs)
dependency injection framework
to instantiate and link all modules together.

The current collection of Comunica modules offers more functionality than the original TPF client.
The [default configuration](https://github.com/comunica/comunica/blob/master/packages/actor-init-sparql/config/config-default.json)
allows users to query different kinds of Linked Data besides TPF interfaces.
We provide support for SPARQL endpoints, Linked Data documents and [HDT](cite:cites hdt) files.
These can all be combined in a single federated query
by making use of the federated TPF algorithm
and using Comunica modules to allow triple pattern queries on those different source types.
