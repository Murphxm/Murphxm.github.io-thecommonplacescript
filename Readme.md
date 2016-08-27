
# The Commonplace Script

This is my project for "Get a book out will ya" my initial reason for choosing the specific books was for self learning purposes.
Inspired by stories of AI I wanted this to be my main focus.
That was when I remembered Sunspring (https://www.youtube.com/watch?v=LY7x2Ihqjmc) the creator of this film was Benjamin, a neural net.
I learned about Ross Goodwin(https://github.com/rossgoodwin) and I tried to find some demonstrations of his program on github to no avail.
So I continued learning about various ways in which this sort of program could work, natural language generation, deep learning, markov chains, LSTM and RNN networks. All of which I had absolutely no experience and almost all of which were programmed in python or node...

It was then that I miraculously found recurrentJS by Karpathy(http://cs.stanford.edu/people/karpathy/recurrentjs), an LSTM and RNN network that is programmed fully in javascript(the only language I'm good at)

  RecurrentJS
  The core of the library is a **Graph** structure which maintains the links between matrices and how they are related through transformations. Another important building block is the **Mat** class which represents a 2-dimensional `N x D` matrix, its values in field `.w` and its derivates in field `.dw`. Here is how you would implement a simple Neural Network layer:
  - Deep **Recurrent Neural Networks** (RNN)
  - **Long Short-Term Memory networks** (LSTM)
  - In fact, the library is more general because it has functionality to construct arbitrary **expression graphs** over which the library can perform **automatic differentiation** similar to what you may find in Theano for Python, or in Torch etc. Currently, the code uses this very general functionality to implement RNN/LSTM, but one can build arbitrary Neural Networks and do automatic backprop.

Now using the recurrentjs demo and a javascript based pdf to text converter I am working to hack together a version that will be able to take multiple texts and then output a "hybrid" text(around 1000 words) based on the nuances of the provided texts. This will potentially create interesting connections and/or ideas that can be elaborated further.

Ideas I would like to implement:
- Multiple PDF file to text inputs working effectively
- PDF outputting directly into the text analysis section of recurrentjs
- Output from recurrent being in the form of one large body of text as opposed to sentences (maybe display an array of sentences?)

## Warning: Beta

This code works fine, but it's a bit rough around the edges - you have to understand Neural Nets well if you want to use it and it isn't beautifully modularized. I thought I would still make the code available now and work on polishing it further later, since I hope that even in this state it can be useful to others who may want to browse around and get their feet wet with training these models or learning about them.

## License
MIT
