# Regularization
Regularization의 흐름 정리를 목표로 함

Shake-Shake regularization & Cutout

early stopping, Drop out, Batch normalization이 이전까지 많이 사용되던 방법이다.
#

multi-vranch network 가 최근 소개가 되었다. 
it was possible to randomly drop some of the information paths during training

Xavier Gastaldi 저자는 이 방법을 발전시켰다. 
 replacing the standard summation of parallel branches with a stochastic afﬁne combination.

평행의 3개의 branch들의 평균을 확률 적으로 결합하여, generalization 하는 것이 목표.

#

1.1 동기 Data augmentation techniques는 가장 편하게 사용 되는 방법이지만, input image와 intermediate representation 사이에 
차이가 크지 않다. 이를 점을 Shake-Shake regularization은 사용한다.



## Cutout [Improved Regularization of Convolutional Neural Networks with Cutout]
input image의 사각형으로 랜덤하게 마킹 후 학습한다. 

Shake-Shake와 

