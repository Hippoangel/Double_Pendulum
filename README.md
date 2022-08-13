# Double Pendulum with DL

## AI and non-linear dynamics

ML & DL was a hot potato since '10 and so many scholars and computer engineer faced new challenged to understand the non-linear dynamics. Especially, Edward Ott from MD, USA published the paper:Using Machine Learning to Replicate Chaotic Attractors and Calculate Lyapunov Exponents From Data **([arXiv:1710.07313](https://arxiv.org/abs/1710.07313))** about the chaotic problem by applying ML & DL. Even his works were successful and proved that ML&DL models can calculate the complex and chaotic incident. But, it was really naive and basic cornerstone. For it's clear that he figured out ML&DL model is good solution to calculate the chaotic case, but this model is simply for one case and it is not sure that every non-linear dynamics are appropriate to adopt such a method.



## LSTM & LSTM-AutoEncoder

Let's concern these problems from bottom. Issac Newton proposed noble way to understand the real world - differential equation. But, ODE faced the impossible challenge - non-linear dynamics. Poincaré proved that such a problems are impossible to solve under the algebraic structures. But as we saw in the paper by Edward Ott that deep-learning models are good for calculating really complex problem. I am likely to insist that be never a coincide. There could contain such a good mathematical relationship. William Gropp in Illinois **([article](https://cloud4scieng.org/2021/02/28/deep-learning-with-real-data-and-the-chaotic-double-pendulum/))** point configuration space structure out for LSTM or DL to be able to calculate ODE even it is nonlinear and chaotic. 

 So, I tried to prove that is true or not. I made the real double-pendulum device with Aluminum. With Arduino sensors we gauged its velocity and accelerator. And I made deep learning model to analysis the real data. 

## How can it be possible?

As the every general physics books said, air resistance is non-conservative and its hamiltonian is not so easily defined. But, we calculated. I think this is really big clue that William Gropp said in his article. 

https://journals.aps.org/pre/abstract/10.1103/PhysRevE.53.1890


## HNN
