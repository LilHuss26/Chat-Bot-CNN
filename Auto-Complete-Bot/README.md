# N-gram Language Model for Autocomplete (Python)

**Description:**

This Python script implements a basic N-gram language model for text autocompletion. It allows users to enter a sequence of words, and the model suggests the most likely next word based on the frequency of word n-grams observed in the training data.

**Features:**

* Processes and cleans Twitter data using regular expressions and tokenization.
* Handles out-of-vocabulary (OOV) words using an unknown token ("<unk>").
* Builds N-gram models (unigrams, bigrams, trigrams, etc.) up to a configurable maximum N.
* Calculates probabilities for next words using Laplace smoothing.
* Provides suggestions based on multiple N-gram models, allowing the user to choose the best fit.

**Usage:**

1. Save the script as `n_gram_autocomplete.py`.
2. Modify the `file_path` variable in the script to point to your Twitter data file (.txt format).
3. Run the script: `python n_gram_autocomplete.py`.
4. Enter a sequence of words and press Enter. The script will suggest the most likely next word(s).
