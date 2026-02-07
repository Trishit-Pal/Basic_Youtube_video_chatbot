YouTube Video Chatbot (RAG with LangChain and Hugging Face)
This project demonstrates a basic Retrieval-Augmented Generation (RAG) system to build a chatbot that can answer questions based on the transcript of a YouTube video. It leverages various components from the LangChain ecosystem and Hugging Face models.

Key Features:

YouTube Transcript Extraction: Fetches spoken content from any public YouTube video using youtube-transcript-api.
Text Processing: Splits the raw transcript into manageable chunks using langchain_text_splitters.RecursiveCharacterTextSplitter.
Embeddings & Vector Store: Generates embeddings for text chunks using HuggingFaceEmbeddings (specifically all-MiniLM-L6-v2) and stores them in a FAISS vector database for efficient similarity search.
Retrieval-Augmented Generation (RAG): Implements a RAG pipeline to retrieve relevant text chunks based on user queries and augment the Large Language Model's (LLM) prompt.
Hugging Face LLM Integration: Utilizes a powerful Hugging Face model (meta-llama/Llama-3.3-70B-Instruct) via HuggingFaceEndpoint as the generative component for answering questions.
LangChain Expression Language (LCEL): Orchestrates the entire chatbot workflow using LangChain's runnable chains for seamless integration of retrieval, prompting, and generation.
