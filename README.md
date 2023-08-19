# Custom Named Entity Recognition (NER) Model using spaCy

Welcome to the Custom Named Entity Recognition (NER) Model project built using spaCy! This repository contains code and resources for training a custom NER model to extract specific entities from text.

## Project Overview

This project aims to develop a specialized Named Entity Recognition (NER) model using the spaCy library. The primary goal is to extract domain-specific entities, such as names of people, organizations, locations, or any other relevant entities, from text data.

## Getting Started

import spacy

nlp = spacy.load("custom_ner_model")
text = "Apple is planning to open a new store in New York."
doc = nlp(text)

for ent in doc.ents:
    print(ent.text, ent.label_)
    
spacy.displacy.render(doc, style='ent')

### Installation

To get started, you'll need to install the required dependencies. You can do this using the following commands:
Install Spacy & en_core_web_lg Model

```bash
pip install spacy
python -m spacy download en_core_web_lg  # Download the spaCy English model


Retrain the Model with your own data
