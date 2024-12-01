# Amazon & Neo4j AI: Document Data (Commercial Contracts)

Demonstrates how to build agentic AI apps on top of documents with repeated lexical structure - i.e. documents sharing similar hierarchical/section structure, components, and/or conceptual breakdown.  Applicable to documents like legal contracts, product catalogs, user manuals and more. This example uses commercial contracts to demonstrate.

- The file [ingest-mixed-struct-finserv.ipynb](ingest-mixed-struct-finserv.ipynb) loads the data into Neo4j to use for retrieval. 

- See the [genai-app module](genai-app) for running an example AI app that leverages GraphRAG. __Warning:__ The current application requires AuraDS which is another deployment of the Neo4j database that uses graph analytics. Ruynning on AuraDB will result inan error about "GDS" not being found.  We hope to refactor a version that doesn't require AuraDS in the near future. 