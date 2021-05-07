# Named-Entity-Recognition-of-Wikipedia-Articles-using-Character-and-Word-LSTMs-
RESEARCH WORK
In this Project, created a 6 NER models, 3 for CoNLL-2003(English) Shared Task and 3 for Wikipedia Articles Dataset.

Named Entity Recognition (NER) -- Named-entity recognition (NER) (also known as (named) entity identification, entity chunking, and entity extraction) is a subtask of information extraction that seeks to locate and classify named entities mentioned in unstructured text into pre-defined categories such as person names, organizations, locations, medical codes, time expressions, quantities, monetary values, percentages, etc.

CoNLL-2003 (English) Shared Task -The shared task of CoNLL-2003 concerns language-independent named entity recognition.It consists of three sets training validation and test sets having words with pos tags, chunks tags and NE tags.This data collection comprises four types of Named Entities (NE): PERSON, LOCATION, ORGANIZATION and MISC. These NE present in IOB2 tagging scheme.The number of sentences and words in the training set, validation set and test set are --
Training Set ----- 14,987 Sentences and 204,567 Words
Validation Set ----- 3,466 Sentences and 51,578 Words
Test Set ----- 3,684 Sentences and 46,666 Words

Wikipedia Articles Dataset -- This dataset created by scrapping the dataset from different wikipedia articles from web. It contain four type of named entities(NE): PERSON (PER), LOCATION LOC), ORGANIZATION (ORG) and MISCELLANEOUS (MISC). These NE present without inside-ouside scheme of tagging. It has total word 3000 Sentences and 70418 Words. This dataset splitted in the training ,validation and test set in the ratio 4:1:1.

Training Set ----- 2000 Sentences

Validation Set ----- 500 Sentences

Test set ----- 500 Sentences

We created a model with input representation as Word encoding created from Bi-LSTM plus Word Embeddings feeded to Bi-LSTM for Context encoding along with dense layer with dropout and outputing the probablities of predicted entities with dense layer with softmax function.
We created 3 models with each of both CoNLL-2003 (English) and Wikipedia Articles Dataset.
1- NER with Word Embeddings
2- NER with Character-Level Embeddings
3- NER with both Character-Level and Word Embeddings
