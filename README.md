# Reducing Hallucinations in Large Language Models Using Retrieval-Augmented Generation

This project investigates techniques for reducing hallucinations in Large Language Models (LLMs) by incorporating Retrieval-Augmented Generation (RAG) pipelines. The project evaluates how different retrieval and processing strategies impact the factual accuracy, relevance, and reliability of model-generated responses.

A baseline LLM was first evaluated to establish its tendency to generate unsupported or incorrect information. An enhanced RAG architecture was then developed using two key strategies, and the overall model compared against the baseline:

* **Pre-Processed RAG:** Improves retrieval quality through document preprocessing, chunk optimization, cleaning, and indexing before information is supplied to the language model.
* **Post-Processed RAG:** Applies validation and refinement techniques after generation to verify responses and reduce factual inconsistencies.

The reliability metrics included scoring past a certain threshold based on the authenticity, recency, accuracy, relevancy, and various other metrics. An algorithm to expand on the search results was also implemented in the case that the primary search gave no results.

The system first determines whether retrieval is necessary or its own expertise would suffice. If required, it retrieves relevant information from scientifically backed websites like NIH and PubMed, and other .org and .edu pages, and grounds model responses in retrieved evidence, reducing reliance on the model's parametric memory. Performance was assessed using quantitative and qualitative evaluation metrics, including response accuracy, hallucination rate, contextual relevance, and answer completeness.

## Technologies and Tools

* Python
* Large Language Models (LLMs)
* Retrieval-Augmented Generation (RAG)
* Vector Databases and Embedding Models
* Information Retrieval Techniques
* Evaluation Frameworks for LLM Performance

## Results

The study demonstrates that integrating external knowledge retrieval significantly improves response reliability and reduces hallucinated content compared to the baseline model. Comparative analysis highlights the strengths and limitations of both pre-processing and post-processing RAG approaches, providing insights into effective strategies for building more trustworthy AI systems.

## Research Focus

This project contributes to ongoing research in trustworthy AI, factuality enhancement, and knowledge-grounded language generation by exploring practical methods for improving the accuracy and dependability of LLM outputs.
