# similar-sent-generator
Similar sentences generator

- This notebook tries to generate similar sentences to a given input sentence. 
- It makes use of WordNet and GloVe embeddings to arrive at substitute words for candidate words in a sentence.
- Similarity threshold, and number of sentences generated can be controlled.

## Usage

- Install gensim, and nltk.
- Download GloVe embeddings (https://nlp.stanford.edu/projects/glove/).
- Run the included jupyter notebook.

## Configuration Options

* The main method which handles the input is: provide_alternate_sentence(...). This has the following modifiable parameters:
  * num_versions = Number of similar versions required. This is just a request, and cannot be guaranteed.
  * similarity_threshold = [0,1]. Higher value indicates closer sentences (this might also decrease the number of versions).

## Samples

Here are some of the samples generated through this tool:

Input: We collect your information regularly
Sample1: We collect your data regularly
Sample2: We gather your information regularly
Sample3: We gather your info regularly

Input: We collect your information regularly
Sample1: We collect your data regularly
Sample2: We gather your information regularly
Sample3: We gather your info regularly
