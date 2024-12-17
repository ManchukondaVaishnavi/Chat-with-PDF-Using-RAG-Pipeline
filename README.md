#CHAT-WITH-PDF-USING-RAG-PIPELINE

Overview

This repository implements a Retrieval-Augmented Generation (RAG) pipeline that allows users to interact with semi-structured data in multiple PDF files. The system extracts, chunks, embeds, and stores data from PDF files, enabling efficient retrieval and accurate responses to user queries.
Functional Requirements
 * Data Ingestion:
   * Extracts text and relevant structured information from PDF files.
   * Segments data into logical chunks.
   * Converts chunks into vector embeddings using a pre-trained embedding model.
   * Stores embeddings in a vector database for efficient similarity-based retrieval.
 * Query Handling:
   * Converts the user's natural language query into vector embeddings.
   * Performs a similarity search in the vector database to retrieve the most relevant chunks.
   * Passes the retrieved chunks to the LLM along with a prompt or agentic context to generate a detailed response.
 * Comparison Queries:
   * Identifies and extracts relevant terms or fields to compare across multiple PDF files.
   * Retrieves corresponding chunks from the vector database.
   * Processes and aggregates data for comparison.
   * Generates a structured response (e.g., tabular or bullet-point format).
 * Response Generation:
   * Uses the LLM with retrieval-augmented prompts to produce responses with exact values and context.
   * Ensures factuality by incorporating retrieved data directly into the response.
Example Data:
https://www.hunter.cuny.edu/dolciani/pdf_files/workshop-materials/mmc-presentations/tables-charts-and-graphs-with-examples-from.pdf
Example Tasks:
 * Extract accurate unemployment information based on type of degree input from page 2.
 * Extract tabular data from page 6.
Installation
 * Clone this repository.
 * Install required dependencies (e.g., pip install -r requirements.txt).
Usage
[Provide instructions on how to run the pipeline, including any command-line arguments or configuration files.]
Contributing
We welcome contributions to improve the RAG pipeline. Feel free to submit issues or pull requests.
License
This project is licensed under the [License Name] license.
Additional Tips
 * Clear Structure: Use headings and subheadings to organize your README.
 * Concise Explanations: Keep explanations clear and concise.
 * Code Examples: If applicable, provide code snippets to illustrate functionality.
 * Visuals: Consider using diagrams or flowcharts to explain complex processes.
 * Testing Instructions: Include instructions on how to test the pipeline.
 * Deployment Instructions: If applicable, provide instructions on how to deploy the pipeline.
