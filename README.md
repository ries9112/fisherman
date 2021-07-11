# fisherman
This is an R package which provides a blueprint for doing automated unit tests to verify the legitimacy of queries being served by an indexer.

A subgraph can have data be served by many indexers, and anyone can act as a "fisherman" who submit proof of the data being served by a given indexer being innacurate, and are then given a reward from the funds the indexer has slashed.

This package aims to provide a simple framework to enable anyone to setup an automated test to compare data from different indexers of the same subgraph for the same queries.
