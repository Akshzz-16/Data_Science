# INSIGHTS: 
**There are more of a positive reviews compared to negative reviews and it was shown predicted accurately.**

### IMPORT LIBRARIES AND LOAD THE DATASET:

- Importing libraries and reading the .csv dataset with encoding in *data* variable.
- Printing the **first 5 rows** of dataset. 

### DATA CLEANING:
- This code performs text preprocessing on a dataset with a column named 'review', which presumably contains text data. 
- IMPORT REQUIRED LIBRARIES
  - **`re`**: Used for regular expressions to clean the text.
  - **`nltk`**: A library for natural language processing, used for tokenization, stemming, and stopword removal.
  - **`PorterStemmer`**: A stemming algorithm that reduces words to their base or root form.
  - **`word_tokenize`**: Tokenizes text into individual words.
  - Downloads the necessary data for tokenization (punkt) and English stopwords (common words like "the", "and", "is").

- Preprocessing Function
  - **`Cleaning`**: Removes punctuation and special characters.Converts text to lowercase.
  - **`Tokenization`**:Breaks the text into individual words. 
  - **`Stopword Removal`**:Filters out common words (e.g., "and", "the") that don't carry significant meaning.
  - **`Stemming`**:Reduces words to their root forms (e.g., "running" → "run").
  - **`Progress Logging`**:Prints progress every 1000 rows using the index idx.

### SENTIMENT ANALYSIS:
- `TextBlob` is a Python library for processing textual data. It provides tools for common natural language processing tasks, including sentiment analysis
- **`Input`**: A single text string (text).
- **`Process`**:
- **`TextBlob(text)`**: Analyzes the text.
- **`analysis.sentiment.polarity`**: A float value between -1 and 1 representing the sentiment polarity:
  - Positive polarity: Values > 0.
  - Negative polarity: Values <= 0.
- **`Output`**: Returns 'positive' for texts with positive polarity and 'negative' otherwise

### VISUALIZE:
- Visualizing the positive and negative values assigned to the sentence. 