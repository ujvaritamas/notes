# Knowledge graph

[Enhancing RAG-based application accuracy by constructing and leveraging knowledge graphs](https://blog.langchain.com/enhancing-rag-based-applications-accuracy-by-constructing-and-leveraging-knowledge-graphs/)

LLMs, with their profound understanding of language and context, can automate significant parts of the knowledge graph creation process.

Knowledge graphs enhance RAG by enabling multi hop reasoning, relationship aware retrieval and better explainability.
It extracts entities and relations from text, stores them in a graph and uses them with LLMs to generate accurate answers.

Extraction
- LLMGraphTransformer: Uses an LLM to extract entities and relationships from text.
- Schema Definition: Defines what types of nodes and relationships are allowed to ensure consistency.
- Pydantic Models: Provides a structured format for nodes and edges, guiding the LLM on what to extract.
- Property Extraction: The LLM can also attach properties like dates, attributes, etc to enrich nodes and relationships.