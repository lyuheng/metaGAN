# metaGAN
implemetation of metaGAN on mini-Imagenet

### difference with paper ###
* We subsitute encoder with resnet18 to extract feature embeddings
* loss function
* wasserstein GAN-GP

### result on mini-Imagenet ###

|model         | 5-way Acc|        | 20-way Acc|        | 
|:-----:       | :-------:| :--:   |:---------:|:---:   |
|              | 1-shot      | 5-shot    | 1-shot       | 5-shot |
|MAML (paper)  | 48.7%      | 63.11%   | 16.49%      | 19.29% |
|MAML (ours)   | 45.56%     | -        |  -          | -      | 
|metaGAN + MAML| 48.87%     | -        |  -          |  -     |
| RN (paper)          |  50.44%    | 65.32%   |  -          |  -     |
| RN (ours)    |     -       |      -    |     -        |     -   |
|metaGAN + RN  | -           |     -     |    -         |         |
|meta SN-GAN   |   -         |  -        | -            | -       | 


### reference ###
[https://github.com/johnperuzzi/MetaGAN](https://github.com/johnperuzzi/MetaGAN)
