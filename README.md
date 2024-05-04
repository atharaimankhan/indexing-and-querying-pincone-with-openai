# Langchain Sample Project
## _Indexing and Querying Pinecone with OpenAI_

This is just a sample file for beginner to understand the working.

## Steps

- First we load the pdf file using loader from langchain
- Then we divide it into chunks because token size must be small.
- Create OpenAI Embeddings 
- Connect to Pinecone index and Insert all the embeddings as vectors into it
- Initallized chain with openai llm and our pinecone vector database
- Run the quries

## How to Run:

Add a file named ".env" and add following enviroment variables names with respective API KEYS:
```sh
OPENAI_API_KEY=
PINECONE_API_KEY=
PINECONE_INDEX_NAME=
```
Now activate venv:
```sh
python -m venv venv
source ./venv/bin/activate
```
Install requirements:
```sh
pip install -r requirements.txt
```
Create a folder named *"document"* and put a PDF file in it like a Resume for instance. 

