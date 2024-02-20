# Clothing Similarity Comparison

Clothes similarity search provides ranked recommendations based on the description of the clothing provided from the database. This repository contains the source code for:

- Data Scraper
- Sentence Encoder
- Similarity Function

### Data Scraper

**Data scraper** makes use of the data available on [H&M website](https://www2.hm.com/en_in/index.html).

The scraped data is further feature-engineered and preprocessed to generate a wordSoup for representational encoding and is stored in the column _cleaned_text_

### Encoder

**Encoder** uses Tfidf-Vectorizer to generate sentence embeddings for every product description of size _1 x MAX_FEATURES_ _(default = 1000)_.

### Similarity Function

**Similarity Function** utilizes cosine similarity by _scikit-learn_ to generate a similarity measure between the **product description** and the **database** and provide n-ranked results to the user.


## Installation

To use util functions and scripts such as _the scraper_ and _the encoders_, clone this repository to your local environment to get started:

```
git clone https://github.com/catlover75926/Clothes-Similarity-Comparison.git
```

After creating a virtual environment in the cloned repository, install the dependencies as:

```
pip install -r requirements-script.txt
```

Developed by Conrad Takashi(https://discord.com/users/382102787649175553)


<img src="img/similarity.JPG" width="600">