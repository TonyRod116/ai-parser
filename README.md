# AI Parser

A natural language parser implementation using NLTK (Natural Language Toolkit) for Harvard's AI course.

## Description

This project implements a context-free grammar parser that can analyze English sentences and extract noun phrase chunks. The parser uses predefined grammar rules to parse sentences and identify syntactic structures.

## Features

- Context-free grammar parsing using NLTK
- Noun phrase chunk extraction
- Support for reading sentences from files or interactive input
- Preprocessing of input text (lowercase conversion, filtering)

## Files

- `parser.py` - Main parser implementation
- `requirements.txt` - Python dependencies
- `sentences/` - Directory containing sample sentences for testing

## Grammar Rules

The parser uses a simplified grammar with the following components:

### Terminals
- Adjectives (Adj): country, dreadful, enigmatical, little, moist, red
- Adverbs (Adv): down, here, never
- Conjunctions (Conj): and, until
- Determiners (Det): a, an, his, my, the
- Nouns (N): armchair, companion, day, door, hand, he, himself, holmes, home, i, mess, paint, palm, pipe, she, smile, thursday, walk, we, word
- Prepositions (P): at, before, in, of, on, to
- Verbs (V): arrived, came, chuckled, had, lit, said, sat, smiled, tell, were

### Non-terminals
- S -> N V (Simple sentence structure)

## Usage

### Install Dependencies
```bash
pip install -r requirements.txt
```

### Run the Parser

1. **Interactive mode:**
   ```bash
   python parser.py
   ```
   Then enter a sentence when prompted.

2. **File mode:**
   ```bash
   python parser.py sentences/1.txt
   ```

## Implementation Status

The project includes the basic structure and grammar definitions. The following functions need to be implemented:

- `preprocess(sentence)` - Convert sentence to list of words with preprocessing
- `np_chunk(tree)` - Extract noun phrase chunks from parse tree

## Sample Sentences

The `sentences/` directory contains sample text files that can be used to test the parser functionality.

## Course Context

This project is part of Harvard's AI course curriculum, focusing on natural language processing and syntactic analysis.
