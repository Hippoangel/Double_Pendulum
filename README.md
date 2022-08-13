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

이러한 고전적인 접근방식 외에 주목할만한 논문으로 첫번째, S. Greydanus가 2019년에 발표한 Hamiltonian Neural Networks([arXiv:1906.01563](https://arxiv.org/abs/1906.01563)) – 이하 HNN- 가 있다. 이 논문은 딥러닝 모델에서 Activation Function으로 해밀토니안을 적용하여 카오스 이론의 예측에 사용할 수 있다는 주장을 한다. 그는 해밀토니안이 시간의 생성자임을 이용하여 물리학적 현상을 예측하는데 HNN을 활용하여 주어진 시스템의 다음을 예측할 수 있다고 주장하였다. 그는 일반적인 baseline 딥러닝 모델과 그가 주장한 HNN을 비교 하였고, baseline의 방법론을 동원한 딥러닝 보다 그의 모델이 우월함을 증명함과 동시에 실제 고전적인 수치해석적 모델과도 잘 맞아 떨어짐을 증명하였다.

동일한 결과는 비슷한 시기 M.Lutter가 발표한 Deep Lagrangian Networks: Using Physics as Model Prior For Deep Learning(arXiv:1907.04490)에서도 나타난다. 그는 Deep Lagrangian Network -이하 DeLaN-을 이용하였고, 라그랑지언으로 쉽게 해밀토니안을 계산할 수 있다는 원리, Greydanus와 동일하게 해밀토니안이 시간의 생성자임을 이용하여 변환을 가하면 다음 운동을 예측할 수 있다는 원리를 주장하였다. 또 그는 이러한 방식으로 2개의 축이 있는 이중진자적 결과를 사용해야하는 복잡한 로봇역학에 적용할 수 있다는 가설을 내놓았다. 이렇듯, 최근에는 이런 물리학적 모델을 활용하여 보다 정밀한 물리학적 현상을 예측하는  경우에 대해 활발하게 연구가 진행되고 있다.

그러나 이러한 방법론의 단점은 기존 모델에 대한 해밀토니안을 이해하고 있어야할 뿐 아니라, Non-conservative한 해밀토니안의 경우에는 계산이 복잡하고 추측하기 어렵기 때문에 현실 세계에서 가장 흔한 Constraints인 마찰에 대해서도 쉽게 적용하기 힘들다는 단점이 존재한다.

딥러닝에 해밀토니안과 라그랑지언을 이용하여 연구하는 방법 외에 주목할만한 방법은 AutoEncoder를 활용하여 물리학적인 모델을 역추적하는 방식이 있다. 워싱턴 대학의 Joseph Bakarji는 Discovering Governing Equations from Partitial Measurements with Deep Delay Autuencoders(arXiv:2201.05136)에서  딥러닝 모델 중 Autoencoder를 활용하여 관측된 데이터를 통해 데이터에서 모델을 찾아낼 수 있는 방법론을 소개한다.

그의 방법론은 2018년 발표된 Raissi의 Physics-Informed Neural Networks: A deep learning framework for solving forward and inverse problems involving nonlinear partitial differential equations를 바탕으로 한다. Raissi는 물리학적인 방정식을 이용하여 오차를 줄이는 방식으로 딥러닝 모델의 학습을 진행하여 물리학적 현상을 예측한다.

이러한 Raissi의 방법론에서 발전하여 Bakarji는 Takens’ Theorm을 활용하여 Lorentz Attraction같은 카오스 현상을 Raissi에서 정의한 비슷한 오차를 줄이는 방식으로 학습을 진행하며 카오스 이론을 재구성할 수 있다고 주장하고 있다. 즉, 저자의 주장이 맞다면 이 방법론으로 x가 지나온 경로의 좌표를 재구성하여 y와 z가 지나온 경로를 재구성하여 예측할 수 있다는 것이고 이를 활용한 모델이 효과적임을 주장하고 있다.
