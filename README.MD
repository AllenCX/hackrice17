Identify the Painting with Deep Learning 

1. The general approach

In order to give a probability whether the two paintings are painted by the same artist, from the view of machine learning, we need a model which the inputs are the pair of paintings and the output ideally is a number indicates a probability (target output).

2. Pre-trained model
Using Inception v3 as a pretrained model, subsitute the original output layer with a single output sigmoid layer yields the probability.

3. Randomly sample negative and positive examples, with 1 : 1 or 2 : 1 ratio, labels them with 1 or 0. Then train it.