# RAG-System
RAG system that can provide personalized skill recommendations and career advice to users based on their queries about specific job roles

![image](https://github.com/user-attachments/assets/52b8a42e-1042-4f47-ad7f-66ae109d6de8)



### Data Loading: 
Ensure the job data CSV file is correctly placed and accessible. Load the data and preprocess it by combining job descriptions and requirements.
### Embedding Creation: 
Initialize the Sentence Transformer model and create embeddings for the combined job details in manageable chunks.
### FAISS Indexing: 
Initialize a FAISS index with the appropriate dimensions and add job embeddings to the FAISS index for efficient similarity search.
### Model Initialization: 
Load the tokenizer and generative model (e.g., LlamaForCausalLM). Move the model to GPU if available for faster processing.
### Query Processing: 
Use the retrieval function to get relevant job postings based on user queries. Generate a personalized response using the generative model.
