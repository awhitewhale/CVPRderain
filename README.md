# CVPRderain
## 1.Towards Robust Rain Removal Against Adversarial Attacks: A Comprehensive Benchmark Analysis and Beyond

[[paper]](https://arxiv.org/abs/2203.16931)
[[code]](https://github.com/yuyi-sd/Robust_Rain_Removal)

除雨的目的是去除图像/视频中的雨痕，减少雨水造成的破坏性影响。它不仅能提高图像/视频的可见度，还能使许多计算机视觉算法正常运行。本文首次尝试对基于深度学习的除雨方法的鲁棒性进行全面研究，以对抗对抗性攻击。我们的研究表明，当图像/视频高度退化时，除雨方法更容易受到对抗性攻击，因为小的失真/扰动变得不那么明显或可检测。在本文中，我们首先从人类感知和机器分析任务的角度，对各种方法在不同级别的攻击和各种损失/目标产生的扰动进行了全面的经验评估。对现有方法中的关键模块进行了系统的评估，即它们对对抗性攻击的鲁棒性。根据我们的分析结果，我们通过整合这些有效的模块，构建了一个更稳健的减损方法。最后，我们研究了针对减损问题的各种类型的对抗性攻击及其对人类和机器视觉任务的影响，包括：1）雨区攻击，只在雨区添加扰动，使被攻击的雨图像中的扰动不那么明显；2）物体敏感攻击，只在给定物体附近区域添加扰动。

## 2.Unpaired Deep Image Deraining Using Dual Contrastive Learning

[[paper]](https://arxiv.org/abs/2109.02973)
[[code]]()

从一组未配对的干净和雨天的图像中学习单一图像衍生（SID）网络是实用和有价值的，因为获取配对的真实世界数据几乎是不可行的。然而，如果没有成对的数据作为监督，学习SID网络是具有挑战性的。此外，在SID任务中简单地使用现有的非配对学习方法（如非配对对抗学习和循环一致性约束）不足以学习从雨天输入到清洁输出的基本关系，因为雨天和清洁图像之间存在明显的领域差距。在本文中，我们开发了一个有效的非配对SID对抗框架，通过深度特征空间的双重对比学习方式探索非配对样本的相互属性，命名为DCDGAN。提出的方法主要由两个合作分支组成。双向翻译分支（BTB）和对比性指导分支（CGB）。具体来说，BTB充分利用对抗性一致性的循环结构来生成丰富的示例对，并通过配备双向映射来挖掘两个领域之间的潜在特征分布。同时，CGB通过鼓励相似的特征分布靠近，而将不相似的特征分布推远，隐含地约束了不同典范在深度特征空间中的嵌入，以更好地促进除雨和帮助图像修复。广泛的实验表明，我们的方法在合成和真实世界的数据集上与现有的非配对脱嵌方法相比表现良好，并产生了与几个完全监督或半监督的模型相当的结果。
