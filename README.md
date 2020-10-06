# Discipline analysis
***
This repository contains project files for the analysis of university disciplines.
***
## Stages of work
***
1. Obtaining data from the database of the MMIS laboratory:
- Acquaintance with the laboratory relational database schema;
- Writing
SQL query to select the required data;
- Query execution and data export.
2. Preliminary analysis of the received data using python
pandas and numpy libraries:
- Finding anomalies, errors in the request, in the data;
- Analysis of data errors, identification of the reasons for their occurrence;
- Separation of the downloaded data into several tables required
for import into a graph model and subsequent cluster analysis.
3. Building a graph based on the uploaded data:
- Writing a request to import data from a relational model into
graph. Using the Cypher query language and the Neo4j graph database.
4. Analysis of the resulting graph data model:
- Writing a query in Cypher language for a selection of disciplines with
communication of the "prerequisite" type in the senior semester;
- Request visualization by means of Neo4j Browser;
- Writing the query result to the table;
- Writing a query calculating the transitive influence and
connectivity (PageRank) of all nodes (disciplines) of the graph;
- Selection of the graph visualization tool taking into account the calculated
PageRank ratio;
- Visualization of the graph taking into account the PageRank coefficient for each
node through the Graph Data Science Playground tool.
5. Cluster analysis of RPD:
- Study of the structure of the RPD;
- Identification of the most significant RPD blocks;
- Determination of the block significance factor;
- Bringing the unloaded and separated data for cluster analysis to the form,
required for the MinHash and Word2vec algorithm;
- Algorithm modification, optimization for processing large volumes of text
information;
- Block-by-block calculation of the similarity of the RPD by pairwise comparison (each with each)
modified MinHash algorithm;
- Clustering using Word2vec technology;
- Record of results;
- Import of results into the previously built graph model for the purpose of visual analysis;
- Based on visual analysis, the definition of hyperparameters:
- degree of similarity (in%) for attributing the RPD to one cluster (for MinHash);
- coefficient of significance of the RPD block.
- Visualization and recording of cluster analysis results
- Analysis of the constructed graph model based on the output of the MinHash algorithm and
word2vec technologies.
