# Projects 

## Academic Projects

### Evaluating Contextual Word Embeddings (Ongoing)
A research project aimed at understanding the properties of contextual word embeddings. The central question relates human linguistic knowledge and the information contained in these word embeddings: Given examples of an unknown word used in a sentence, humans can discern how many distinct meanings that word has, and can most often classify each example of the word as an instance of one meaning. Can we also determine, via many contextual embeddings of a word, how many meanings it has? Can we also classify word instances as having one of these meanings? If current word representations do not capture this information, how can we build word representations that do? Potential downstream applications include not only word sense disambiguation, but also analysis of polysemy in less-documented languages using unlabeled data.

### Imagenet Transfer Learning
<img src="/assets/img/vgg19.png" width="280" height="140">

A simple project with two goals:
1. Via transfer learning, train models to distinguish between two image classes.
2. Evaluate the performance of various pre-trained models, using multiple deep learning frameworks and hardware configurations.

For this project, I took image classification models (VGG19, mobilenet, and nasnet), and removed the last layer. I then created my own dataset with two classes (spiders and scorpions) not in the original dataset. I retrained these models on these image classes, and tracked training / inference time across different frameworks (tensorflow, theano, pytorch) and hardware (Nvidia GTX 1080Ti, Nvidia GTX 1080, Nvidia Tesla K80).

Source code and longer writeup available <a href='https://github.com/hannamw/imagenet-transfer-learning'>on github</a>.

### Classifying Document Sentiment
A project that I used to familiarize myself with machine learning / deep learning techniques. At its core, it performs simple text sentiment analysis. Reviews were drawn from various sections of Amazon, and their sentiment (in terms of simple positive / negative sentiment) was classified based on their rating (out of 5 stars).

In order to do this, I used various word / document representations. I used tf-idf representations and doc2vec representations to represent whole documents (reviews), and trained various machine learning models (logistic regression, SVM, random forest) on these. Then, I experimented with deep learning models, using pre-trained and totally new word embeddings.

### Language Detection
A toy project that detects the language that a text is written in. This is easy for some languages (e.g. English and Chinese, which will have almost no overlap even at the character level). However, other languages, like Bahasa Indonesia and Malay, are much more similar; they use the same alphabet and their texts look similar on first glance.

This simple tool uses an *n*-gram model to predict language, based on the intuition that while the total distribution of letters in a text in a given language may not perfectly predict the language, the distributions of *n*-grams, *n* letter sequences, predict language well.

## Software Engineering Projects

### Learn Hangul
<img src="/assets/img/Thumb.png" width="140" height="140">

A learning game (think Duolingo) that teaches you Hangul / 한글, the Korean alphabet. The game is written entirely in Elm, a purely functional language designed for reliable webapps with no runtime exceptions—a property of Elm that I hope you enjoy while playing this game!

This was developed as a project for CMSC 22300: Functional Programming. It does not yet include all elements of Hangul.

Play the demo [here](https://hannamw.github.io/demos/learn-hangul)!

### Othello
<img src="/assets/img/othello.png" width="140" height="140">

An implementation of the classic board game, Othello, in C. Play against a human, or a computer. The computer can be very hard to beat - at its hardest setting, it uses a minimax strategy that evaluates board states up to 6 moves in advance.

This program can found on <a href="https://github.com/hannamw/othello-in-c">github</a>, and is run from the command line.
