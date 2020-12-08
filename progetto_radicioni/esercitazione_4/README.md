# Corpora and Sense Identification

## Corpora
A score from 0 to 4 (including decimals) of the samilarity between 100 pairs of terms (words.txt):
- 4: very similar -> synonyms
- 3: similar -> the words share a lot, but do not refer to the same concept (e.g. lion and zebra)
- 2: slightly similar -> the words do not have a very similar meaning, but they share the same topic, domain, function or are related (e.g. house and window)
- 1: different -> the two words are different, but they may have small details that unite them (ex: software and keyboard)
- 0: completely different -> the two words do not have the same meaning and belong to different topics (eg: pen and frog)

## Files
- The SemEval17_IT_senses2synsets.txt file contains the mapping from corresponding terms to synset. It can be obtained by directly querying BabelNet with the terms of the input pairs.
- The mini_NASARI.tsv file contains the vectors present in NASARI embed for the synsets listed in the previous file. Not all synsets listed in the first file have a vector description.

## Sense Identification
Calculate the similarity as the maximum obtained using as metric the cosine-similarity between the NASARI vectors of the senses associated with the various terms.

## OUTPUT 
A BabelNet synset ID and its gloss (the gloss is needed because the synset id tells us very little).
