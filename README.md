# Literature review
> This project helps review scientific literature efficiently.  Its purpose is to give scientists a quick way to process a large amount of literature.


## Install

`pip install literature_review`
> Note that this project uses GROBID, which should get automatically installed by text_extractor on first use.  However, if this fails, have a look at its [installation guide](https://grobid.readthedocs.io/en/latest/Install-Grobid/).  GROBID also requires Java Virtual Machine (versions 8 to 11 are suported). On a mac the easiest way to install it is via homebrew: `brew install adoptopenjdk/openjdk/adoptopenjdk11`):

## How to use

Fill me in please! Don't forget code examples:

```python
# Extract text information from pdfs
from literature_review.text_extractor import extract_texts
from literature_review.article import make_articles


#extract_texts('../data/raw/','../data/interim/article_dicts')

# Review 
articles = make_articles('../data/interim/article_dicts/')
ad = Article_Displayer(articles, 
                       checks = ['AAT','AAT_uncertain','split-half','retest','reliability_uncertain'],
                      search = r'\brelia\w+')
```


    ---------------------------------------------------------------------------

    NameError                                 Traceback (most recent call last)

    /var/folders/16/2wxbnpk5321f8g40bxf0ht_h0000gn/T/ipykernel_75042/2117848704.py in <module>
          4 
          5 # Review
    ----> 6 articles = make_articles('../data/interim/article_dicts/')
          7 ad = Article_Displayer(articles, 
          8                        checks = ['AAT','AAT_uncertain','split-half','retest','reliability_uncertain'],


    NameError: name 'make_articles' is not defined

