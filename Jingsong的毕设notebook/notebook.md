# Reid 相关论文总结

### Parameter Sharing Exploration and Hetero-Center based Triplet Loss for Visible-Thermal Person Re-Identification
源码详见(https://github.com/hijune6/Hetero-center-triplet-loss-for-VT-Re-ID)
> RegDB mAP 83.28
> SYSU-MM01 mAP 57.51

研究ResNet50双流网络的参数共享对VI Reid的影响

对于part-level的people feature learning，提出一个损失函数hetero-center based triplet loss

*we propose the hetero-center based triplet loss to relax the strict constraint of traditional triplet loss through replacing the comparison of anchor to all the other samples by anchor center to all the other centers.*

