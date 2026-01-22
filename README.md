


<!-- **DustinAngerhofer/DustinAngerhofer** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile. -->

Master's student in Mathematics | Transformer theory | Stochastic Processes | scientific ML

I am a Master's student in mathematics with four years of research and scientific computing experience with the Air Force Research Laboratory (AFRL).  My areas of practical expertise include self-supervised image representation learning, offline reinforcement learning, time series analysis, transformers, High-Performance Computing (HPC), Python, and dozens of scientific ML libraries. My theoretical expertise lies in probability theory, measure theory, Bayesian statistics, linear algebra, functional analysis, logic and metalogic. I am seeking to apply my skills to atmospheric science and climate modeling.

**Research Interests**
-Stochastic Processes, especially ones that are difficult for transformers to learn and model.
-Predictive modeling, especially climate modeling.
-Probability logic and applications, i.e. the development of probability theory as extensions of formal logics.

## Selected Projects
-**Diachronic Allignment of Probabilities in LLMs**

Suppose you ask an LLM for the probability of some proposition $Q$, and it returns a probability $p$. If, in that same context, you ask for the probability of $\neg Q$, it will likely return $1-p$, since it likely knows the basic rule that $P(Q) + P(\neg Q) = 1$ for all $Q$. If, however, you start a new context and then ask for the probability of $\neg Q$, you may find that it does not return $1-p$. In our experience, this is most often the case. In the first instance, the LLM was capable of consistent probabilistic reasoning because it is able to apply learned schemas of how probababilities should behave. We call this synchronic consistency--consistency within a single context. In the second instance, the LLM is not capable of consistent probabilistic reasoning because it is not capable of assigning probabilities to propositions in a consistent or robust manner. Whatever way the LLM is making those probability assignments, it is doing so in an irrational manner. This is what we call diachronic inconsistency--inconsistency across multiple contexts. Using reinforcement learning (particulary GRPO RLVR), we to train LLMs to be diachronically consistent and therefore more rational.

-**Successive-Rank Neural Networks**

In this project, we essentially perform Low-Rank Adaptation (LoRA), but without a pretrained model. That is, we start with a model whose weights are all rank-1 matrices, freeze the weights after training, inject a rank-1 update, and repeat. Inspired by the Singular Value Decomposition (SVD), the "singular vectors" comprising each rank-1 update are constrained to being orthogonal to those of all other updates, past and future. The idea is that, like the SVD, the model will learn the most important features in the first few ranks. In addition, these most important features are easily identified.
Repo link: https://github.com/DustinAngerhofer/Successive-Rank-Neural-Networks

-**Decoding Hidden Markov Models with Self-Attention Layers and Transformer Blocks**

The task at hand is to use a self-attention layer to predict the hidden states of a Hidden Markov Model (HMM) given the sequence of observed states. Our HMMs consist of k-ary Markov chains as the hidden states, and k-ary sequences as the observed states. What we find in practice is that both a single self-attention layer and a single transformer block get stuck in the naive solution. With a large enough embedding dimension, they seem to eventually find their way out. Repo link: https://github.com/DustinAngerhofer/HMM-Transformers
