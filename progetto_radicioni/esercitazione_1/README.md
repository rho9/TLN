# Conceptual similarity with WordNet
The aim of this project is to find the conceptual similarity of a list of words using 3 different misures:
- Wu & Palmer
- Shortest Path
- Leakcock & Chodorow

For each measure we compute:
- Spearman's rank correlation coefficient
- Pearson correlation coefficient

We then compare the results with the values in the file WordSim353.

## Input
Use WordSim353 (tsv or csv). Each line is formed by 2 terms and their similarity given by humans [0,10].

## Output
Numerical similarity score indicating the semantic proximity of the input terms.

## Score
In the range [0,1]: 0 completely dissimilar; 1 identity

## How to
Execute: 'python3 conc_sim_WN.py WordSim353.tab'
