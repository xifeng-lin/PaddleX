# PaddleX

飞桨全流程开发客户端，集飞桨核心框架、模型库、工具及组件等深度学习开发全流程所需能力于一身，不仅为您提供一键安装的客户端，开源开放的技术内核更方便您根据实际生产需求进行直接调用或二次开发，是提升深度学习项目开发效率的最佳辅助工具。

PaddleX由PaddleX Client可视化前端和PaddleX Core后端技术内核两个部分组成。

PaddleX Client是提升项目开发效率的核心模块，开发者可快速完成深度学习模型全流程开发。而开源开放的后端技术内核PaddleX Core， 为开发者提供统一的任务API，在集成飞桨模型库、工具组件的基础上，提供更高层、简洁的开发方式。开发者可以根据实际业务需求，选择使用可视化前端，或直接调用PaddleX Core后端技术内核完成任务开发。

 PaddleX不仅打通了深度学习开发的全流程、提供可视化开发界面， 还保证了开发者可以直接灵活地使用底层技术模块。

 我们诚挚地邀请您前往 [官网](https://www.paddlepaddle.org.cn/paddlex)下载试用PaddleX可视化前端，并获得您宝贵的意见或开源项目贡献。



## 目录

* <a href="#1">**产品特性**</a>
* <a href="#2">**PaddleX Client可视化前端**</a>
* <a href="#3">**PaddleX Core后端技术内核**</a>
* <a href="#4">**FAQ**</a>



## <a name="1">产品特性</a>

\-  **全流程打通**

将深度学习开发全流程打通，并提供可视化开发界面， 省去了对各环节API的熟悉过程及重复的代码开发，极大地提升了开发效率。

\-    **开源技术内核**

集飞桨产业级CV工具集、迁移学习工具PaddleHub、可视化工具VisualDL、模型压缩工具PaddleSlim等于一身，并提供统一的任务API，可脱离前端单独下载使用，方便被集成与改造，为您的业务实践全程助力。

\-    **本地一键安装**

无需额外下载依赖或驱动，提供适配Windows、Mac、Linux系统一键安装的客户端，技术内核可单独通过pip install安装。本地开发、保证数据安全，高度符合产业应用的实际需求。

\-    **教程与服务**

从数据集准备到上线部署，为您提供业务开发全流程的文档说明及技术服务。开发者可以通过QQ群、微信群、GitHub社区等多种形式与飞桨团队及同业合作伙伴交流沟通。



## <a name="2">PaddleX Client可视化前端</a>

**第一步：下载客户端**

您需要前往 [官网](https://www.paddlepaddle.org.cn/paddlex)填写基本信息后下载试用PaddleX可视化前端



**第二步：准备数据**

在开始模型训练前，您需要根据不同的任务类型，将数据标注为相应的格式。目前PaddleX支持【图像分类】、【目标检测】、【语义分割】、【实例分割】四种任务类型。不同类型任务的数据处理方式可查看[数据标注方式]([https://github.com/jiangjiajun/PaddleSolution/tree/master/Docs/3_%E6%A0%87%E6%B3%A8%E8%87%AA%E5%B7%B1%E7%9A%84%E8%AE%AD%E7%BB%83%E6%95%B0%E6%8D%AE](https://github.com/jiangjiajun/PaddleSolution/tree/master/Docs/3_标注自己的训练数据))。



**第三步：导入我的数据集**

数据标注完成后，需要根据不同的任务，将数据和标注文件，按照客户端提示更名并保存到正确的文件中。

![image-20200326214525816](/Users/lvxueying/Library/Application Support/typora-user-images/image-20200326214525816.png)

在客户端新建数据集后，选择与数据集匹配的任务类型，并选择数据集对应的路径，将数据集导入：

![数据集导入步骤](D:/百度/官网/官网文档编写/README.assets/导入数据集步骤-1584938863545.jpg)

导入完成后，客户端会自动校验数据及标注文件是否合规，校验成功后，您可根据实际需求，将数据集按比例划分为训练集、验证集、测试集。

![划分数据集](D:/百度/官网/官网文档编写/README.assets/划分数据集.jpg)

您可在「数据分析」模块按规则预览您标注的数据集，双击单张图片可放大查看。



**第四步：创建项目**

在完成数据导入后，您可开始新建项目开始一个模型训练。

![创建项目步骤](D:/百度/官网/官网文档编写/README.assets/创建项目步骤.jpg)

项目创建完成，选择选择已载入客户端并校验后的数据集，并点击下一步，进入参数配置页面。

![数据选择](D:/百度/官网/官网文档编写/README.assets/数据选择-1584953277024.jpg)



**第四步：参数配置**

参数配置主要分为三部分：模型参数、训练参数、优化策略。您可根据实际需求选择模型结构、骨架网络及对应的训练参数、优化策略，使得任务效果最佳。

![参数配置1](D:/百度/官网/官网文档编写/README.assets/参数配置1.jpg)

![参数配置2](D:/百度/官网/官网文档编写/README.assets/参数配置2.jpg)

参数配置完成后，点击启动训练，模型开始训练并进行效果评估。



**第五步：训练可视化**

在训练过程中，您可通过VisualDL查看模型训练过程参数变化、日志详情，及当前最优的训练集和验证集训练指标。模型在训练过程中通过点击"终止训练"随时终止训练过程。

![image-20200326223158476](/Users/lvxueying/Desktop/PaddlePaddle/00-PaddleX/05-产品文档、PPT/README.assets/训练可视化.png)

![训练可视化](D:/百度/官网/官网文档编写/README.assets/训练可视化.jpg)

模型训练结束后，点击”下一步“，进入模型评估页面。



**第六步：模型评估**

在模型评估页面，可查看模型在验证集上的效果，包括混淆矩阵、精度、召回率等。

![模型评估](D:/百度/官网/官网文档编写/README.assets/模型评估.jpg)

评估指标定义如下：

| 评估指标 | 定义                                                         |
| -------- | :----------------------------------------------------------- |
| 混淆矩阵 | 模型评估的一种基本方法，矩阵大小为N*N（N为类别数）。矩阵中的每个元素表示，类A识别为类B的样本数目。 |
| 交并比   | 两个集合的交集与并集的比值。                                 |
| 精准率   | TP/（TP+FP），其中TP（True Positive）是把正类预测为正类的样本数，FP（False Positive）是将负类预测为正类的样本数。 |
| 召回率   | TP/（TP+FN），其中FN（False Negative）是将正类预测为负类的样本数。 |

点击”下一步“，进入模型发布页面



**第七步：模型发布**

您可根据实际的生产环境需求，选择将模型发布为需要的版本。

![模型发布](D:/百度/官网/官网文档编写/README.assets/模型发布-1584958908870.jpg)



## <a name="3">PaddleX Core后端技术内核</a>





## <a name="4">FAQ</a>







