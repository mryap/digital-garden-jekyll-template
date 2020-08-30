---
title: Integrate literate statistical programming into RStudio workflow
image: /assets/image.jpg
---

# Reproducible Research 
Be able to answer 5 questions about your research:
1. What did I do?
2. Why did I do it?
3. How did I set up everything at the time of the analysis?
4. When did I make changes, and what were they?
5. Who needs to access it, and how can I get it to them? 

# GitHub - Remote Code Repositary

Share your RStudio project directory is by pushing it to a remote repo on [Github](/githubnotes), and cloning it to your machine when you next need to work on it. This also has the additional advantage of allowing you to keep track of changes to your project. 

# What is R Markdown? 

Like Python, R has its own tooling for literate statistical programming called R Markdown. Just like with Juypter notebooks, you can write chunks of markdown text alongside R code, meaning you can create easy-to-read, meaningful annotations for your analysis. You can also include results, tables and charts, allowing you to create reports and other documents from one self-contained R Markdown script.

## R Markdown

You can avoid copy-pasting tables (and all other analyses) by writing your reports using R Markdown instead of a word processor. R Markdown is a language for writing documents which include R code. The code is run, and the output is included in the document. R Markdown can be used to produce different types of document (e.g. reports, presentations, web pages), in various formats (e.g. Microsoft Word, PDF, HTML). The Research Methods in R worksheets are written using R Markdown, and although we don’t teach it in these materials, there are other courses which make it easy to learn.

# Alternatives

R has a similar solution to Python’s virtualenvs called packrat which allows you to keep track of your analyses’ dependencies.

# Data structures
R has many data structures. These include

    atomic vector
    list
    matrix
    data frame
    factors
