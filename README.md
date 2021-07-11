# fisherman
This is an R package which provides a blueprint for doing automated unit tests to verify the legitimacy of queries being served by an indexer on [The Graph](https://thegraph.com/).

A subgraph can have data be served by many indexers, and anyone can act as a "fisherman" who submit proof of the data being served by a given indexer being innacurate, and are then given a reward from the funds the indexer has slashed.

This package aims to provide a simple framework to enable anyone to setup an automated test to compare data from different indexers of the same subgraph for the same queries. 

## Framework
The idea is to create functions with automated tests that confirm the data from the different indexers is equivalent across the board, and throw an error if that is not the case, in order to provide detection around potential issues to take a look at and potentially [generate a dispute](https://www.youtube.com/watch?v=TuFx0-StM8o).
