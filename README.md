# FTD: Fuzzy Taxonomic Diversity

Fuzzy Taxonomic Diversity is a quantitative biodiversity metric designed to account for variation in taxonomic resolution and ambiguity in species assignments. Unlike traditional diversity indices that assume fully resolved and equally informative taxa, FTD incorporates both the depth of taxonomic identification and the uncertainty associated with incomplete or ambiguous classifications.

The metric is calculated by:

1. Recognizing incomplete taxonomy (e.g., reads assigned only to family or phylum) as inherently less informative than fully resolved taxa (e.g., species).

2. Modeling taxonomic ambiguity through a bootstrapping approach, where reads with unresolved assignments are randomly redistributed across plausible lower-level taxa based on available data.

3. Iteratively computing standard diversity metrics across bootstrap replicates to produce a distribution of diversity estimates that reflect uncertainty.

The final output is not a single diversity value, but a range (e.g., mean ± CI), offering a more robust and realistic summary of diversity in datasets with taxonomic ambiguity—common in metabarcoding, environmental DNA, and dietary analysis.
