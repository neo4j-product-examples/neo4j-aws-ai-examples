# Amazon & Neo4j AI: Mixed Structured Data (Finserv)

Demonstrates how to build an AI apps on top of mixed data - where documents are connected by structured data. This is akin to structured tables linking to unstructured text fields. Leverages United States Security & Exchange Commission (SEC) company filings data.  Semi-structured data comes from form13 Asset manager ownership data while unstructured text comes from  form10k sections.

This project is based off the work from this [blog](https://neo4j.com/developer-blog/graphrag-in-action/). It has been adjusted here to demonstrate Amazon Bedrock integration. 

## Steps to Run End-to-End

1. See configuration prerequisites from the [main README.md](../README.md)
2. Create a Neo4j database.  Easiest to do through [AuraDB Pro free trial](https://aws.amazon.com/marketplace/pp/prodview-2t3o7mnw5ypee).
3. Create and fill in a `cred.env` file using [cred.env.template](cred.env.template) as a template
4. Run [extract-pdf-to-json.ipynb](extract-pdf-to-json.ipynb) to create extracted, structured, json data
5. Run [ingest-json-to-graph.ipynb](ingest-json-to-graph.ipynb) to ingest into Neo4j
6. In terminal run `export $(grep -v ^# cred.env | xargs)`
7. Run the agent with `python test_agent.py`

