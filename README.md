# Natural Language Processing

Name: Manahil Shahid
Reg No: SP24-BDS-023
Class: BDS-6A

The Jupyter notebooks in this repository are my Natural Language Processing lab tasks and assignment. Each notebook demonstrates NLP concepts with working code, real output, and short notes that explain what the code does and what the output shows. I will keep adding notebooks as I study more of the subject.

## NLP Concepts

### Text Basics
Corpus: a collection of text used for analysis or training.
Token and tokenization: a token is a unit of text such as a word, subword or character. Tokenization splits text into tokens.
Vocabulary: the set of distinct tokens in a corpus.
Sentence segmentation: splitting a text into sentences.
Regular expressions: patterns used to search, match and replace text.

### Text Preprocessing
Case normalization: lowercasing text to shrink the vocabulary, at the cost of losing capital letter information.
Noise removal: deleting URLs, HTML tags, mentions, emojis and extra whitespace.
Stop word removal: dropping very common words such as the, is and of. It saves space but can destroy negation and grammar.
Stemming: cutting word endings with fixed rules, for example running to run. Fast, but it can over stem and under stem.
Lemmatization: mapping a word to its dictionary form using its part of speech, for example was to be.
Text normalization: making text consistent through spelling fixes, abbreviation expansion and number handling.

### Edit Distance and Spelling
Minimum edit distance (Levenshtein): the fewest insertions, deletions and substitutions needed to turn one string into another.
Dynamic programming: solving a problem by storing answers to small sub problems so none is computed twice.
Backtrace: walking back through the DP table to recover the exact edit operations.
Spelling correction: ranking dictionary words by edit distance and breaking ties with word frequency.
Real word errors: mistakes that are valid words, such as their for there, which need context to detect.

### Text Representation
Bag of words: representing a text by word counts and ignoring order.
TF-IDF: a weight that is high for words frequent in a document but rare across documents.
N-grams: sequences of n neighbouring tokens that capture some word order.
One hot encoding: a sparse vector with a single 1 for each word.
Word embeddings: dense vectors where similar words are close together (Word2Vec, GloVe, FastText).
Contextual embeddings: vectors that change with the sentence, as in BERT and GPT.

### Language Models
Language model: a model that assigns a probability to a sequence of words.
N-gram language model: predicts the next word from the previous n minus 1 words.
Smoothing: giving unseen n-grams a small probability (Laplace, backoff, Kneser Ney).
Perplexity: a standard measure of how well a language model predicts text.

### Syntax and Linguistic Analysis
Part of speech (POS) tagging: labelling each word as noun, verb, adjective and so on.
Named entity recognition (NER): finding names of people, organizations, places and dates.
Chunking and shallow parsing: grouping words into phrases such as noun phrases.
Constituency parsing: building a phrase structure tree of a sentence.
Dependency parsing: finding head and dependent word relations.
Coreference resolution: linking words like he and it to the thing they refer to.
Word sense disambiguation: choosing the right meaning of a word with several meanings.

### Text Classification and Sentiment
Text classification: predicting a label for a text, for example spam or not spam.
Naive Bayes and Logistic Regression: classic classifiers used with bag of words and TF-IDF features.
Sentiment analysis: detecting opinion in text, with lexicon tools like VADER or trained models.
Negation handling: keeping words like not and no so the meaning does not flip.
Cross validation: training and testing on several splits to get a stable accuracy.
Evaluation metrics: accuracy, precision, recall and F1 score.

### Neural NLP
Recurrent neural networks (RNN): networks that read a sequence one step at a time.
LSTM and GRU: recurrent networks with gates that handle longer memory.
Sequence to sequence models: an encoder and decoder pair for tasks like translation.
Attention: letting a model focus on the most relevant words.
Transformer: an architecture built on self attention instead of recurrence.
Pretrained language models: BERT, GPT and similar models that are fine tuned for tasks.

### NLP Applications
Machine translation: translating text between languages, scored with BLEU.
Question answering: finding or generating answers to questions.
Chatbots and intent detection: understanding what a user wants from a short message.
Text summarization: shortening a text while keeping the main points.
Topic modelling: finding hidden topics in a corpus, for example with LDA.
Information retrieval and search: ranking documents for a query.
Information extraction: pulling structured facts out of unstructured text.

## Tools Used

Python, Jupyter Notebook, NLTK, spaCy, scikit-learn, pandas, NumPy, matplotlib

## How to Run

```
pip install nltk spacy scikit-learn pandas matplotlib
python -m spacy download en_core_web_sm
```

Open any notebook in Jupyter, VS Code or Google Colab and run the cells from top to bottom.
