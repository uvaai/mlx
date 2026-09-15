# AlphaGo

I hope that during the past few written assignments it has become clear that
one of the difficult things about creating an Artificial Intelligence is having
a good definition of intelligence in the first place. Philosophers like Searle
might argue that understanding requires intentionality or consciousness, but
neuroscientific theories of consciousness to the level of detail that we could
simulate them on a computer, currently still seem very much like science
fiction, or in some theories, even impossible by definition. While this
philosophical question is an interesting one to consider, it is far from
settled, if it even ever will be, so we’ll instead consider more pragmatic
definitions of intelligence next.

Historically, AI researchers have taken intelligence to be a general
problem-solving ability. A new research challenge would be defined by taking a
task humans are good at, but we don’t know how to get computers to solve, and
then try and program computers to solve it. This might be a problem of
translating a complete Dutch sentence to a sentence in English using proper
grammar (which would be machine translation, natural language processing) or
recognizing an individual person based on just the pixel values of an image
of their face (which would be facial recognition, computer vision). Both are
complex problems requiring very technical algorithms to solve, but some
solutions to these problems are publicly available and you might even use them
in your everyday life already.

The argument here is that if we can solve many of these complex problems in a
general way, i.e. using the same algorithms and representations for all of
them, then at some point the program will be indistinguishable from, or even
better than, human intelligence. The result probably will not function in the
same way a human intelligence does, but if it is equally capable of solving
problems within the real world, then it must also possess some form of
intelligence.

## AI and games

Games are very often used as such challenges for intelligence in AI, because
programming the basic rules of a game is usually easy and the challenge has a
very clear goal (win the game). However, finding a strategy with which you can
win, is usually much harder. The classic example here is the game of chess,
which was "solved" in 1997 when the computer *Deep Blue* beat Garry Kasparov,
who at that time was ranked the best player in the world. Most of the
victory of *Deep Blue* is usually attributed to the increases in computational
power at the time, and not the algorithm that *Deep Blue* was running, which
was relatively simple. This is a recurring problem in AI of course; once a
problem is solved, then we can understand the solution and say this solution
wasn't actually intelligent.

In order to avoid this type of *computational horsepower* solution, the next
big challenge became the game of Go. Go is a much harder game to solve in a
purely computational way, because there are so many possible moves every turn.
In fact, there are more possible Go board positions ($10^{170}$) than atoms in
the universe ($10^{80}$), and even, more possible positions than the number of
atoms in the universe squared $(10^{80})^2 = 10^{160}$. Despite this insanely
large number of possibilities, in 2016 the computer program *AlphaGo* managed
to beat a top ranked human player in a best of 5 series of games. This was
considered by many to be a problem which was still at least a decade away from
being solved, so the success was big news. DeepMind, the company that made
*AlphaGo*, has made a documentary on these historic 5 games, which will be the
viewing material for this week:

![embed](https://www.youtube.com/embed/WXuK6gekU1Y)

## Creative AI

First, let's try and link this complex algorithm back to the linear regression
algorithm we discussed this week, where we learn to predict a y-value based on
some x-value, given a set of training examples. This algorithm instead tries to
predict how likely the human player is to play a certain move, and how likely
the program is to win the game, which are both also just numbers we can use as
regression targets, and uses the current state of the board (i.e. which pieces
are placed where) as the function input. These are of course *much* harder
functions to try and learn, and they definitely won’t have a straightforward
set of training examples, but it *is* possible. The algorithm still uses
*gradient descent* to try and find the minimum of some cost function, and the
whole system actually works surprisingly similar to linear regression, even if
the model is much more complicated. Once we have learned these functions, we
can simply select the next move that will result in the board state with the
highest probability of winning the game.

This explanation is a little oversimplified in places, but the core algorithm
really does just approximate the parameters of these functions using gradient
descent. The hard part is of course getting the right training data, which in
part was a large collection of games played by humans. In addition, the
algorithm played versus itself many, many times, in order to get a better
estimate of what the win probabilities of certain board states are. This
allowed the algorithm to also explore new strategies and not just learn from
human games.  Because the number of positions is *so* large, the last essential
component was the ability to generalize the complex board patterns to new board
positions, which it might not have specifically seen before, but perhaps it did
see situations which were *similar*.

Given this understanding of the algorithm, consider if move 37 is actually
creative. It is a move that is extremely unlikely for humans to play, but did
get a high probability of winning in AlphaGo when playing many games versus
itself. Is an unlikely sequence of music notes that still sounds good (given a
data set or metric for "sounding good") creative? Apparently, world experts
would characterize this specific move as being creative, which in a sense is
the highest bar we could possibly set for such a system.

For your written assignment this week, argue whether or not you think move 37
is creative. Search online for some definitions of creativity and cite at least
one definition that matches your own. These may just be dictionary definitions
and do not have to come from scientific papers, as long as you can compare
whether move 37 is creative or not according to this / these definitions.

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

