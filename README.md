# Automated-Data-Query
Objective:
The objective of this project is to build an intelligent, automated data query and retrieval system that allows users to ask natural language questions about tabular data (CSV), have those questions converted to executable MongoDB queries using an offline, open-source Large Language Model (LLM), and then display or save the results of those queries.

Key Features:
CSV Data Ingestion:
Automatically loads and stores each row of a CSV file into a MongoDB collection.

Offline LLM Query Generation:
Uses a locally running, free and open-source language model (e.g., GPT4All or LLaMA2 via LangChain) to translate user questions into MongoDB queries without requiring any internet access or external API calls.

Dynamic Query Execution:
Executes the generated MongoDB queries to retrieve relevant data directly from the database.

Flexible Output Options:
Provides users with the option to either:

Display the results in a human-readable table, or

Save the output as a new CSV file.

Secure and Offline:
Fully offline operation ensures data privacy and eliminates dependency on cloud services or paid APIs.

User-Friendly Interaction:
A simple command-line interface allows users to load data, ask queries, and manage outputs seamlessly.

Robust Error Handling:
Handles various edge cases such as:

Invalid column names or malformed questions

Syntax errors in LLM-generated queries

MongoDB connection issues or empty query results

Technologies Used:
Python

MongoDB

LangChain

GPT4All / LLaMA2 (Offline LLMs)

Pandas

Scalability & Efficiency Considerations:
Efficiently handles large CSV files by batch inserting into MongoDB.

Can be extended to support multiple CSV uploads and more advanced query understanding.

Modular design makes it easy to switch LLM models or plug in a GUI later.

Deliverables:
End-to-End Python Script to perform all major steps (load → query → retrieve → display/save).

Modular Scripts for CSV ingestion, query generation, and data output.

README File with installation, usage, and system overview.

Test Cases including sample inputs, queries, and outputs.

Query Logs saved in queries_generated.txt.
