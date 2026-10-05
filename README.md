<img width="1252" height="616" alt="image" src="https://github.com/user-attachments/assets/0222e7d7-313e-4708-bc08-34e75a40f495" />

<img width="1312" height="1199" alt="image" src="https://github.com/user-attachments/assets/9520e7ee-c808-4cea-a652-eb0775d8b625" />

<img width="1254" height="1254" alt="image" src="https://github.com/user-attachments/assets/7cfb077d-a5a2-4b91-9a04-b97ae9af4940" />

## In semantic search: Sentence-Transformer for encoding  and  Numpy for dot product used

<img width="1402" height="1122" alt="image" src="https://github.com/user-attachments/assets/1822890d-da93-4f66-939b-fa22b220b33d" />

## chroma-db: open-source vector database used to store, manage, and search data based on semantic similarity.

<img width="1149" height="1369" alt="image" src="https://github.com/user-attachments/assets/70faffea-33d0-4cda-9d7a-3bbe9d894f21" />

<img width="1077" height="467" alt="image" src="https://github.com/user-attachments/assets/0269c948-771c-4576-90be-3ea2fe18039b" />

## Complete Rag Pipeline
<img width="1262" height="637" alt="image" src="https://github.com/user-attachments/assets/28cbe6bd-1332-4ec0-9b39-3706c16cf82e" />

```
 Document chunking
 Vector database storage
 Query processing
 Vector search
 Context augmentation
 Response generation

```

```
import os
import time
from typing import List, Dict, Any
import chromadb
from sentence_transformers import SentenceTransformer
from langchain_text_splitters import RecursiveCharacterTextSplitter
import numpy as np
```

```
def load_and_chunk_documents():
    # Load documents
    # Split documents into chunks
    return chunks


def setup_vector_database(chunks):
    # Create vector database
    # Store document chunks and embeddings
    return collection


def process_user_query(query):
    # Convert user query into embedding
    return query_embedding


def search_vector_database(collection, query_embedding, top_k=3):
    # Search vector database
    return search_results


def augment_prompt_with_context(query, search_results):
    # Add retrieved context to the user query
    return augmented_prompt


def generate_response(augmented_prompt):
    # Send augmented prompt to LLM
    return response


def run_complete_rag_pipeline(query):
    # 1. Process user query
    query_embedding = process_user_query(query)

    # 2. Search vector database
    search_results = search_vector_database(
        collection,
        query_embedding,
        top_k=3
    )

    # 3. Add retrieved context to prompt
    augmented_prompt = augment_prompt_with_context(
        query,
        search_results
    )

    # 4. Generate final response
    response = generate_response(augmented_prompt)

    print("\nFinal Answer:")
    print(response)

    return response


# Test all queries

for i, query in enumerate(test_queries, 1):

    print("\n" + "=" * 60)
    print(f"DEMO {i}: {query}")
    print("=" * 60)

    try:
        run_complete_rag_pipeline(query)

    except Exception as e:
        print(f"❌ Error in demo {i}: {e}")

    if i < len(test_queries):
        input("\nPress Enter to continue to next demo...")
    

```


## Caching:
<img width="1277" height="706" alt="image" src="https://github.com/user-attachments/assets/7d588ee3-14e4-48f6-ad92-2a4f0d0d142b" />
<img width="656" height="596" alt="image" src="https://github.com/user-attachments/assets/ca0a69d2-1d85-405a-a039-f43a6aecb949" />

## Monitoring:
<img width="1272" height="677" alt="image" src="https://github.com/user-attachments/assets/e34318c8-5d0b-44da-a095-b7c5c8c2f437" />

## Error Handling:
<img width="1257" height="656" alt="image" src="https://github.com/user-attachments/assets/2afb13f3-efea-4466-8263-604e9b3bd353" />
<img width="566" height="492" alt="image" src="https://github.com/user-attachments/assets/bba4924b-2d43-4281-80d0-3763df45abb7" />







