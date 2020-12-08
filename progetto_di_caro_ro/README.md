# Text Segmentation
The aim of this project is to implement a simple segmentation system of texts inspired by Text Tiling using resources such as WordNet, named entities, etc.

## Text Tiling Algorithm
Credits: https://www.aclweb.org/anthology/J97-1003

TextTiling: Segmenting Text into

Multi-paragraph Subtopic Passages

Marti A. Hearst*, Xerox PARC

The Text Tiling algorithm for discovering subtopic structure using term repetition has three main parts:
1. Tokenization
2. Lexical Score Determination
3. Boundary Identification

## How it works
w: pseudo sentence size  
k: number of pseudo sentences within the blocks

- Divide the sentence into blocks of fixed size
- Within each block compare the words in pseudo sentences contiguous
- Split the block where the minimum of the previous step is
