# GSG-Task
## Humans Talk, Machines Understand: LLM & NLP Mastery with GSG
This Python script provides three functions for basic text processing and analysis:

1. `preprocess_text`: Cleans and tokenizes text.
2. `word_frequency`: Counts the frequency of words in the processed text.
3. `estimate_sentiment`: Estimates the sentiment (positive, negative, or neutral) based on predefined word lists.

### Requirements

- Python 3.x
- Standard library module: string

### Functions
#### 1. preprocess_text(text)

Purpose:
  - Converts text to lowercase
  - Removes punctuation
  - Splits string into words
  - Removes common stopwords.
Input: String of text.
Output: List of processed words.
Stopwords: ["the", "and", "in", "is", "to", "of"]

#### 2. word_frequency(text)

Purpose: 
  - Counts the frequency of each word in the processed text.
Input: String of text.
Output: Dictionary with words as keys and their frequencies as values.
Depends on: preprocess_text

#### 3. estimate_sentiment(text)

Purpose: 
  - Estimates sentiment based on counts of positive and negative words.
Input: String of text.
Output: String: "positive", "negative", or "neutral".
Positive Words: ["good", "happy", "excellent", "great", "wonderful]
Negative Words: ["bad", "sad", "terrible", "horrible", "awful"]
Logic:
Positive count > Negative count: Returns "positive"
Negative count > Positive count: Returns "negative"
Otherwise: Returns "neutral"
Depends on: preprocess_text

