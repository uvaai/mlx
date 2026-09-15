
## Interpretable AI

As you've read in the writing assignment from the previous module, current AI
legislation also provides the right to an explanation in the case of an
automated decision. And, in many applications, being able to explain why a
certain prediction was made can be very valuable, as it can help humans to
assess whether they think that prediction is correct, or even desirable for the
system to make (in the case of biases, for instance).

As you might imagine, making the predictions of a neural network explainable is
actually very difficult to do. This type of model is also called a *black box*
model, where a sample goes in, and a prediction comes out, but you can't really
say much about what exactly happens in the middle. There are just way too many
neurons, each with their own weights, to really explain why the network made
that exact prediction.

This has led to recent research into how to make AI systems explainable, which
has resulted in several different methods to generate an explanation for a
black box model. For example:

* Determining what features in the testing sample, or which specific samples
from the training data were relevant for this prediction.
* Interpreting or visualizing the internal structure or weights of the model in
some way as to give insight in what has actually been learned.
* Learning an interpretable model that comes very close to the results of 
the original black box model for (some part of) the problem and then interpret
that model instead.

To get a better introduction to these types of methods, we'll read some
sections from the
[Interpretable Machine Learning Book](https://christophm.github.io/interpretable-ml-book/)
by Christoph Molnar. Start by reading the following sections from the book:

* 2: Interpretability 
* 4: Methods Overview
* 9: Decision Tree
* 25: Surrogate Models

Cynthia Rudin from Duke University wrote an article advocating a different
position, namely to stop using black box models altogether, whenever possible,
for any situation where explanations might be needed. Read the article linked
here:
[Cythia Rudin - Stop Explaining Black Box Machine Learning Models for High Stakes Decisions and Use Interpretable Models Instead](https://arxiv.org/abs/1811.10154).

The article makes some interesting claims. For each of the claims listed below,
state whether you agree or disagree with that claim. Motivate your answers.

1. Even explanation models with relatively high agreement with the black box
model, still disagree for some samples, and therefore you cannot trust these
explanations, and by extension cannot trust the original black box model.

2. If a pattern in the data is important enough for the black box model to
leverage to provide better predictions, then a machine learning researcher
might also extract this same pattern and create an accurate-yet-interpretable
version of the model.

3. Governments should regulate the use of black box models, either enforcing
that no black box should be deployed when there exists an interpretable model
with the same level of performance, or just mandating that organizations that
introduce black box models should also report the accuracy of interpretable
modeling methods.

Your assignment should be long enough to make a clear and cohesive argument for
your point of view. In general, this tends to correspond with around 500 words. 
The minimum requirement for the assignment is 350 words.

#### Peer review

You are encouraged to swap writing assignments with other students, read them
and share feedback with each other, both on the contents of the arguments and
the structure of the writing. Writing a good text can be difficult and,
especially after you rewrote something a couple of times, other people will
generally see improvements that you can't spot anymore. So, make use of that
and help each other out by exchanging feedback.

