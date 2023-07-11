# Projects/Publications

## Academic Projects

### [How does GPT-2 compute greater-than?: Interpreting mathematical abilities in a pre-trained language model (ArXiv 2023)](https://arxiv.org/abs/2305.00586)
Pre-trained language models can be surprisingly adept at tasks they were not explicitly trained on, but how they implement these capabilities is poorly understood. In this paper, we investigate the basic mathematical abilities often acquired by pre-trained language models. Concretely, we use mechanistic interpretability techniques to explain the (limited) mathematical abilities of GPT-2 small. As a case study, we examine its ability to take in sentences such as "The war lasted from the year 1732 to the year 17", and predict valid two-digit end years (years > 32). We first identify a circuit, a small subset of GPT-2 small's computational graph that computes this task's output. Then, we explain the role of each circuit component, showing that GPT-2 small's final multi-layer perceptrons boost the probability of end years greater than the start year. Finally, we find related tasks that activate our circuit. Our results suggest that GPT-2 small computes greater-than using a complex but general mechanism that activates across diverse contexts.

### [The Functional Relevance of Probed Information: A Case Study (EACL 2023)](https://aclanthology.org/2023.eacl-main.58/)
Recent studies have shown that transformer models like BERT rely on number information encoded in their representations of sentences’ subjects and head verbs when performing subject-verb agreement. However, probing experiments suggest that subject number is also encoded in the representations of all words in such sentences. In this paper, we use causal interventions to show that BERT only uses the subject plurality information encoded in its representations of the subject and words that agree with it in number. We also demonstrate that current probing metrics are unable to determine which words’ representations contain functionally relevant information. This both provides a revised view of subject-verb agreement in language models, and suggests potential pitfalls for current probe usage and evaluation.

### [ACT-Thor: A Controlled Benchmark for Embodied Action Understanding in Simulated Environments (COLING 2022)](https://aclanthology.org/2022.coling-1.495/)
Artificial agents are nowadays challenged to perform embodied AI tasks. To succeed, agents must understand the meaning of verbs and how their corresponding actions transform the surrounding world. In this work, we propose ACT-Thor, a novel controlled benchmark for embodied action understanding. We use the AI2-THOR simulated environment to produce a controlled setup in which an agent, given a before-image and an associated action command, has to determine what the correct after-image is among a set of possible candidates. First, we assess the feasibility of the task via a human evaluation that resulted in 81.4% accuracy, and very high inter-annotator agreement (84.9%). Second, we design both unimodal and multimodal baselines, using state-of-the-art visual feature extractors. Our evaluation and error analysis suggest that only models that have a very structured representation of the actions together with powerful visual features can perform well on the task. However, they still fall behind human performance in a zero-shot scenario where the model is exposed to unseen (action, object) pairs. This paves the way for a systematic way of evaluating embodied AI agents that understand grounded actions.

### [A Fine-Grained Investigation of BERTScore (WMT 2021)](https://aclanthology.org/2021.wmt-1.59/)
BERTScore, a recently proposed automatic metric for machine translation quality, uses BERT, a large pre-trained language model to evaluate candidate translations with respect to a gold translation. Taking advantage of BERT’s semantic and syntactic abilities, BERTScore seeks to avoid the flaws of earlier approaches like BLEU, instead scoring candidate translations based on their semantic similarity to the gold sentence. However, BERT is not infallible; while its performance on NLP tasks set a new state of the art in general, studies of specific syntactic and semantic phenomena have shown where BERT’s performance deviates from that of humans more generally.

This naturally raises the questions we address in this paper: what are the strengths and weaknesses of BERTScore? Do they relate to known weaknesses on the part of BERT? We find that while BERTScore can detect when a translation exhibits poor choice of content words, it struggles to correctly penalize incorrect candidates when they are lexically similar to the reference, or only differ in function words.

### [Analyzing BERT's Knowledge of Hypernymy via Prompting (BlackboxNLP 2021)](https://aclanthology.org/2021.blackboxnlp-1.20)
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
