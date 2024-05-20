# 前言

随着深度学习在现代工业中迅速被广泛采用，组织机构正在寻找将流行的大数据工具与高效的深度学习库结合起来的方法。这将有助于深度学习模型以更高的效率和速度进行训练。

借助*Apache Spark 深度学习食谱*，您将通过具体的配方来生成深度学习算法的结果，而不会陷入理论中。从为深度学习设置 Apache Spark 到实现各种类型的神经网络，本书解决了常见和不太常见的问题，以便在分布式环境中进行深度学习。除此之外，您还将获得在 Spark 中可以重复使用以解决类似问题或微调以解决稍有不同问题的深度学习代码。您还将学习如何使用 Spark 进行数据流处理和聚类。一旦掌握了基础知识，您将探索如何使用流行的库（如 TensorFlow 和 Keras）在 Spark 中实现和部署 CNN、RNN 和 LSTM 等深度学习模型。最终，这是一本旨在教授如何在 Spark 上实际应用模型的食谱，因此我们不会深入探讨理论和数学。

在本章中使用的模型背后的原理，尽管我们会引用额外的

可以获取每个模型的信息。

通过本书，您将掌握在 Apache Spark 上训练和部署高效深度学习模型的专业知识。

# 本书适合对象

本书适用于具有基本机器学习和大数据概念的人，希望通过自顶向下的方法扩展他们的理解。本书以即插即用的方式提供了深度学习和机器学习算法。任何没有编程经验的人，特别是对 Python 不熟悉的人，都可以按照逐步指示轻松实现本书中的算法。本书中大部分代码都是不言自明的。每个代码块执行一个特定的功能，或者在挖掘、操作、转换和拟合数据到深度学习模型方面执行一个动作。

本书旨在通过有趣的项目（如股价预测）为读者提供实践经验，同时更加扎实地理解深度学习和机器学习概念。这是通过书中每一章节提供的大量在线资源链接（如发表的论文、教程和指南）来实现的。

# 本书涵盖内容

第一章，*为深度学习设置 Spark*，涵盖了您需要的一切，以便在虚拟 Ubuntu 桌面环境中开始使用 Spark 进行开发。

第二章，*使用 Spark 创建神经网络*，解释了在不使用 TensorFlow 或 Keras 等深度学习库的情况下，从头开始开发神经网络的过程。

第三章，*卷积神经网络的痛点*，介绍了在图像识别的卷积神经网络上工作时出现的一些痛点，以及如何克服这些问题。

第四章，*循环神经网络的痛点*，介绍了前馈神经网络和循环神经网络，并描述了循环神经网络出现的一些痛点，以及如何利用 LSTM 来解决这些问题。

第五章，*使用 Spark ML 预测消防部门呼叫*，介绍了使用 Spark 机器学习为旧金山市的消防部门呼叫开发分类模型的过程。

第六章，*在生成网络中使用 LSTMs*，提供了使用小说或大型文本语料库作为输入数据来定义和训练 LSTM 模型的实际方法，同时还使用训练好的模型生成自己的输出序列。

第七章，*使用 TF-IDF 进行自然语言处理*，介绍了对聊天机器人对话数据进行升级分类的步骤。

第八章，*使用 XGBoost 进行房地产价值预测*，专注于使用 Kings County 房屋销售数据集训练一个简单的线性模型，并用它来预测房价，然后深入研究一个稍微复杂的模型来提高预测准确性。

第九章，*使用 LSTM 预测苹果股票市场成本*，专注于使用 Keras 上的 LSTM 创建深度学习模型，以预测 AAPL 股票的股市价格。

第十章，*使用深度卷积网络进行人脸识别*，利用 MIT-CBCL 数据集中 10 个不同主题的面部图像来训练和测试深度卷积神经网络模型。

第十一章，*使用 Word2Vec 创建和可视化词向量*，专注于机器学习中向量的重要性，并指导用户如何利用 Google 的 Word2Vec 模型训练不同的模型并可视化从小说中生成的词向量。

第十二章，*使用 Keras 创建电影推荐引擎*，专注于使用深度学习库 Keras 为用户构建电影推荐引擎。

第十三章，*在 Spark 上使用 TensorFlow 进行图像分类*，专注于利用迁移学习识别世界上两位顶级足球运动员：克里斯蒂亚诺·罗纳尔多和利昂内尔·梅西。

# 为了充分利用本书

1.  利用提供的所有链接，更好地理解本书中使用的一些术语。

1.  互联网是当今世界上最大的大学。使用 YouTube、Udemy、edX、Lynda 和 Coursera 等网站的视频，了解各种深度学习和机器学习概念。

1.  不要只是读这本书然后忘记它。在阅读本书时，实际实施每一步。建议您在阅读每个配方时打开您的 Jupyter Notebook，这样您可以在阅读书籍的同时处理每个配方，并同时检查您获得的每个步骤的输出。

# 下载示例代码文件

您可以从[www.packtpub.com](http://www.packtpub.com)的帐户中下载本书的示例代码文件。如果您在其他地方购买了这本书，可以访问[www.packtpub.com/support](http://www.packtpub.com/support)并注册，以便将文件直接发送到您的邮箱。

您可以按照以下步骤下载代码文件：

1.  登录或注册[www.packtpub.com](http://www.packtpub.com/support)。

1.  选择“支持”选项卡。

1.  单击“代码下载和勘误”。

1.  在搜索框中输入书名，然后按照屏幕上的说明操作。

下载文件后，请确保使用最新版本的解压缩软件解压缩文件夹：

+   WinRAR/7-Zip 适用于 Windows

+   Zipeg/iZip/UnRarX 适用于 Mac

+   7-Zip/PeaZip 适用于 Linux

该书的代码包也托管在 GitHub 上，网址为[`github.com/PacktPublishing/Apache-Spark-Deep-Learning-Cookbook`](https://github.com/PacktPublishing/Apache-Spark-Deep-Learning-Cookbook)。如果代码有更新，将在现有的 GitHub 存储库上进行更新。

我们还有来自我们丰富的图书和视频目录的其他代码包，可在 **[`github.com/PacktPublishing/`](https://github.com/PacktPublishing/)** 上找到。去看看吧！

# 使用的约定

本书中使用了许多文本约定。

`CodeInText`：表示文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄。这是一个例子："保存在工作目录内的 `trained` 文件夹下。"

代码块设置如下：

```scala
print('Total Rows')
df.count()
print('Rows without Null values')
df.dropna().count()
print('Row with Null Values')
df.count()-df.dropna().count()
```

任何命令行输入或输出都以以下方式编写：

```scala
nltk.download("punkt")
nltk.download("stopwords")
```

**粗体**：表示一个新术语、一个重要词或屏幕上看到的词。例如，菜单或对话框中的单词会出现在文本中。这是一个例子："右键单击页面，然后单击“另存为”…"

警告或重要说明会出现在这样。

提示和技巧会出现在这样。

# 部分

在本书中，您会经常看到几个标题（*准备工作*、*如何做*、*它是如何工作的*、*还有更多*和*另请参阅*）。

清晰地说明如何完成食谱，使用以下部分：

# 准备工作

本节告诉您在食谱中可以期望什么，并描述如何设置食谱所需的任何软件或任何初步设置。

# 如何做…

本节包含遵循食谱所需的步骤。

# 它是如何工作的…

本节通常包括对前一节中发生的事情的详细解释。

# 还有更多…

本节包含有关食谱的其他信息，以使您对食谱更加了解。

# 另请参阅

本节提供了指向食谱的其他有用信息的链接。