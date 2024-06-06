# NLP with nltk python

My learning notes for natural language processing with sentiment analysis project

## Table of Contents

1. [Introduction](#introduction)
2. [Ambiguity and uncertainty in language](#ambiguity-and-uncertainty-in-language)
3. [NLP Process Phases](#nlp-process-phases)
4. [Core Concept in NLP and NLTK](#core-concept-in-nlp-and-nltk)
   - [Tokenizing](#tokenizing)
   - [Stop Words](#stop-words)
   - [Stemming](#stemming)
   - [Lemmatization](#lemmatization)
   - [Chunking](#chunking)
   - [Chinking](#chinking)
   - [Named Entity Recognition (NER)](#named-entity-recognition-ner)
   - [Concordance](#concordance)
   - [Dispersion plot](#dispersion-plot)
   - [Frequency distribution](#frequency-distribution)
   - [Collocation](#collocation)

## Introduction

NLP (Natural Language Processing) is a field of study that focused on teaching computers to understand human language.

### Ambiguity and uncertainty in language

Ambiguity means that a text can be understood in more than one way.

- **Lexical ambiguity**

It means that ambiguity happens with one word.

- **Syntactic ambiguity**

It means that ambiguity happens because a sentence can be parsed in different ways.
For example, "I see a women with a sunglasses." Does it mean that I am using sunglass or the women is using sunglass?

- **Semantic ambiguity**

It means that a sentence has ambiguous word that makes the sentence become ambiguous.
For example, "The car hit the people while **it's** moving." The bold word make it ambiguous.

- **Anaphoric ambiguity**

It means ambiguity that happend because a sentence uses anaphoric words or words that refer to earlier sentences.
For example, "The cat run in the roads. **It's** very steep. **It** soon gets tired."

- **Pragmatic ambiguity**

It means that the statement is not specific.
For example, "I like you too" can mean that i like you just as you like me or just like other person like me.

### NLP Process Phases

Morphological process -> Syntax analysis (lexicon, grammar) -> Semantic analysis (Semantic rules) -> Pragmatic analysis (Contextual information)

- **Morphological processing**

This phase breaks down language into tokens that correspondend with paragraphs, sentences and words.
For example, into is broken down into "**in-to**".

- **Syntax analysis (parsing)**

This phase checks if a sentence is well-formed and break it up to to show different syntactic relationships
between different words.

- **Semantic analysis**

This phase checks the meaning of the words in the text using dictionary.

- **Discourse integration**

This phase check meaning of sentences in relation to preceding and succeeding sentences.

- **Pragmatic analysis**

This phase reinterprets what sentence means with real-world knowledge.

## Core Concept in NLP and NLTK

## Tokenizing

By tokenizing, you split up text by word or sentence. Tokenizing by sentence can analyze how words relate to one and another with more context.
In nltk library, you can use this syntax

> > > from nltk.tokenize import sent_tokenize, word_tokenize

## Stop Words

Common words that you want to ignore like 'is', 'the', 'an'.
nltk:

> > > nltk.download("stopwords")
> > > from nltk.corpus import stopwords
> > > from nltk.tokenize import word_tokenize

## Stemming

Reduce words into root word. Stemming dont use dictionary reference for words. For example, reduce words "helping", "helper" into "help".
nltk:

> > > from nltk.stem import PorterStemmer

## Lemmatization

Reduce words into root word using dictionary reference.

## Chunking

While tokenizing allows you to identify words and sentences, chunking allows you to identify phrases.

NP Chunking means searching chunks that corresponding to individual noun.

## Chinking

Chinking is used to exclude pattern in text.

## Named Entity Recognition (NER)

Named entities are noun phrases that refer to specific organization, places, person, etc.
Named Entity Recognition can find the named entities in texts and determined what kind of named entity they are.

## Concordance

To see how many times that word has been used

## Dispersion plot

To see multiple Concordance plot

## Frequency distribution

To check which word show up most frequently

## Collocation

Sequence of words that show most often
