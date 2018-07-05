# Note

This work was proposed by Yang Li, Xiaoming Tao, Jianhua Lu and it was accepted by CyberneticsCom 2012.

I read this paper is because of the term "network grafting" which seems to be interesting and may be the related work in my research.

Li et al proposed a new neural network architecture based on transfer learning. They transferred the pretrained model to adapt to target task. I consider transferring neural network to be a form as transfer learning can be referred to many years ago, but the most impressing one is proposed by Yosinski et al in NIPS 2014[1]. This paper was proposed in 2012, so I think Li et al's work has certain novelty.

The actual method is to transfer both pretrained input layers and hidden layers to a new task.(called trunk) They grafed the pretrained part with another new hidden neuron plus another new output neuron to adapt to a target domain and then train the new neurons with target domain but fixed the wights in transfrred part. This kind of trasferring method is similar to Rusu et al.'s work[2] which used cascade-correlation architecture to handle multitask.

They used hold-out cross validation to evaluate their model, but k-fold cross validation is more popular and more general now.

They compared their network grafting method than TrAdaBoost and TrBagg and they claims their performance is better. Shown by Table III, I think the variance of grafting model is well. However, in general, the experiments are not enough to me. Maybe, conducting different aspects of experiment would be better.

# Reference
[1] Yosinski et al., How transferable are features in deep neural networks? [NIPS 2014]

[2] Rusu et al., Progressive Neural Networks [ICLR] 

[3] [cross-validation：从 holdout validation 到 k-fold validation](https://blog.csdn.net/lanchunhui/article/details/50522424)