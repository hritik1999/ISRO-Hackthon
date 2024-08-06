##Context-Aware Geospatial Data Retrieval using LLM/NLP

Data Processing:
Text Data: Articles, news, and research papers related to geospatial data are chunked, embedded, and stored in the vector database.
Geospatial Data: Stored in PostGIS for efficient spatial queries.
Query Handling:
User Query: When a user submits a query, a similarity search is performed in the vector database to retrieve the top 5 most relevant pieces of information.
Context Generation: The retrieved information provides context for the LLM to generate a text answer.
Geospatial Query: The text answer is used by the LLM to generate a PostGIS query, retrieving relevant geospatial data.
Output:
Text Answer: The LLM provides a detailed text answer based on the context from the vector database.
Data Plotting: The geospatial data is plotted on a map and displayed to the user, providing a clear and interactive visualization.
