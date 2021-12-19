# Projects/Publications

## Academic Projects

### <a href='https://www.statmt.org/wmt21/pdf/2021.wmt-1.59.pdf'>A Fine-Grained Investigation of BERTScore (WMT 2021)</a>
BERTScore, a recently proposed automatic metric for machine translation quality, uses BERT, a large pre-trained language model to evaluate candidate translations with respect to a gold translation. Taking advantage of BERT’s semantic and syntactic abilities, BERTScore seeks to avoid the flaws of earlier approaches like BLEU, instead scoring candidate translations based on their semantic similarity to the gold sentence. However, BERT is not infallible; while its performance on NLP tasks set a new state of the art in general, studies of specific syntactic and semantic phenomena have shown where BERT’s performance deviates from that of humans more generally.

This naturally raises the questions we address in this paper: what are the strengths and weaknesses of BERTScore? Do they relate to known weaknesses on the part of BERT? We find that while BERTScore can detect when a translation exhibits poor choice of content words, it struggles to correctly penalize incorrect candidates when they are lexically similar to the reference, or only differ in function words.

### <a href='https://aclanthology.org/2021.blackboxnlp-1.20/'>Analyzing BERT's Knowledge of Hypernymy via Prompting (BlackboxNLP 2021)</a>
The high performance of large pretrained language models (LLMs) such as BERT on NLP tasks has prompted questions about BERT’s linguistic capabilities, and how they differ from humans’. In this paper, we approach this question by examining BERT’s knowledge of lexical semantic relations. We focus on hypernymy, the “is-a” relation that relates a word to a superordinate category. We use a prompting methodology to simply ask BERT what the hypernym of a given word is. We find that, in a setting where all hypernyms are guessable via prompting, BERT knows hypernyms with up to 57% accuracy. Moreover, BERT with prompting outperforms other unsupervised models for hypernym discovery even in an unconstrained scenario. However, BERT’s predictions and performance on a dataset containing uncommon hyponyms and hypernyms indicate that its knowledge of hypernymy is still limited.

## Software Engineering Projects

### Learn Hangul (2019)
<img src="/assets/img/Thumb.png" width="140" height="140">

A learning game (think Duolingo) that teaches you Hangul / 한글, the Korean alphabet. The game is written entirely in Elm, a purely functional language designed for reliable webapps with no runtime exceptions—a property of Elm that I hope you enjoy while playing this game!

This was developed as a project for CMSC 22300: Functional Programming. It does not yet teach all elements of Hangul.

Play the demo [here](https://hannamw.github.io/demos/learn-hangul)!

### Othello (2017)
<img src="/assets/img/othello.png" width="140" height="140">

An implementation of the classic board game, Othello, in C. Play against a human, or a computer. The computer can be very hard to beat - at its hardest setting, it uses a minimax strategy that evaluates board states up to 6 moves in advance.

This program can found on <a href="https://github.com/hannamw/othello-in-c">github</a>, and is run from the command line.
