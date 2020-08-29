---
title: Integrate literate statistical programming into RStudio workflow
image: /assets/image.jpg
---

The simplest way to share your RStudio project directory is by pushing it to a remote repo on something like Github, and cloning it to your machine when you next need to work on it. 

This also has the additional advantage of allowing you to keep track of changes to your project.

R has a similar solution to Python’s virtualenvs called packrat which allows you to keep track of your analyses’ dependencies.


Be able to answer 5 questions about your research:
1. What did I do?
2. Why did I do it?
3. How did I set up everything at the time of the analysis?
4. When did I make changes, and what were they?
5. Who needs to access it, and how can I get it to them? 

# What is R Markdown? 

Like Python, R has its own tooling for literate statistical programming called R Markdown. Just like with Juypter notebooks, you can write chunks of markdown text alongside R code, meaning you can create easy-to-read, meaningful annotations for your analysis. You can also include results, tables and charts, allowing you to create reports and other documents from one self-contained R Markdown script.