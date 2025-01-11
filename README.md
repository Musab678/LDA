# LDA




## IMDB Movie Reviews Topic Modeling

## Overview:
This project uses the **IMDB Movie Reviews Dataset** to extract hidden topics from movie reviews. The script preprocesses the reviews using tokenization, stopword removal, and stemming. Then, it applies **Latent Dirichlet Allocation (LDA)** to identify and display the key topics from the dataset.

## Features:
- Preprocesses movie reviews (stemming and stopword removal).
- Creates a dictionary of terms from processed reviews.
- Applies **LDA** for topic modeling to discover hidden themes in the reviews.
- Outputs the top words associated with each discovered topic.

## Requirements:
- Python 3.x
- Libraries:
  - `pandas`: For handling and reading the dataset.
  - `nltk`: For text processing (stemming).
  - `gensim`: For topic modeling and text preprocessing.

### To install dependencies:
```bash
pip install pandas nltk gensim
```

## Files:
- **IMDB Dataset.csv**: A CSV file containing IMDB movie reviews (each row has a review).
- **script.py**: Python script that reads the dataset, preprocesses the text, and runs topic modeling.

## How to Run:
1. Ensure that the `IMDB Dataset.csv` file is located in the same folder as the script.
2. Run the Python script:
   ```bash
   python script.py
   ```

### Steps Executed by the Script:
1. **Data Loading**:
   - Reads the `IMDB Dataset.csv` file using `pandas`.
2. **Text Preprocessing**:
   - Tokenizes the reviews.
   - Removes stopwords using the built-in list from `gensim`.
   - Applies stemming using **SnowballStemmer** from `nltk` to reduce words to their root form.
3. **Dictionary Creation**:
   - Creates a dictionary of unique words from the reviews and filters out rare words.
4. **Topic Modeling (LDA)**:
   - Applies **Latent Dirichlet Allocation (LDA)** using `gensim` to find 20 topics.
5. **Output**:
   - Displays the topics with the top words for each one.

## Output:
- The script outputs 0t09 topics, with the top words associated with each topic. For example:
  ```
  Topic: 0
  Words: 0.034*"movie" + 0.022*"film" + 0.018*"like" + 0.017*"time" + 0.014*"watch"
  ```

## License:
This project is open-source. Feel free to use or modify it for your own purposes.
