# Context-Aware Geospatial Data Retrieval using LLM/NLP

This repository contains the implementation of a context-aware geospatial data retrieval system leveraging large language models (LLM) and natural language processing (NLP) techniques. The system processes textual and geospatial data to provide users with relevant information and visualizations based on their queries.

## Features

- **Data Processing:**
  - **Text Data:** Articles, news, and research papers related to geospatial data are chunked, embedded, and stored in a vector database.
  - **Geospatial Data:** Stored in PostGIS for efficient spatial queries.
  
- **Query Handling:**
  - **User Query:** When a user submits a query, a similarity search is performed in the vector database to retrieve the top 5 most relevant pieces of information.
  - **Context Generation:** The retrieved information provides context for the LLM to generate a text answer.
  - **Geospatial Query:** The text answer is used by the LLM to generate a PostGIS query, retrieving relevant geospatial data.
  
- **Output:**
  - **Text Answer:** The LLM provides a detailed text answer based on the context from the vector database.
  - **Data Plotting:** The geospatial data is plotted on a map and displayed to the user, providing a clear and interactive visualization.

## Technologies Used

- **Model:** 
  - **Llama 3.1 (8B):** Natural language understanding and generation.
  
- **Embedding:**
  - **sentence-transformers/all-MiniLM-l6-v2:** Text data embeddings.
  
- **Databases:**
  - **Vector Database:** ChromaDB - Stores embedded text data.
  - **Spatial Database:** PostgreSQL with PostGIS - Manages geospatial data.
  
- **Geospatial Tools:**
  - **fastkml:** Handles KML files.
  - **shapely:** Geometric operations.
  - **geopandas:** Spatial data operations.
  - **json:** Data interchange.
  
- **Database Connectivity:**
  - **SQLAlchemy:** Connects and queries PostGIS.
  
- **Visualization:**
  - **Matplotlib:** Data plotting.
  - **contextily:** Map tiles and overlays.
  
- **Data Management:**
  - **Langchain:** Chunks, embeds, stores data, integrates LLM.




