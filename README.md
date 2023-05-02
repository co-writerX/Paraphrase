# Text Paraphrasing with Customizable Parameters

This project uses Spacy, T5-base, and NLTK to paraphrase text and score the output based on various factors. The code allows you to adjust the parameters to control the paraphrasing output.

## How it works

1. The text is split by its context using Spacy (for text longer than 2 sentences).
2. Set the mode and temperature (synonyms) - this sets the parameters for the model.
3. Paraphrase the text using T5-base (with options like top-k, top-p, beam search, and scoring).
4. Scoring is done using NLTK, considering factors like:
   - Fluency (Perplexity)
   - Coherence (Cosine Similarity)
   - Semantic Similarity (STS)
   - Diversity (N-Gram Overlap)
   - Creativity (Language Model Perplexity)
   - Readability (Flesch-Kincaid Grade Level)
   - Grammaticality (Grammatical Error Rate)
   - Formality (Use of Formal vs Informal Language)
   - Simplicity (Complexity of Sentence Structure and Vocabulary)
   - Common Word Choice (Lexical Diversity)

## Sample layout and options

The code provides various modes and temperature options to customize the paraphrasing output.

## Mode options:
   - Standard
   - Fluency
   - Formal
   - Simple

## Synonym (temperature) options:
   - Few
   - Standard
   - Many
   - All
