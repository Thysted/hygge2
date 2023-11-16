This repository contains code for our assignment focused on creating a Retrieval Augmented Generation (RAG) system by integrating a powerful generative pre-trained transformer language model (LLM) with document retrieval techniques. The goal is to enable the model to generate informative responses by not only relying on its pre-existing knowledge but also augmenting it with relevant information retrieved from external documents.

Setup
We install the necessary libraries This includes LangChain, PyTorch, transformers, and other pacakges for setting up the environment

Model (LLM)
Utilizing the HuggingFacePipeline from LangChain, the assignment uses the Hugging Face transformers library to set up the Llama 2 language model. This includes the model and a tokenizer.

Simple Retrieval Augmented Generation (RAG)
Demonstrating the practical application of RAG, the assignment uses the use of LangChain's data loaders to load documents from external sources, such as PDF files. By employing the UnstructuredMarkdownLoader, the assignment efficiently loads, merges, and splits documents.

Embeddings
The assignment leverages HuggingFaceEmbeddings to generate embeddings for document chunks. By using embeddings hosted by HuggingFace and the Chroma database, the code ensures efficient storage and retrieval of embeddings.

RetrievalQA Chain
Integrating the LLM with the databases. This chain passes a user prompt to the LLM with results retrieved from the database, enabling the model to generate informative and contextually relevant answers based on both pre-existing knowledge and external information.

Interactive Conversation
In a sample interactive conversation loop, the assignment simulates a scenario where the LLM acts as an experienced high school teacher, responding to user input with informative answers. The conversation loop utilizes a chat prompt template and demonstrates the practical application of the LLM in an interactive setting.

