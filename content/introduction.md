## Introduction
{:#introduction}

Add sources
{:.todo}

There are a multitude of ways we can access Linked Data these days.
Some of the more commonly used ones are SPARQL endpoints, 
Triple Pattern Fragments and its variations, subject pages and data dumps.
These all have their own methods on how they can be accessed and help solve SPARQL queries.
While a SPARQL endpoint can solve queries on its own,
data dumps will require client-side processing to produce more granular results.
This is measured in client cost on the Linked Data Fragments axis.

Having all these heterogeneous interfaces greatly complicates federated queries.
While resolving such a query,
different actions have to be taken depending on the source that is being accessed.
Different solutions might also be required depending on the combination of sources.
In case of a single SPARQL endpoint, a single query will suffice.
On the other hand, if all sources are data dumps they all have to be downloaded and parsed client-side.
But what if some sources are SPARQL endpoints and some are data dumps?

To this end we created a modular Linked Data client called [Comunica](cite:cites comunica).
In our ISWC 2018 article we describe how this client can easily be extended
to support a variety of sources and algorithms.
This allows everyone to quickly set up a federated SPARQL client
without having to worry about the sources,
and to easily extend it should more types be required.

In this paper we describe how we will showcase the heterogeneous features of Comunica.
We created a web client capable of solving federated SPARQL queries over heteregeneous interfaces.
Additionally, this client will automatically identify the type of all sources.
This way the end-user only has to provide the URLs and query;
Comunica will take care of the rest.