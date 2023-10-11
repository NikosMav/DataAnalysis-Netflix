# Movie and TV Show Recommendation System

## Overview

This Jupyter Notebook presents a recommendation system for movies and TV shows using two different methods: Boolean (Bag of Words, BoW) and TF-IDF (Term Frequency-Inverse Document Frequency). The system uses text descriptions of movies and TV shows to provide recommendations based on similarity scores.

## Dependencies

To run this notebook, you'll need the following dependencies:

- Python (>=3.7)
- Jupyter Notebook
- Pandas
- Scikit-learn (for BoW)
- TfidfVectorizer (from Scikit-learn, for TF-IDF)
- Numpy

You can install these dependencies using pip or conda:

```bash
pip install jupyter pandas scikit-learn numpy
```

## How to Use

Clone the Repository:

```bash
git clone https://github.com/your-username/DataAnalysis-Netflix.git
cd your-repo
```

Open the Jupyter Notebook:

```bash
jupyter notebook netflix_data_analysis.ipynb
```

Run the Notebook:

Click on "Cell" > "Run All" to run all the cells.
Follow the instructions and examples provided in the notebook.

## Components

The notebook contains the following main components:

1. Data Preprocessing: Loading and preparing the dataset for recommendation.

2. Similarity Computation:
For BoW: Calculating Jaccard similarity between items based on binary text representations.
For TF-IDF: Calculating cosine similarity between items based on TF-IDF vector representations.

3. Recommendation Functions:
get_similar_movies1: Recommends similar items based on user input using BoW or TF-IDF.
get_similar_movies2: Recommends similar items based on user input using BoW or TF-IDF with text data.

4. Testing and Analysis: Evaluating and comparing the recommendation methods.

5. Results: Displaying recommendations for sample input queries.

## Methodology

- The system precomputes similarity matrices for both BoW and TF-IDF representations, which significantly speeds up the recommendation process.
- Two recommendation functions (get_similar_movies1 and get_similar_movies2) are provided to recommend items based on user input text.
- TF-IDF method generally provides more accurate and relevant recommendations compared to BoW (Boolean) method, especially for text-based recommendation tasks.
- Cosine similarity is more efficient and provides better results with text data compared to Jaccard similarity.

## Conclusion

This recommendation system demonstrates the effectiveness of TF-IDF in providing accurate and relevant recommendations for movies and TV shows. It also highlights the computational efficiency of cosine similarity in comparison to Jaccard similarity.

Feel free to explore and use this notebook to build and experiment with your own recommendation system.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE.md) file for details.
