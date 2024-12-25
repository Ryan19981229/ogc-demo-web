# Technology Description

We are leveraging Retrieval-Augmented Generation (RAG) technology to develop our Virtual Assistant.

Traditional generative language models rely on pretraining to build their knowledge base, but they have inherent limitations. These models may provide outdated or inaccurate responses when dealing with new information or rapidly evolving fields. Updating the model through retraining or fine-tuning to expand its knowledge requires substantial time and computational resources.

RAG combines retrieval and generation techniques to address these challenges. It enhances the language model's knowledge by retrieving relevant information from an external database and incorporating it into responses. This approach ensures timeliness and accuracy in the assistant’s outputs. Additionally, RAG reduces reliance on large-scale parameters, as the retrieval system supplies the necessary information, and the generation model focuses solely on crafting responses based on those inputs.

This dual approach improves system efficiency and simplifies model training. RAG balances knowledge coverage and response quality, making it particularly effective in scenarios requiring dynamic data updates. By integrating RAG, our Virtual Assistant achieves enhanced accuracy, flexibility, and efficiency in generating reliable, up-to-date responses.

## Technology Used
- Development Framework: Langchain 0.3
- Programming Language: python 3.12.8
- Generative Language Model: OPENAI GPT-4（Generative Pre-trained Transformer）
- Embedding Model: OpenAI Embeddings
- Vector Database: Chroma
