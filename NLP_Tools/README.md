This folder contains 12 proposed NLP-based tools using the combination of 03 key phrase extraction (YAKE,PatternRank, KeyBert) and 04 similarity measures
(Cosine, Jarow-Wrinkler, Latent Sementic Analysis (LSA), Word2Vec)in NLP.

Proposed NLP-based tools are
* YAKE_Cosine
* YAKE_JaroW
* YAKE_LSA
* YAKE_Word2Vec
* PATTERN_Cosine
* PATTERN__JaroW
* PATTERN__LSA
* PATTERN_Word2Vec
* KEYBERT_Cosine
* KEYBERT__JaroW
* KEYBERT__LSA
* KEYBERT_Word2Vec
  
Main sections in the proposed NLP-based tools are as follows;

**Section 01: Text cleaning**

This section is responsible for preprocessing the text extracted from PDF documents. 
It involves data preprocessing tasks. After completing data preprocessing, the list of cleaned text is converted into string and then entire string is used as an input to key phrase extraction function.   

**Section 02: Key phrase extraction for cleaned text**

In this section, (YAKE_Extractor, PATTERNRANK_Extractor, KEYBERT_Extractor) focus on the extraction of key phrases from the preprocessed text.
In this study, three distinct algorithms namely, YAKE, PatternRank, and KeyBert have been selected from the unsupervised key phrase extraction methods in NLP. 
Each algorithm contributes its unique approach to identifying and isolating essential phrases in the text.  

**Section 03: Extraction of the list of EO4GEO BoK concepts and pre-processing the extracted list**

This section (EO4GEO) involves automating the extraction of EO4GEO BoK concepts from an [EO4GEO BoK visualization and search tool](https://bok.eo4geo.eu/GIST) and EO4GEO BoK RESTfull API v219. 
The extracted BoK list is then pre-processed, potentially involving tasks mentioned in the data preprocessing task

**Section 04: Measure similarity between extracted key phrases and EO4GEO concepts**

The role of these similarity measurement section (Cosine_Similarity, Jarowinkler_Similarity, LSA_Similarity, Word2Vec_Similarity) is to compute the similarity between the list of extracted key phrases and the pre-processed EO4GEO BoK concepts. 
In this study, four distinct similarity technologies within the lexical and semantic similarity have been employed. 
These technologies encompass Cosine Similarity, Jarow-Winkler Similarity, LSA Similarity, and Word2Vec Similarity measures

**Section 05: Download Output Results as a JSON Format**

This section (Create_Json) allows users to download the output results in a structured format, specifically JSON.  
This gives the DOI, title of the relevant paper, and the matching EO4GEO BoK concepts (with original names) for given PDF document 

NOTE :  In oder to run the tools required library should be installed. Also 'glove.6B.50d' and 'glove.6B.100d' should be downloaded from 
[GloVe: Global Vectors for Word Representation] (https://nlp.stanford.edu/projects/glove/)

