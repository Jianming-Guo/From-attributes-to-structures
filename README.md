# Patent Value Evaluation with Attribute–Structure Integration
## Overview
This repository provides the code and dataset for the study on patent value evaluation by integrating attribute-based indicators and network structural features.

The proposed framework extends classical PageRank and HITS algorithms by incorporating patent attribute information directly into the ranking process, enabling a unified evaluation of patent value.

The repository supports reproducibility of the results reported in the corresponding Scientometrics submission.

## Dataset Description
The dataset is organized into three technological domains, each stored as a separate folder.

Each domain contains the following files:

1. patent_node.csv
Nodes in the patent citation network
Each row represents a patent
2. patent_edge.csv
Directed citation relationships between patents
Format: source → target
3. patent_score.csv
Final computed patent value scores
Includes:
Attribute-based score
Structural score
Integrated score
4. 02patents_normalized_with_scores.csv
Preprocessed patent-level dataset
Includes:
Raw indicators
Normalized variables
Intermediate attribute scores

## Methodology
The framework consists of three main components:

1. Attribute-based evaluation

Patent value is quantified using multiple indicators (e.g., citations, claims, technological features), which are normalized and aggregated.

2. Network structural evaluation

Patent importance is captured using citation networks and ranking algorithms:

PageRank
HITS
3. Integrated evaluation

Attribute information is embedded into the ranking process:

Generalized PageRank
Generalized HITS

This enables attribute and structural information to jointly influence the ranking results.

## How to Run
Clone the repository:
git clone https://github.com/your-repo-link
Install dependencies:
pip install -r requirements.txt
Run notebooks:
generalized_pagerank.ipynb
generalized_hits.ipynb

## Reproducibility
The repository includes:

Full datasets
Core algorithms
Intermediate processing steps

All key results in the paper can be reproduced using the provided scripts.

## Environment
Recommended environment:

Python 3.10+
numpy
pandas
networkx
scipy
scikit-learn
matplotlib

## Notes
Data are derived from patent citation networks within selected technological domains.
Large files are compressed for efficient storage and download.

## License
This project is released under the MIT License.







