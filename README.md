# IPA-Segmentation
图像分割

图像分割是计算机视觉研究中的一个经典难题，已经成为图像理解领域关注的一个热点，图像分割是图像分析的第一步，是计算机视觉的基础，是图像理解的重要组成部分，同时也是图像处理中最困难的问题之一。所谓图像分割是指根据灰度、彩色、空间纹理、几何形状等特征把图像划分成若干个互不相交的区域，使得这些特征在同一区域内表现出一致性或相似性，而在不同区域间表现出明显的不同。简单的说就是在一副图像中，把目标从背景中分离出来。对于灰度图像来说，区域内部的像素一般具有灰度相似性，而在区域的边界上一般具有灰度不连续性。 关于图像分割技术，由于问题本身的重要性和困难性，从20世纪70年代起图像分割问题就吸引了很多研究人员为之付出了巨大的努力。虽然到目前为止，还不存在一个通用的完美的图像分割的方法，但是对于图像分割的一般性规律则基本上已经达成的共识，已经产生了相当多的研究成果和方法。
迄今为止我们已经在深度学习的路上越走越远，但必须要理解的是，Segmentation在CV行业是一个非常有历史的问题，随着近几年深度学习的飞速进化，该问题的解答才出现了一个全新的格局。
Segmentation能够自下而上分为三个等级的任务，导论可以参考：
https://zhuanlan.zhihu.com/p/50996404
https://www.jiqizhixin.com/graph/technologies/0871915d-52eb-4ada-8bb8-6c9267f3816c
https://mp.weixin.qq.com/s?__biz=MzIxOTczOTM4NA==&mid=2247487852&idx=1&sn=01245f0ddb67888243bb86e63e88c83f&chksm=97d7f4fba0a07dedf994762eaa3ae7a886211a1f2b9ba2c5f3d7dafd40b372e1120538496da1&token=748150220&lang=zh_CN#rd
任务1
第一环节我们会接触图像分割领域启发性的算法FCN。
FCN
https://arxiv.org/abs/1411.4038
https://zhuanlan.zhihu.com/p/80715481
https://zhuanlan.zhihu.com/p/30195134
https://github.com/MarvinTeichmann/tensorflow-fcn
在tf上用fcn算法对coco2017训练出一个常规的多分类网络，并阐述你对它的理解
并且选读U-net：https://zhuanlan.zhihu.com/p/44958351
任务2
我们将在本环节接触之前学习过的Faster RCNN的Segmentation变体，即Mask RCNN
Mask RCNN
https://arxiv.org/pdf/1703.06870.pdf
https://blog.csdn.net/jiongnima/article/details/79094159
https://blog.csdn.net/magic_ll/article/details/104606067
https://zhuanlan.zhihu.com/p/161379603
https://github.com/matterport/Mask_RCNN
我们将尝试使用Mask RCNN去完成一个比较有趣的自动驾驶环境感知测试。
AI4MARS来自Nasa Open Data，该数据集是为训练和验证火星的地形分类模型而构建的，这可能对未来的自动驾驶工作有用。 它包含了来自 Curiosity、Opportunity 和 Spirit rovers上采集的35K张图片以及基于此的326K语义分割完整图像标签，这些图像是通过众包收集的。 每张图片由 10 个人标记，以确保众包标签的质量和一致性更高。 它还包括约 1.5K 验证标签，这些验证标签由 NASA 的 MSL（火星科学实验室）任务（运行好奇号漫游车）和 MER（火星探索漫游车）任务（运行勇气号和机遇号漫游车）的漫游者计划者和科学家进行注释。
https://data.nasa.gov/Space-Science/AI4MARS-A-Dataset-for-Terrain-Aware-Autonomous-Dri/cykx-2qix
通过该数据集完成语义分割任务，并展示其效果。
