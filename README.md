# sparse_performance
Este repositório mostra a performance de diferentes modelos na atribuição de tokens (word-token weight dictionary for sparse embeddings)
Cada modelo foi aplicado a um dataset sample com 429 entradas do dgsi e +17M de caracteres no total (o texto em 'Decisão Texto Integral' foi concatenado entre todos os registos)

Em sparse_dictionary_tokens estão os dicionários de tokenização de palavras para diferentes modelos testados (com exatamente o mesmo nome que o do ficheiro sem .txt). Os modelos testados são: 

-bert-case-uncased (BM25) usado pelo James Briggs para hybrid search;

-splade-cocondenser-ensembledistil (SPLADE) usado pelo James Briggs para hybrid search;

-bert-large-portuguese-case - é general purpose: "pretrained BERT model for Brazilian Portuguese that achieves state-of-the-art performances on three downstream NLP tasks: Named Entity Recognition, Sentence Textual Similarity and Recognizing Textual Entailment"

-Legal-BERTimbau-sts-large-ma-v3 modelo com melhor performance média criada pelo Rui Melo na tese de mestrado "A Semantic Search System for Supremo Tribunal de Justiça"

 O melhor desempenho aparente para fazer sparse embeddings do sample dataset do dgsi é de longe o do modelo bert-large-portuguese-case.
