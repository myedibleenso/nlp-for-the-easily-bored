# ~~NLP~~ Information Extraction for the easily bored
NLP/IE workshop for the Tucson Data Science meetup (6/30/2016)

Please [fork this repository](https://help.github.com/articles/fork-a-repo/#fork-an-example-repository) and follow along.

**NOTE**: _this is a work in progress. Check back later for updates..._

# Table of Contents

_NOTE: When viewing the slides, it's easiest to advance using `fn`+ Down Arrow_
1. ~~NLP~~ Information Extraction for the easily bored
  - [slides](https://myedibleenso.github.io/nlp-for-the-easily-bored/slides/nlp-for-the-easily-bored.html) / [notebook](notebooks/nlp-for-the-easily-bored.ipynb)
   - How do we get useful things out of a sea of text?  
   - Learn about finding people, places, organizations, etc.

2. Introduction to `py-processors`

  - [slides](https://myedibleenso.github.io/nlp-for-the-easily-bored/slides/py-processors-intro.html) / [notebook](notebooks/py-processors-intro.ipynb)
   - An overview of the library for natural language processing (NLP) library we'll be using in the examples

## Examples

Here you'll find a few use cases illustrating the concepts covered in the intros.

1. Who, what, when, and where?  Making sense of web-based news
  - [slides](https://myedibleenso.github.io/nlp-for-the-easily-bored/slides/news-ie-example.html) / [notebook](notebooks/news-ie-example.ipynb)
  - go from `html` -> people, places, etc.  
  - Learn how to do basic IE on [an article you may have read from The Guardian](https://www.theguardian.com/world/2013/jun/09/edward-snowden-nsa-whistleblower-surveillance)
  - **Challenge**: How do we disambiguate organizations and people?

2. Getting structured information out of Wikipedia pages
  - [slides](https://myedibleenso.github.io/nlp-for-the-easily-bored/slides/wikipedia-ie-example.html) / [notebook](notebooks/wikipedia-ie-example.ipynb)
  - You now know a little about how to find named entities (people, places, organizations, etc.) in text, but how do these interact in text?  - **Challenge**: Try to populate a [Wikipedia infobox](https://en.wikipedia.org/wiki/Infobox#wikipedia) for [Barack Obama](https://en.wikipedia.org/wiki/Barack_Obama).
3. Movie reviews
  - [slides](https://myedibleenso.github.io/nlp-for-the-easily-bored/slides/rotten-tomatoes-example.html) / [notebook](notebooks/rotten-tomatoes-example.ipynb)
  - Is it a positive or negative review?  If we don't have a score, can we tell from the review text?
  - NOTE: To really get into this example, you'll need [a rotten tomatoes developer key](http://developer.rottentomatoes.com)
  - **Challenge**: Predict critics consensus scores based only on the review text
    - Use whatever method you want
        - feature-based classifier, latent feature model, etc.
    - What works _and **why**_?

# Installation

There a couple of things you'll need to run the notebooks in this repository...

## Requirements
- [Java 8](https://docs.oracle.com/javase/8/docs/technotes/guides/install/install_overview.html)
- 2 or 3GB of RAM available for running the NLP server

## Python dependencies via [`conda`](http://conda.pydata.org/miniconda.html)

```
conda create -n bored python=3
source activate bored
pip install -r requirements.txt
```

# Running the notebooks

The notebooks are all under `/notebooks`

If you want to run/alter them locally after installing the project dependencies, simply run this command:
```python
jupyter notebook
```
