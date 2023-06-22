# LatinCy Video Tutorial

To help you get started with LatinCy, I have created a Jupyter notebook that walks you through the basics of using LatinCy with spaCy. You can find this notebook in this repository.

For a more in-depth look at how to use LatinCy, you can watch the following video tutorial. Click on the thumbnail below to watch the video on YouTube.

[![LatinCy Tutorial](https://img.youtube.com/vi/4vOlGZGZpvg/0.jpg)](https://www.youtube.com/watch?v=4vOlGZGZpvg)

## About LatinCy

LatinCy is a new spaCy project created by Patrick J. Burns, designed to work with Latin texts in spaCy natively. This project aims to facilitate Latin text analysis by providing an intuitive and straightforward interface for accessing spaCy's powerful features.

For more information about Patrick J. Burns, please refer to his profile on the [ISAW NYU website](https://isaw.nyu.edu/people/staff/patrick-burns).

You can find the original project on the [spaCy Universe page](https://spacy.io/universe/project/latincy).

## Installation

To use LatinCy, first, you need to install it. You can install LatinCy using pip:

```
pip install https://huggingface.co/latincy/la_core_web_lg/resolve/main/la_core_web_lg-any-py3-none-any.whl
```

You also need to have spaCy installed. If you don't have it installed, you can do so by running:

```
pip install spacy
```

## Usage

LatinCy integrates directly with spaCy, allowing you to use its powerful features with Latin texts natively.

Here is an example of how to use it:

```python
import spacy
nlp = spacy.load('la_core_web_lg')
doc = nlp('Haec narrantur a poetis de Perseo')

print(f'{doc[0].text}, {doc[0].norm_}, {doc[0].lemma_}, {doc[0].pos_}')

# > Haec, haec, hic, DET
```
