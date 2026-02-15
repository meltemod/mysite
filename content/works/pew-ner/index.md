---
title: "Computational methods for redacting identifying information in large text data"
date: 2026-02-15
summary: "Exploring techniques for anonymizing sensitive information in text datasets."
tags: ["data privacy", "NLP", "text analysis"]
featured_image: "featured.png"

organization: "Pew Research Center"
tools: ["R", "Python", "NLP libraries", "Hugging Face", "transformers"]

external_link: "https://www.pewresearch.org/decoded/2024/01/12/redacting-identifying-information-with-computational-methods-in-large-text-data/"
link_text: "View Blog Post →"
---
This blog post explains how researchers used computational methods to redact identifying information from unstructured text data, a set of 1,314 mission statements from U.S. K-12 school districts, before releasing it publicly. Removing identifiers like district names is straightforward in structured datasets, but much harder with free-form text because there are no fixed labels for names or addresses. To tackle this, the researcher combined three different techniques:

- Exact name matching against an external list of known district names,
- Named Entity Recognition (NER) with pretrained models to detect organization names, and
- Regular expressions to spot patterns like capitalized words preceding “school” or “district.”

Each approach had limitations on its own, so they were used together to maximize correctly redacted terms while minimizing false positives.

## What I did

I developed and evaluated scalable NLP approaches for detecting and removing personally identifiable information from large text corpora, and narrated the implications of these methods for research transparency and data privacy in a public-facing blog post.
