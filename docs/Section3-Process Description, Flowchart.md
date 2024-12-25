# Process Description

<img src="../assets/flowchart.png" alt="RAG Process" width="" />

### Split

RAG starts by converting structured or unstructured documents into plain text and then breaking the text into smaller segments, or chunks, for easier processing.

### Embed Documents

A text embedding model processes each chunk, transforming it into a vector that captures its semantic meaning.

### VectorDB

These vectors are stored in a vector database, which serves as the foundation for efficient data retrieval.

### Retrieval

When a user submits a query, the vector database quickly identifies and retrieves the chunks most relevant to the query.

### Response Generation

The large language model (LLM) synthesizes the retrieved chunks to produce a coherent and informative response.
