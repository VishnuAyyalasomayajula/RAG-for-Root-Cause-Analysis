This project explores the application of Retrieval-Augmented Generation (RAG) for root cause analysis in microservices environments. We transform datasets representing different traffic scenarios (low, high, temporary) and store them in Pinecone, a vector storage service, for efficient retrieval. A JSON file containing service dependencies and dependents is used to understand the microservices architecture. The goal is to use training datasets stored in Pinecone as inputs to RAG for analyzing root causes of issues occurring in the system.
We conduct a thorough evaluation using different prompts: a focused prompt that considers only the root cause and target nodes, and an extensive prompt that includes additional details such as dependencies, dependents, pathways, metrics, and mitigation factors mentioned in the generated response. Our evaluation includes scenarios without RAG, with RAG using training data on Pinecone, and with RAG using synthetic and training data on Pinecone. We assess the performance of the RAG model based on these scenarios.
The analysis prompt is generated based on the identified anomaly, including the affected service, metrics, dependencies, and dependents. The response generated by the Mistral 7B model provides detailed insights into the root cause, impact on dependencies, pathways of impact, metrics affected, and suggested mitigation strategies.
Overall, this project demonstrates the effectiveness of using RAG for root cause analysis in microservices environments, showcasing the importance of data-driven decision-making in managing complex architectures.
