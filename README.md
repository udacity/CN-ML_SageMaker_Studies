# 使用 AWS SageMaker 部署机器学习模型的案例研究

此代码库包含使用 AWS SageMaker 部署机器学习模型的代码和相关文件。其中包含各种案例研究、代码练习和项目文件的多个教程 notebook，展示了机器学习工作流程的各个环节，并使你有机会练习部署各种机器学习算法。

### 教程

* [人口分割](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Population_Segmentation)：学习如何在 SageMaker 中构建和部署非监督式模型。在此示例中，你需要聚类美国人口普查数据：使用 PCA 降低数据的维度，并通过 k 均值对生成的主成分进行聚类。
* [支付欺诈检测](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Payment_Fraud_Detection)：学习如何在 SageMaker 中构建和部署监督式 LinearLearner 模型。你需要优化模型并处理类别不平衡性问题，然后训练模型检测信用卡欺诈行为。
* [部署自定义 PyTorch 模型 (Moon Data)](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Moon_Data)：训练和部署一个分类“月亮”数据的自定义 PyTorch 神经网络，“月亮”数据是形状像月亮一样的二维数据集。
* [时间序列预测](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Time_Series_Forecasting)：学习分析时间序列数据，并调整数据格式，使其能够用于训练 [DeepAR](https://docs.aws.amazon.com/sagemaker/latest/dg/deepar.html) 算法，这是一种利用循环神经网络的预测算法。你需要训练一个模型来预测家庭能耗模式并评估结果。

### 实战项目

[剽窃检测器](https://github.com/udacity/ML_SageMaker_Studies/tree/master/Project_Plagiarism_Detection)：构建一个端到端剽窃分类模型。运用所学的技能清理数据、提取有意义的特征，并在 SageMaker 中部署剽窃分类器。

![Examples of dimensionality reduction and time series prediction](./Time_Series_Forecasting/notebook_ims/example_applications.png)

---

## 设置说明

此代码库中提供的 notebook 需要使用 Amazon SageMaker 平台执行。下面简要说明了如何使用 SageMaker 设置托管 notebook 实例，你可以在此实例中完成和运行 notebook。

### 登录 AWS 控制台并创建一个 notebook 实例

登录 [AWS 控制台](https://console.aws.amazon.com)并转到 SageMaker 信息中心。点击“Create notebook instance”。
* notebook 可以随意命名，建议使用 ml.t2.medium，因为它属于免费套餐。
* 对于角色，新建一个角色就行了。使用默认选项即可。
* 注意，notebook 实例需要能够访问 S3 资源，默认就能访问。该 notebook 可以访问名称中带 sagemaker 的任何 S3 存储桶或对象。
* 使用 **git clone** 将项目代码库克隆到 notebook 实例中，网址为：`https://github.com/udacity/ML_SageMaker_Studies.git`

### 打开和运行你所选的 notebook

将代码库克隆到 notebook 实例中后，你可以转到要完成或执行的任何 notebook，然后完成该 notebook。每个 notebook 都包含了额外的说明。
