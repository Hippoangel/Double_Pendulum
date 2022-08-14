# Double Pendulum with DL

## AI and non-linear dynamics

> ML & DL was a hot potato since '10 and so many scholars and computer engineer faced new challenged to understand the non-linear dynamics. 

Especially, Edward Ott from MD, USA published the paper:**Using Machine Learning to Replicate Chaotic Attractors and Calculate Lyapunov Exponents From Data** **([arXiv:1710.07313](https://arxiv.org/abs/1710.07313))** about the chaotic problem by applying ML & DL.

 Even his works were successful and proved that ML&DL models can calculate the complex and chaotic incident. But, it was really naive and basic cornerstone. For it's clear that he figured out ML&DL model is good solution to calculate the chaotic case, but this model is simply for one case and it is not sure that every non-linear dynamics are appropriate to adopt such a method.



## LSTM & LSTM-AutoEncoder

> Let's concern these problems from bottom. Issac Newton proposed noble way to understand the real world - differential equation. But, ODE faced the impossible challenge - non-linear dynamics. Poincaré proved that such a problems are impossible to solve under the algebraic structures. 

But as we saw in the paper by Edward Ott that deep-learning models are good for calculating really complex problem. I am likely to insist that be never a coincide. There could contain such a good mathematical relationship. William Gropp in Illinois **([Deep-Learning-with-Real-Data-and-The-Chaotic-Double-Pendulum](https://cloud4scieng.org/2021/02/28/deep-learning-with-real-data-and-the-chaotic-double-pendulum/))** point configuration space structure out for LSTM or DL to be able to calculate ODE even it is nonlinear and chaotic. 

 So, I tried to prove that is true or not. I made the real double-pendulum device with Aluminum. With Arduino sensors we gauged its velocity and accelerator. And I made deep learning model to analysis the real data. 

## How can it be possible?

 As the every general physics books said, air resistance is non-conservative and its hamiltonian is not so easily defined. But, we calculated. I think this is really big clue that William Gropp insisted in his article. There is **some good geometrical structure** in dynamics systems, that is reason why we can calculate something really complex circumstance. 

Plus, some physicist proposed that some constraints are calculable. [Nonconservative  Lagrangian and Hamiltonian Mechanics](https://journals.aps.org/pre/abstract/10.1103/PhysRevE.53.1890) is good example of them. So, it imply that we could build a good model for dynamics system.


## Further

Corresponding to my curioisty, S.Greydanus proposed Hamiltonian Neural Networks(2019)([arXiv:1906.01563](https://arxiv.org/abs/1906.01563)) - HNN -. This paper adopted hamiltonian as kind of activation function, which is application that hamiltonian is the generator of time. By compare to baseline neural network, he proved that his HNN is superior to other models.

Similary, M.Lutter published Deep Lagrangian Networks: Using Physics as Model Prior For Deep Learning([arXiv:1907.04490])(https://arxiv.org/abs/1907.04490). Also it is similar to Greydanus' paper, Lagrangian is kind a good key to calculate the hamiltonian. 

Otherwise, reservoir learning by Auto-Encoder is also tried to find out the best way to understand physical problems. Joseph Bakarji published Discovering Governing Equations from Partitial Measurements with Deep Delay Autuencoders(arXiv:2201.05136) which is fancy application of takens' theorm. 

