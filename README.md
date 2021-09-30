# CinCGAN-SE
Joint magnitude estimation and phase recovery using Cyle-in-cycle GAN for non-parallel speech enhancement

This is the repo of the manuscript "Joint magnitude estimation and phase recovery using Cyle-in-cycle GAN for non-parallel speech enhancement", which is to be submitted to ICASSP2022. Some audio samples are provided here and the code will be released soon.

Abstract: For the lack of adequate paired noisy-clean speech corpus in many real scenarios, non-parallel training is a promising task for DNN-based speech enhancement methods. However, because of the severe mismatch between input and target speech, many previous studies only focus on magnitude spectrum estimation and remain the phase unaltered, resulting in the degraded speech quality under low signal-to-noise ratio conditions. To tackle this problem, we decouple the difficult target w.r.t. original spectrum optimization into spectral magnitude and phase, and a novel Cycle-in-cycle generative adversarial network (dubbed CinCGAN) is proposed to jointly estimate the spectral magnitude and phase information stage by stage. In the first stage, we pretrain a magnitude CycleGAN to coarsely denoise the spectral magnitude spectrum. In the second stage, we couple the pretrained CycleGAN with a complex-valued CycleGAN as a cycle-in-cycle structure to recover phase information and refine the spectral magnitude simultaneously. Experimental results on Voice Bank + DEMAND show that the proposed approach significantly outperforms previous baselines under non-parallel training. The evaluation on training the models with standard paired data also shows that the proposed method can achieve remarkable performance.

System flowchart of CinCGAN

![image](https://user-images.githubusercontent.com/51236251/135372928-9d6b1480-d357-4ec1-83f6-625791d71c6c.png)

The architecture of generators:


Results:
![image](https://user-images.githubusercontent.com/51236251/135373001-cd62343b-e44e-40e1-8c3a-0e9a85250464.png)

![image](https://user-images.githubusercontent.com/51236251/135373047-7cbc19e1-deba-4cb8-8d47-bee76d86b8a2.png)

Samples under non-parallel training:

![image](https://user-images.githubusercontent.com/51236251/135373159-d5e57d3f-737d-4522-8662-8f284e720f48.png)

