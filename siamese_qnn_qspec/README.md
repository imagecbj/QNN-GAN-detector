# 基于四元数的强泛化性 GAN 生成人脸检测算法
论文相关代码

# Paper Abstract
基于生成式对抗网络(generative adversarial network, GAN)模型生成的逼真人脸图像给司法、刑侦、名誉保
护等带来了挑战. 因此, 基于四元数提出一种具有强泛化性的 GAN生成人脸检测算法, 其由 GAN噪声指纹提取模块
与分类模块组成. GAN 噪声指纹提取模块采用孪生四元数 U-Net 提取噪声指纹特征; 分类模块基于提取的噪声指纹
特征采用四元数 ResNet 区分真实人脸和生成人脸; 使用基于距离的逻辑回归损失函数和交叉熵损失函数对参数进行
寻优. 采用公开的自然人脸数据集 CelebA 进行实验, 基于其利用多种 GAN 模型得到不同生成人脸数据集. 4 组消融
实验验证了该算法在 4 个方面的改进的有效性. 一种 GAN 生成人脸数据训练多种 GAN 测试的结果以及鲁棒性实验
结果表明, 所提算法比对比算法具有更强的泛化性以及较好的抵抗 JPEG 攻击的鲁棒性. 

# 代码简介
网络关键部分代码实现包含在该repo的文件中。实例化相应的类即可获得实例。

extractor: QNN siamese U-Net (fingerprint extractor)

ResNet: QNN ResNet

loss: siamese loss

mydata: an example of dataloader
