## Comunica
{:#comunica}

[Comunica](cite:cites comunica) is a modular meta engine: 
it uses modular dependency injection to set up an engine
with the functionality described by the modules.
Together with our initial publication we released
[80+ modules](https://github.com/comunica/comunica){:.mandatory}
that can be combined to fully replicate all features of the original
[TPF client](https://github.com/LinkedDataFragments/Client.js){:.mandatory}.
But Comunica is not limited to simply solving SPARQL queries:
new modules can always be added to solve new problems and add additional features.
Similarly, features can easily be switched out for others
to quickly compare different implementations and ideas.

Every module consists of two parts: the source code and the the components description.
The second part is a collection of Linked Data documents
describing the functionality of the corresponding module.
These then get used by [Components.js](cite:cites componentsjs),
a semantic dependency injection framework,
to link all modules together correctly.

The current collection of Comunica modules does more than simply clone the original TPF client though.
The [default configuration](https://github.com/comunica/comunica/blob/master/packages/actor-init-sparql/config/config-default.json)
allows users to query all kinds of Linked Data besides TPF interfaces.
There is also support for SPARQL endpoints, Linked Data documents and HDT files.
These can also all be combined in a single federated query
by making use of the federated TPF algorithm
and using Comunica modules to allow triple pattern queries on those different source types.