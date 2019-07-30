# Projects 
Here are some of my projects.

## Academic Projects

### Evaluating Contextual Word Embeddings (Ongoing)

### Imagenet Transfer Learning
A simple project with two goals:
1. Via transfer learning, train models to distinguish between two image classes.
2. Evaluate the performance of various pre-trained models, using multiple deep learning frameworks and hardware configurations.

For this project, I took image classification models (VGG19, mobilenet, and nasnet), and removed the last layer. I then created my own dataset with two classes (spiders and scorpions) not in the original dataset. I retrained these models on these image classes, and tracked training / inference time across different frameworks (tensorflow, theano, pytorch) and hardware (Nvidia GTX 1080Ti, Nvidia GTX 1080, Nvidia Kesta T80).

### Classifying Document Sentiment

### Language Detection
A toy project that detects

## Software Engineering Projects

### Learn Hangul
<img src="/assets/img/Thumb.png" width="140" height="140">

A learning game (think Duolingo) that teaches you Hangul / 한글, the Korean alphabet. The game is written entirely in Elm, a purely functional language designed for reliable webapps with no runtime exceptions—a property of Elm that I hope you enjoy while playing this game!


This was developed as a project for CMSC 22300: Functional Programming. It does not yet include all elements of Hangul.

Play the demo [here](https://www.classes.cs.uchicago.edu/archive/2019/spring/22300-1/showcase/mwhanna/index.html)!

### Othello
<img src="/assets/img/othello.png" width="140" height="140">

An implementation of the classic board game, Othello, in C. Play against a human, or a computer. The computer can be very hard to beat - at its hardest setting, it uses a minimax strategy that evaluates board states up to 6 moves in advance.

This program can found on <a href="https://github.com/hannamw/othello-in-c">github</a>, and is run from the command line.
