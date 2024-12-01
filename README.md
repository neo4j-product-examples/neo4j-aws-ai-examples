# Amazon Web Services & Neo4j AI Use Cases

This repository contains worked examples for ai applications with different source data types and use cases.  Examples leverage Amazon Bedrock. 

1. [Mixed Structured Data (Finserv)](mixed-data-finserv): Demonstrates how to build an AI apps on top of mixed data - where documents are connected by structured data. This is akin to structured tables linking to unstructured text fields. Leverages United States Security & Exchange Commission (SEC) company filings data.  Semi-structured data comes from form13 Asset manager ownership data while unstructured text comes from  form10k sections. 
2. [Document Data (Commercial Contracts)](document-data-contracts): Demonstrates how to build agentic AI apps on top of documents with repeated lexical structure - i.e. documents sharing similar hierarchical/section structure, components, and/or conceptual breakdown.  Applicable to documents like legal contracts, product catalogs, user manuals and more. This example uses commercial contracts to demonstrate.  
3. [Unstructured Text Data (Medical Research)](unstructured-data-medical): Demonstrates how to build AI apps on top of highly unstructured text documents. Leveraged Named Entity Recognition (NER) to build a knowledge graph for GraphRAG. Applicable to some forms of internal documentation,research papers, and other text where this no consistent structure. Leverages Named Entity Recognition (NER) to build a knowledge graph. 

## Prerequisites for All Examples

1. Follow this [guide](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/quickstart.html#configuration) to configure your environment to use the Bedrock API. 
2. Install `requirements.txt`