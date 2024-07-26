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

- `Dependency Rels/`
  - `Codes/`: ipynb notebooks for dependency parsing and extracting relations out of them using DIA Parser. Relations include \[daughter, mother, sister, brother, father, son]
  - `relation_extraction/`: Scripts for extracting relations using the REBEL model.
  - `transliteration/`: Python script for transliteration of Mahabharata text.
  - `neo4j/`: Scripts for generating and executing Cypher queries for Neo4j.
- `data/`: Contains sample data and manually labeled relations.
- `notebooks/`: Jupyter notebooks for exploratory data analysis and visualization.
- `results/`: Precision and recall metrics, along with detailed evaluation reports.

## Getting Started

### Prerequisites

- Python 3.x
- Neo4j (with APOC plugin)
- DIA Parser
- REBEL Model

