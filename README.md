# Mahabharat Knowledge Graph: Relation Extraction and Visualization with Neo4j

This repository contains the code and resources for the project "Mahabharat Knowledge Graph: Relation Extraction from Index and Visualizing with Neo4j," developed as part of the Computational Linguistics (CS689) course at IIT Kanpur (Feb 2024 - April 2024).

## Project Overview

The project aims to build a knowledge graph representing the family relations depicted in the ancient Indian epic, Mahabharata. We employed advanced computational linguistic techniques for extracting and visualizing these relations.

### Key Features

1. **Dependency Parsing with DIA Parser**: Utilized the DIA Parser for dependency parsing on the Mahabharata index, extracting rules from recurring patterns in family relations depicted in the text.
   - Achieved a precision of 90.75%.

2. **Relation Extraction with REBEL Model**: Compared results with the REBEL model to derive relation triplets.
   - Achieved a precision of 33.7% when evaluated against 150 manually labeled relations.

3. **Transliteration and Automation**: Developed a Python script for:
   - Transliteration of Mahabharata text from ISO15919 to Latin script.
   - Automating the generation of Cypher queries for importing data into the Neo4j graph database.

## Repository Structure

- `Dependency Rels/`: Contains pickle file of relations extracted from parsing.
  - `Codes/`: ipynb notebooks for dependency parsing and extracting relations out of them using DIA Parser. Relations include \[daughter, mother, sister, brother, father, son]
- `Evaluation/`: Precision and accuracy metrics, along with detailed evaluation reports. REBEL results were evaluated against 150 manually labelled relations.
- `Relations/`: Relations extracted from the REBEL model.
Rest are the notebooks for text cleaning, extracting relations using REBEL model, Transliterating the text from ISO15919 to Latin, Automating the process of feeding the triplets to Neo4j and generating the knowledge graph.

### Prerequisites

- Python 3.x
- Neo4j (with APOC plugin)
- DIA Parser
- REBEL Model

