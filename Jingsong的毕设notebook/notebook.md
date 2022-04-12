# Reid 相关论文总结

### Parameter Sharing Exploration and Hetero-Center based Triplet Loss for Visible-Thermal Person Re-Identification
源码详见(https://github.com/hijune6/Hetero-center-triplet-loss-for-VT-Re-ID)
> RegDB mAP 83.28

> SYSU-MM01 mAP 57.51

研究ResNet50双流网络的参数共享对VI Reid的影响

对于part-level的people feature learning，提出一个损失函数hetero-center based triplet loss

*we propose the hetero-center based triplet loss to relax the strict constraint of traditional triplet loss through replacing the comparison of anchor to all the other samples by anchor center to all the other centers.*

### Channel Augmented Joint Learning for Visible-Infrared Recognition

> SYSU-MM01 All Search mAP 66.89 Indoor Search mAP 80.37

> RegDB *VtoI* mAP 79.14 *ItoV* mAP 77.82

### Deep Learning for Person Re-Identification
AGW baseline 
> SYSU-MM01 All Search mAP 47.65 Indoor Search mAP 62.97

### Bag of Tricks and a Strong Baseline for Deep Person Re-Identification
源码详见(https://github.com/michuanhaohao/reid-strong-baseline)
> Market1501 global feature mAP 85.9 rank-1 94.5

这是一篇关于VVReid的baseline和tricks的文章，我相信其中的思想会带来新的思路


### Discriminative Spatial Feature Learning for Person Re-Identification ACM2020 (Part-level Feature)

