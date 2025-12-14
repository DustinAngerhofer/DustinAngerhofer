


<!-- **DustinAngerhofer/DustinAngerhofer** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile. -->

Master's student in Mathematics | Transformer theory | Stochastic Processes | scientific ML

I am a Master's student in mathematics with four years of research and scientific computing experience with the Air Force Research Laboratory (AFRL).  My areas of practical expertise include self-supervised image representation learning, offline reinforcement learning, time series analysis, transformers, High-Performance Computing (HPC), Python, and dozens of scientific ML libraries. My theoretical expertise lies in probability theory, measure theory, Bayesian statistics, linear algebra, functional analysis, logic and metalogic. I am seeking to apply my skills to atmospheric science and climate modeling.

**Research Interests**
-Stochastic Processes, especially ones that are difficult for transformers to learn and model.
-Predictive modeling, especially climate modeling.
-Probability logic and applications, i.e. the development of probability theory as extensions of formal logics.

## Selected Projects
-**Successive Rank Neural Networks**

In this project, we essentially perform Low-Rank Adaptation (LoRA), but without a pretrained model. That is, we start with a model whose weights are all rank-1 matrices, freeze the weights after training, inject a rank-1 update, and repeat. Inspired by the Singular Value Decomposition (SVD), the "singular vectors" comprising each rank-1 update are constrained to being orthogonal to those of all other updates, past and future. The idea is that, like the SVD, the model will learn the most important features in the first few ranks. In addition, these most important features are easily identified.
[https://github.com/DustinAngerhofer/Successive-Rank-Neural-Networks]
