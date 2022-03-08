# Web Scraping, Text Wrangling and Pre-processing (Inshorts News)

This covers the following aspects of NLP :

1. Data Retrieval with Web Scraping
2. Text wrangling and Pre-processing

When I started delving into the world of data science, even I was overwhelmed by the challenges in analyzing and modeling on text data. However, after working on several challenging problems and projects around NLP over the months, I’ve noticed certain interesting aspects, including techniques, strategies and workflows which can be leveraged to solve a wide variety of problems.

The source data which I have used are news articles, which I have retrieved from Inshorts, a website that gives us short, 60-word news articles on a wide variety of topics, and they even have an app for it!

Web Scraping using Beautiful Soup.

For text-wrangling and text pre-processing, I have leveraged a fair bit of nltk
and spacy , both state-of-the-art libraries in NLP. Typically a pip install <library> or a
conda install <library> should suffice.
  
## OPTIONAL: ONLY USE IF SPACY FAILS TO LOAD LANGUAGE MODEL
## Use the following command to install spaCy
> pip install -U spacy
OR
> conda install -c conda-forge spacy

## Download the following language model and store it in disk
https://github.com/explosion/spacy-models/releases/tag/en_core_web_md-2.0.0

## Link the same to spacy 
> python -m spacy link ./spacymodels/en_core_web_md-2.0.0/en_core_web_md en_core
Linking successful
    ./spacymodels/en_core_web_md-2.0.0/en_core_web_md --> ./Anaconda3/lib/site-packages/spacy/data/en_core
You can now load the model via spacy.load('en_core')

Contractions module is not a standard python module. I did leverage a standard set of
contractions available in the contractions.py file in my repository. Please add it in the
same directory you run your code from, else it will not work.

Happy Learning!

