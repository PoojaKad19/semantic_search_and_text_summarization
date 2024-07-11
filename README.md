# semantic_search_and_text_summarization

## Summary

Users want to search for specific movies based on their plot descriptions or obtain concise summaries of movie plots before deciding to watch them.

How can we efficiently search and summarize movie plots to help users find relevant information and make informed decisions about which movies to watch?

The solution to the posed problem involves leveraging natural language processing (NLP) techniques such as semantic search and text summarization. 
- SBERT
- FAISS
- GPT-3

Dataset is from Kaggle. It is movie plot description scraped from Wikipedia.
https://www.kaggle.com/datasets/jrobischon/wikipedia-movie-plots/data

## Skills

1. Text pre-processing and mining using Python: Pandas, Numpy, matplotlib, NLTK, TextBlob, tqdm,SentenceTransformer
2. Semantic search pipeline using Python: Transformers, SBERT, FAISS, T5
3. Text summarization using Python: GPT-3
4. Streamlit UI deployment using Python

## Methodology

### Pre-processing of Data

- Normalizing case folding.
- Removing punctuations and numbers
- Removing stopwords
- Removing less frequently repeating words
- Tokenization using NLTK's word_tokenize
- Lemmatization using NLTK's WordNet Lemmatizer

### Semantic Search Pipeline – SBERT, FAISS

- Encoding Plots with Sentence Transformer Model
- Searching for Similar Movies
- Generating Queries for Movie Plots
- Fine-tuning a Semantic Search Model

<img width="561" alt="image" src="https://github.com/user-attachments/assets/d1f478a5-2c3d-46a3-afe1-e27d564e872b">


- Saving and Exporting the Trained Model
- Reindexing the Data with the Updated Model
- Performing Semantic Searches with the Updated Model


<img width="583" alt="image" src="https://github.com/user-attachments/assets/66bb954c-3b57-4333-ad94-b184f54f5417">


### Movie Search & Summarization Web App

- Utilized pre-trained Sentence Transformer model and Faiss index to perform semantic search over movie plot descriptions
- Present the top search results along with their titles to the user
- Defined “generate_summary” function, to utilize GPT-3, to generate summaries of movie title input based on user input

<img width="530" alt="image" src="https://github.com/user-attachments/assets/0097aedc-389c-4902-a623-5f47e984005e">

### Movie Search & Summarization Web App

Below are the screenshot of Streamlit UI

<img width="314" alt="image" src="https://github.com/user-attachments/assets/04f305a2-1ef1-403a-abb8-ea2f4574abe2">


<img width="256" alt="image" src="https://github.com/user-attachments/assets/2fc2e131-e046-44da-bfbf-ff93eb70df60">


<img width="255" alt="image" src="https://github.com/user-attachments/assets/77689516-75bd-4e46-8283-0a6f8f951cc9">


## Conclusion

1. Effective Semantic Search:
  The use of pre-trained models like SBERT for semantic search proved to be effective in retrieving relevant movies based on the similarity of their plot descriptions to user queries. This allowed users to discover movies that match their interests more accurately.

2. Automated Summarization:
  Use of GPT-3 for automatic summarization enabled the generation of concise summaries for movie plot descriptions. This  enhanced user experience by providing quick insights into the content of movies without the need to read lengthy descriptions.

3. User-Friendly Interface:
   The Streamlit web application provided a user-friendly interface for interacting with the search and summarization functionalities. Its simple layout and controls made it easy for users to search for movies and obtain relevant information.


## Potential for Further Improvement

- This project can be further improved by adding a chatbot model. This will give users a chance to query effectively about the movie they are interested in and hence make informed decision of watching a movie. 
- This could involve fine-tuning models for better performance on specific datasets or integrating additional features to enhance the user experience.



