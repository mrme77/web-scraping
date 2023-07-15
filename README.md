# Project Title

Web Scraping and NLP with Requests, BeautifulSoup, and spaCy

## Description

This project is part of the Web Mining and Applied NLP (44-620) course, student's name is Pasquale Salomone. The notebook aims at reviewing some python functionalities like web scraping and NLP with Requests, BeautifulSoup, and spaCy. Here is the link to the Github repository: [Github Repo](https://github.com/mrme77/web-scraping).

## Table of contents

### Question 1 
Write code that extracts the article html from https://web.archive.org/web/20210327165005/https://hackaday.com/2021/03/22/how-laser-headlights-work/ and dumps it to a .pkl (or other appropriate file)

### Question 2 
Read in the article's html source from the file you created in question 1 and print it's text (use .get_text())

### Question 3 
Load the article text into a trained spaCy pipeline, and determine the 5 most frequent tokens (converted to lower case). Print the common tokens with an appropriate label. Additionally, print the tokens their frequencies (with appropriate labels). Make sure to remove things we don't care about (punctuation, stopwords, whitespace).

### Question 4 
Load the article text into a trained spaCy pipeline, and determine the 5 most frequent lemmas (converted to lower case). Print the common lemmas with an appropriate label. Additionally, print the lemmas with their frequencies (with appropriate labels). Make sure to remove things we don't care about (punctuation, stopwords, whitespace).

## Installation

To use this project, make sure you have Python 3.8 installed on your system. Do not install modules like math and statistics. You can check your Python version by running the following command in your terminal:

```shell
python --version
```

### Modules

The following modules are required for the installation of this project:
<br>
```import requests,pickle,io,re,spacy
from bs4 import BeautifulSoup
from contextlib import redirect_stdout
from spacytextblob.spacytextblob import SpacyTextBlob
from spacy.lang.en.stop_words import STOP_WORDS
from collections import Counter
import matplotlib.pyplot as plt
import numpy as np
```
## Acknowledgments

I would like to acknowledge the following resources that were instrumental in the development of this project:

- ChatGPT by OpenAI: We used ChatGPT, a powerful language model, to assist in generating responses and providing guidance during the development process. ChatGPT played a crucial role in enhancing the functionality and accuracy of our project.

- Stack Overflow: We would like to express our gratitude to the vibrant community of developers on Stack Overflow. Their valuable insights, code snippets, and solutions to various programming challenges have been immensely helpful in solving problems encountered during the development of this project.

Complete the tasks in the Python Notebook in this repository.
Make sure to add and push the pkl or text file of your scraped html (this is specified in the notebook)

## Rubric

* (Question 1) Article html stored in separate file that is committed and pushed: 1 pt
* (Question 2) Article text is correct: 1 pt
* (Question 3) Correct (or equivalent in the case of multiple tokens with same frequency) tokens printed: 1 pt
* (Question 4) Correct (or equivalent in the case of multiple lemmas with same frequency) lemmas printed: 1 pt
* (Question 5) Correct scores for first sentence printed: 2 pts (1 / function)
* (Question 6) Histogram shown with appropriate labelling: 1 pt
* (Question 7) Histogram shown with appropriate labelling: 1 pt
* (Question 8) Thoughtful answer provided: 1 pt
