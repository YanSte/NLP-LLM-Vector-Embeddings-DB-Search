# | NLP | LLM | Vector | Embeddings DB Search |

## Natural Language Processing (NLP), Large Language Models (LLM), and the Power of Vector Embeddings and Databases

![Learning](https://t3.ftcdn.net/jpg/06/14/01/52/360_F_614015247_EWZHvC6AAOsaIOepakhyJvMqUu5tpLfY.jpg)

# <b><span style='color:#78D118'>|</span> Overview</b>

### Embeddings, Vector Databases, and Advanced Search

Converting text into embedding vectors is the first step to any text processing pipeline. As the amount of text gets larger, there is often a need to save these embedding vectors into a dedicated vector index or library, so that developers won't have to recompute the embeddings and the retrieval process is faster. We can then search for documents based on our intended query and pass these relevant documents into a language model (LM) as additional context. We also refer to this context as supplying the LM with "state" or "memory". The LM then generates a response based on the additional context it receives! 

In this notebook, we will implement the full workflow of text vectorization, vector search, and question answering workflow. While we use [FAISS](https://faiss.ai/) (vector library) and [ChromaDB](https://docs.trychroma.com/) (vector database), and a Hugging Face model, know that you can easily swap these tools out for your preferred tools or models!

<img src="https://storage.googleapis.com/kagglesdsdata/datasets/4232024/7296128/vector.png?X-Goog-Algorithm=GOOG4-RSA-SHA256&X-Goog-Credential=databundle-worker-v2%40kaggle-161607.iam.gserviceaccount.com%2F20231228%2Fauto%2Fstorage%2Fgoog4_request&X-Goog-Date=20231228T094528Z&X-Goog-Expires=345600&X-Goog-SignedHeaders=host&X-Goog-Signature=2358155e44397b47c5cd178ae645e0ad4a656e3f30b773ce9ce29dc596a7c59319465e6fa9f2c8019257a0be627bbff2e3452aa2cb9b8e117813fdf62b82d6864f2b6a31f00e4bdab75eafff8b634426b6d0781331179283408fa357eaf43ce17dfcafea30461d305fb647abdfbe4309ca0921b5bd816451e084e12df550ebad38f020e39b1ebc2df4821c02cc861d5b44a6eb581bfada85c074e6913d64554777cab3c035f2e946146fc743dadbeee62019fa5649219573616c341566ffc3a122b04070cb72152f4bc4810c4be4bd45f28442a7d1e1b8e20c279c511b506274a31208f7aa8b61b91af0dbaab42b3aa6c52dc5024dd98d1c2538d08d47f9d6ce" width=1000 target="_blank" > 

### Learning Objectives
1. Implement the workflow of reading text, converting text to embeddings, saving them to FAISS and ChromaDB 
2. Query for similar documents using FAISS and ChromaDB 
3. Apply a Hugging Face language model for question answering.
