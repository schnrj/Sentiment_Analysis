# Sentiment Analysis App 😊😐😔😡

## About  
**A sentiment analysis application built using Streamlit**  
Sentiment Analysis is a powerful application of Natural Language Processing, allowing us to process and derive emotions from various types of data like text, audio, video, and images. This project focuses on building a web application to showcase sentiment analysis capabilities on different data types, including text, IMDb movie reviews, and images.

## Live Link  
**Hosted on Streamlit**  
🔗 [https://share.streamlit.io/gaganpreetkaurkalsi/sentimentanalysis-streamlit/main/app.py](https://share.streamlit.io/gaganpreetkaurkalsi/sentimentanalysis-streamlit/main/app.py)

## Project Specifications

**Below are the libraries and frameworks used to create the project**
- **Web Framework** :- Streamlit
- **Graphs and Images** :- PIL, plotly, cv2
- **Libraries for sentiment analysis** :- textblob, nltk(vader), flair, text2emotion, fer
- **Libraries for API requests** :- requests, json

## Project Components

**The project currently contains 3 applications:**
1. **Text** - Applying sentiment analysis on text given by the user.
2. **IMDb movie reviews** - We get review data based on movie entered by user from the IMDb API and process the same to obtain emotions of people regarding the movie.
3. **Image** - Here we analyze sentiments out of image uploaded by the user. We detect faces and then analyze sentiments for each. We also calculate the sentiment of image as a whole.

## Video Demonstration

**Application 1 - User Input**  
[![Application 1](https://github.com/schnrj/Sentiment_Analysis/blob/main/User_Input.mp4)](https://github.com/schnrj/Sentiment_Analysis/blob/main/User_Input.mp4)

**Application 2 - IMDb reviews**  
[![Application 2](https://github.com/schnrj/Sentiment_Analysis/blob/main/IMDB_Review.mp4)](https://github.com/schnrj/Sentiment_Analysis/blob/main/IMDB_Review.mp4)

**Application 3 - Image analysis**  
[![Application 3](https://github.com/schnrj/Sentiment_Analysis/blob/main/Image_Analysis.mp4)](https://github.com/schnrj/Sentiment_Analysis/blob/main/Image_Analysis.mp4)


## Important Information

### IMDb API
API documentation link - [https://imdb-api.com/api/#Reviews-header](https://imdb-api.com/api/#Reviews-header)

To work with the API, you need to first **create an API key**.  
To create an API key, **register** on the site mentioned above and a unique key will be generated for you. We will use this key to make successful requests.  
**Note:** API call limit per day is 100.

#### API Specifications
To get reviews, we will need to make 2 API calls:  
1. Get movies based on user input. Each movie received will have a unique ID.
2. Get reviews for a movie by passing the unique ID associated with it received from the above API call.

**Movie API** - [https://imdb-api.com/en/API/SearchMovie/{apiKey}/{movieName}](https://imdb-api.com/en/API/SearchMovie/{apiKey}/{movieName})  
**Review API** - [https://imdb-api.com/en/API/Reviews/{apiKey}/{id}](https://imdb-api.com/en/API/Reviews/{apiKey}/{id})

## Models Used
There are multiple libraries available in Python for sentiment analysis. Let's see them below 👇

- **TextBlob** - TextBlob is a Python library for processing textual data. It provides a simple API for diving into common NLP tasks such as part-of-speech tagging, noun phrase extraction, sentiment analysis, classification, translation, and more.
- **Flair** - A very simple framework for state-of-the-art NLP. It is a powerful NLP library which allows you to apply state-of-the-art natural language processing (NLP) models to your text, such as named entity recognition (NER), part-of-speech tagging (PoS), etc.
- **Vader** - VADER (Valence Aware Dictionary and Sentiment Reasoner) is a lexicon and rule-based sentiment analysis tool that is specifically attuned to sentiments expressed in social media.
- **text2emotion** - text2emotion is the Python package that will help you to extract the emotions from the content. It processes any textual message and recognizes the emotions embedded in it. It is compatible with 5 different emotion categories: Happy, Angry, Sad, Surprise, and Fear.

**Note:**
1. textblob, flair, and vader provide polarity scores where text is declared in one of 3 states (POSITIVE🙂, NEGATIVE☹️, NEUTRAL😐)
2. text2emotion is the only library among the others mentioned above which can classify text in 5 emotion categories (HAPPY😊, ANGRY😡, SAD😔, SURPRISE😲, FEAR😨)

## Project Development Ideas
**Below mentioned applications can be implemented as future scope:**
- Tweets analysis using Twitter API
- Sentiment analysis on Live video streaming
- Sentiment analysis of Audio data
- Sentiment analysis of data received from sites given by users using web scraping in Python.

## Thank You!  
Thank you. **I hope you liked the project**.  
If you really did then don't forget to **give a star**⭐ to this repo. It would mean a lot.
