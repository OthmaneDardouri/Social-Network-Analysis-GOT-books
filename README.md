# Social Network Analysis of Game of Thrones: An Exploration of Character Dynamics
Overview
This project presents a social network analysis of George R.R. Martin's epic series A Song of Ice and Fire, known widely through its TV adaptation, Game of Thrones. By examining the interactions between characters, this study merges literary analysis with network science to reveal insights into character relationships, power structures, and narrative trends. The analysis is based on interactions across the five books of the series, exploring alliances, rivalries, and character prominence.

## Objective
The primary aim is to investigate the complex network of character relationships in the series. Through this analysis, we aim to:

Identify key characters and their significance using centrality measures.
Discover clusters of interconnected characters and analyze their relevance to the plot.
Enhance understanding of the series' narrative by visualizing and quantifying character interactions.
## Datasets
The analysis leverages the Game of Thrones Online Dataset, which is available publicly on Kaggle. This dataset represents character interactions across the five books of the series:

## Data Collection: Character pairs are marked as connected if they appear within 15 words of each other in the books. Connections are weighted, indicating the frequency of interactions.
Structure: The dataset is an undirected, weighted graph with five columns: Source, Target, Type, Weight, and Book.
Nodes: Characters appearing in the story.
Edges: Represent interactions, with weights quantifying the number of co-occurrences.
Total Counts:
Nodes: 796 (aggregated across all books)
Edges: 2822 (total interactions)
## Book-Specific Networks
Each book is represented as a separate network:

| Book   | Nodes | Edges |
|--------|-------|-------|
| Book 1 | 187   | 684   |
| Book 2 | 266   | 774   |
| Book 3 | 293   | 1008  |
| Book 4 | 309   | 682   |
| Book 5 | 325   | 760   |
| **All Books** | **796**   | **2822**  |



Visualizations
Below are visualizations of networks for Book 1 and Book 2:
![Book 1](C:/Users/othma/Downloads/Social Network Analysis of _Game of Thrones_ series/book_1.png)
Node size is proportional to the degree of each character (number of direct interactions).
Book 1Book 2

## Methodology
The analysis was implemented using NetworkX, a Python library for the creation, manipulation, and study of the structure and dynamics of complex networks.

## Key Measures Used
Degree Centrality: Identifies the most connected characters in each book. For example, Eddard Stark emerged as the character with the highest degree centrality in Book 1, indicating his prominence in the narrative.
Clustering and Group Detection: Using network analysis techniques, we explored groups of nodes that form tightly connected clusters, revealing potential alliances or conflicts.
Results and Findings
Degree Centrality Insights
Main Characters: The analysis identified Eddard Stark, Robert Baratheon, Tyrion Lannister, and Catelyn Stark as having the highest degree centrality, underscoring their significant roles.
Threshold for Significance: A degree centrality threshold of 0.20 was used to filter out the most influential characters across each book and in the aggregated dataset.
Clustering Analysis
Clusters: The network analysis revealed distinct character clusters, aligning with known alliances and rivalries from the story. This validates the model's accuracy and reflects the underlying narrative structure.
Validity and Reliability
Validity: While the dataset provides a reasonable representation of interactions, its accuracy may be influenced by the subjective criteria used for defining interactions (i.e., proximity within 15 words).
Reliability: The dataset is hosted on Kaggle, a trusted platform for data sharing. It is widely used, has been verified by the community, and received a bronze medal for popularity and reliability.
Conclusion
This project demonstrated the utility of social network analysis for examining complex relationships in literature. By applying network science, we gain a deeper understanding of character interactions and story structure, providing fresh insights that enhance traditional literary analysis.

## Prerequisites
Ensure the following Python packages are installed:

scikit-learn: pip install scikit-learn
pandas: pip install pandas
networkx: pip install networkx
matplotlib: pip install matplotlib
seaborn: pip install seaborn
## Future Work
Advanced Metrics: Extend the analysis to include betweenness centrality and closeness centrality.
Temporal Analysis: Explore how relationships evolve across different books.
Comparison with the TV Series: Apply the same analysis to the show for comparative insights.
## References
Dataset: Game of Thrones Online Dataset on Kaggle
NetworkX Documentation: NetworkX Library
