# Thesis
Thesis와 관련된 코드이다. GAN의 기본적인 사용법을 소개하고 이를 이용해서 stochastic process를 학습하는 방법과, stochastic partial differential equation (SDPE)을 푸는 방법을 소개한다. 튜토리얼을 위한 코드이기도 하다.

> ###### 주의사항: 2D_EllipticSPDE 코드는 따로 손을 보지 않아서 다른 코드에 비해 가독성이 떨어진다. 튜토리얼을 위해 만든 것이 아니고, 학습에 필요한 memory와 time cost가 (특히 FC의 경우) 굉장히 크기 때문에 돌리지 않는 것을 추천한다.

##### 논문
- GAN의 기본은 tutorial paper를 참조 https://arxiv.org/abs/1701.00160
- WGAN을 알고 싶으면 해당 paper 참조 https://arxiv.org/abs/1701.07875
  - WGAN만을 사용하면 성능이 좋지 않기 때문에, gradient penalty (https://arxiv.org/abs/1704.00028 )를 사용하거나 spectral normalization (https://arxiv.org/abs/1802.05957 )을 사용해야한다.
- WGANGP(gradient penalty)를 써서 SPDE를 푸는 문제가 알고 싶다면 https://arxiv.org/abs/1811.02033 참조
- WGANSN(spectral normalization)을 써서 SPDE를 푸는 문제가 알고 싶다면 https://ieeexplore.ieee.org/document/9989352/ 참조
- Thesis를 봐도 위의 내용은 잘 정리되어 있으나, access가 제한되어있을 수 있다.

##### 코드
- GAN으로 기본적인 2차원 data를 학습하는 방법을 알고 싶으면 mode_collap_2DRV/2DRV_GAN.ipynb 파일 참조
- GAN으로 stochastic process를 푸는 방법을 알고 싶으면 GaussianProcess0.2/GAN_FCN.ipynb, GaussianProcess0.2/WGANSN_FCN.ipynb 파일 참조
- GAN으로 SPDE를 푸는 방법을 알고 싶으면 Fully Correlated SODE/ODE_SD.ipynb 파일 참조
- Timechk_FCPC는 PCN이 FCN에 비해 얼마나 시간을 절약할 수 있는지 확인하는 코드이며 튜토리얼과 무관하다. EllipticSPDE는 시간이 오래 걸리므로 학습은 하지 않는 것을 추천한다.
