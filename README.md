# Olfacatory-NER

## Summary

The overall objective of this project was to replicate the results of a paper by Menini et al. (2023) which developed a supervised system for information extraction of olfactory language. This project followed their methods for named entity recognition (NER) of olfactory-related entities in text. This information extraction task was approached as a token classification task. The entities of interest were smell word, smell source, and quality. The method to approach this task was to train the Bert-base-uncased model using annotated data from the Odeuropa dataset. To achieve better results a hyperparameter search was conducted and then the model was trained five times with each of the folds. 

## Data

The data was from the English subset of the Odeuropa dataset (https://github.com/Odeuropa
/benchmarks_and_corpora) which is a multilingual dataset of books tagged with olfactory information. The data in English consisted of 86 books across 10 genres published from 1602-1933. The domains of the dataset cover: Household & Recipes, Law, Literature, Medicine & Botany, Perfumes & Fashion, Public health, Religion, Science & Philosophy, Theatre, Travel & Ethnography. This data set was tagged with 10 different entities of which 3 (smell source, smell word, and quality) were of interest. The data contained 147 beginning smell source entities, 136 inside smell source entities, 124 smell word entities, 92 beginning quality entities, and 61 inside quality entities.
