This paper was proposed by Yoshua Bengio and they emphasized the importance of choosing appropriate samples in a meaningful order. (design approriate curriculum for model)

Curriculum Learning: When we train our agent/ML algorithms we can give our model simpler samples first, and then gradually raise the complexity of samples which means we expand the sample space and task difficulty gradually until the complexity is as same as our target problem.

How to apply?
Raise the sample policy (probability) of more difficult samples gradually, which means it will expand the sample space in our training procedure.

How to classify the complexity of samples?
- noisy or not
- diversity
- similarty to our target problem

The Advantage of Curriculum Learning:
- faster convergence
- could learn usually unlearnable task

Experiments:
- Shape recognition: from square, approriate size to rectangle and grey levels are more similar between foreground and background.
- Word prediction: expand the corpus gradually. it shows obvious improvement when it expand its corpus(# of words).


Curriculum learning could help to find better local minima of a highly non-convex criterion.


My opinions:
In Reinforcement Learning, self-play has succeeded in many throny problem. DeepMind use self-play to train AlphaGo Zero, and it needs less samples to reach much higher performance than use supervised learning before.

In self-play, the agent fights against itself, when it learning from scratch the rival is poor which is similar to use simpler sample to train the model. When the agent grows stronger, the rival is also stronger too. Just like the sample and the problem become more complicated and more difficult in Curriculum Learning.

Others:
1. How to identify the optimization problem is convex/non-convex?
- [research gate](https://www.researchgate.net/post/Identify_if_optimization_problem_is_convex_or_non-convex)
- [StackExchange](https://math.stackexchange.com/questions/1627493/identify-if-optimization-problem-is-convex-or-non-convex)

In this paper, it says: "training deep architecture involves a potentially intractable non-convex optimization problem".

2. Criterion in ML:


3. The importance of random seed in ML:
https://www.quora.com/What-does-the-seed-value-actually-mean-in-machine-learning-algorithm

4. Active Learning:
[Wikipedia](https://en.wikipedia.org/wiki/Active_learning_(machine_learning))

5. continuation method
[Wikipedia](https://en.wikipedia.org/wiki/Numerical_continuation)

Unknown:
1. Basin of Attraction
2. Attractor
