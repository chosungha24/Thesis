# Thesis
나의 thesis와 관련된 코드이다. GAN의 기본적인 사용법을 소개하고 이를 이용해서 stochastic process를 학습하는 방법과, stochastic partial differential equation (SDPE)을 푸는 방법을 소개한다. 이 과정에서 많이 사용하는 fully connected network (FCN) 모델 외에, SPDE에서 사용하기 좋은 polynomial chaos network (PCN)를 구현하는 방법 역시 포함한다.

> ###### 주의사항: 2D_EllipticSPDE 코드는 따로 손을 보지 않아서 다른 코드에 비해 확인하기 어렵다. 또한 학습에 필요한 memory와 time cost가 (특히 FC의 경우) 굉장히 크기 때문에 함부로 돌리지 않는 것을 추천한다.

- GAN으로 기본적인 2차원 data를 학습하는 방법을 알고 싶으면 mode_collap_2DRV 폴더로
- GAN으로 stochastic process를 푸는 방법을 알고 싶으면 GaussianProcess0.2 폴더로
- GAN으로 SPDE를 푸는 방법을 알고 싶으면 1D_EllipticSPDE 폴더로
- 다른 폴더에는 튜토리얼을 추가하지 않을 예정이다.
