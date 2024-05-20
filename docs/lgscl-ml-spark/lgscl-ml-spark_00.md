# 前言

机器学习的核心是关注将原始数据转化为可操作智能的算法。这一事实使得机器学习非常适合于大数据的预测分析。因此，如果没有机器学习，要跟上这些大规模信息流几乎是不可能的。相对较新且新兴的技术 Spark 为大数据工程师和数据科学家提供了一个强大的响应和统一的引擎，既更快速又易于使用。

这使得来自多个领域的学习者能够以更大规模地交互解决他们的机器学习问题。本书旨在使数据科学家、工程师和研究人员能够开发和部署规模化的机器学习应用程序，以便他们学会如何在数据密集型环境中处理大数据集群，构建强大的机器学习模型。

本书的内容是从 Spark 和 ML 基础开始以自下而上的方式编写的，探索了特征工程中的数据，构建可扩展的 ML 管道，通过调整和适应新的数据和问题类型，最终进行模型构建和部署。为了更清晰，我们以这样一种方式提供了章节大纲，以便具有最基本的机器学习和 Spark 编程知识的新读者能够跟随示例，并朝着一些真实的机器学习问题及其解决方案迈进。

# 本书内容包括以下内容

第一章，*使用 Spark 进行数据分析简介*，本章介绍了 Spark 的概述、计算范式、安装，并帮助我们开始使用 Spark。它将简要描述 Spark 的主要组件，并专注于其具有弹性分布式数据集（RDD）和数据集的新计算进展。然后，它将专注于 Spark 的机器学习库生态系统。在扩展到 Amazon EC2 之前，将演示使用 Spark 和 Maven 安装、配置和打包简单的机器学习应用程序。

第二章，*机器学习最佳实践*，提供了对统计机器学习（ML）技术的概念介绍，旨在带领新手从对机器学习的最基本知识到成为熟练的从业者。本章的第二部分侧重于为根据应用类型和要求选择合适的机器学习算法提供一些建议。然后，它将介绍应用大规模机器学习管道时的一些最佳实践。

第三章，*通过了解数据来理解问题*，详细介绍了用于处理结构化数据的数据集和弹性分布式数据集（RDD）API，旨在提供对可用数据进行基本理解的机器学习问题。最后，您将能够轻松处理基本和复杂的数据操作。将提供使用 RDD 和基于数据集的数据操作的基本抽象的一些比较，以展示在编程和性能方面的收益。此外，我们将指导您走上正确的道路，以便您能够使用 Spark 将 RDD 或数据对象持久化在内存中，从而在后期的并行操作中有效地重复使用。

《第四章》《通过特征工程提取知识》解释了了解应该用于创建预测模型的特征不仅至关重要，而且可能是一个需要深入了解问题领域的难题。可以自动选择数据中对某人正在处理的问题最有用或最相关的特征。考虑到这些问题，本章详细介绍了特征工程，解释了应用它的原因以及特征工程中的一些最佳实践。

除此之外，还将讨论应用于大规模机器学习技术的特征提取、转换和选择的理论描述和示例，使用 Spark MLlib 和 Spark ML API。

《第五章》《通过示例进行监督和无监督学习》将提供围绕如何快速而有力地将监督和无监督技术应用于可用数据解决新问题的实际知识，这些知识是基于前几章的一些广泛使用的示例。这些示例将从 Spark 的角度进行演示。

《第六章》《构建可扩展的机器学习管道》解释了机器学习的最终目标是使机器能够在不需要繁琐和耗时的人工参与和交互的情况下自动从数据中构建模型。因此，本章将指导读者通过使用 Spark MLlib 和 Spark ML 创建一些实用和广泛使用的机器学习管道和应用。将详细描述这两个 API，并且还将涵盖基线用例。然后，我们将专注于扩展 ML 应用程序，使其能够应对不断增加的数据负载。

《第七章》《调整机器学习模型》表明，调整算法或机器学习应用可以简单地被视为一个过程，通过这个过程优化影响模型的参数，以使算法表现最佳。本章旨在指导读者进行模型调整。它将涵盖用于优化 ML 算法性能的主要技术。技术将从 MLlib 和 Spark ML 的角度进行解释。我们还将展示如何通过调整多个参数（如超参数、MLlib 和 Spark ML 的网格搜索参数、假设检验、随机搜索参数调整和交叉验证）来改善 ML 模型的性能。

《第八章》《调整您的机器学习模型》涵盖了使算法适应新数据和问题类型的高级机器学习技术。它将主要关注批处理/流处理架构和使用 Spark 流处理的在线学习算法。最终目标是为静态机器学习模型带来动态性。读者还将看到机器学习算法如何逐渐从数据中学习，即每次算法看到新的训练实例时，模型都会更新。

第九章《使用流式和图形数据进行高级机器学习》解释了如何利用 Spark MLlib 和 Spark ML 等工具在流式和图形数据上应用机器学习技术，例如在主题建模中。读者将能够利用现有的 API 从流数据源（如 Twitter）构建实时和预测性应用程序。通过 Twitter 数据分析，我们将展示如何进行大规模社交情感分析。我们还将展示如何使用 Spark MLlib 开发大规模电影推荐系统，这是社交网络分析的一个隐含部分。

第十章《配置和使用外部库》指导读者如何使用外部库来扩展他们的数据分析。将给出使用第三方包或库在 Spark 核心和 ML/MLlib 上进行机器学习应用的示例。我们还将讨论如何编译和使用外部库与 Spark 的核心库进行时间序列分析。如约定的，我们还将讨论如何配置 SparkR 以改进探索性数据操作。

# 本书所需内容

**软件要求：**

第 1-8 章和第十章需要以下软件：Spark 2.0.0（或更高版本）、Hadoop 2.7（或更高版本）、Java（JDK 和 JRE）1.7+/1.8+、Scala 2.11.x（或更高版本）、Python 2.6+/3.4+、R 3.1+和已安装的 RStudio 0.99.879（或更高版本）。可以使用 Eclipse Mars 或 Luna（最新版本）。此外，还需要 Maven Eclipse 插件（2.9 或更高版本）、用于 Eclipse 的 Maven 编译器插件（2.3.2 或更高版本）和用于 Eclipse 的 Maven 汇编插件（2.4.1 或更高版本）。最重要的是，重复使用 Packt 提供的`pom.xml`文件，并相应地更改先前提到的版本和 API，一切都会得到解决。

对于第九章《使用流式和图形数据进行高级机器学习》，几乎所有先前提到的所需软件都是必需的，除了 Twitter 数据收集示例，该示例将在 Spark 1.6.1 中展示。因此，需要 Spark 1.6.1 或 1.6.2，以及友好的 Maven `pom.xml`文件。

**操作系统要求：**

Spark 可以在多个操作系统上运行，包括 Windows、Mac OS 和 LINUX。然而，Linux 发行版更可取（包括 Debian、Ubuntu、Fedora、RHEL、CentOS 等）。更具体地说，例如对于 Ubuntu，建议使用 14.04/15.04（LTS）64 位完整安装或 VMWare player 12 或 Virtual Box。对于 Windows，建议使用 Windows（XP/7/8/10），对于 Mac OS X（10.4.7+）也是如此。

**硬件要求：**

为了顺利使用 Spark，建议使用至少核心 i3 或核心 i5 处理器的计算机。然而，为了获得最佳结果，核心 i7 将实现更快的数据处理和可伸缩性，至少需要 8GB RAM（建议）用于独立模式，至少需要 32GB RAM 用于单个 VM，或者用于集群的更高内存。此外，需要足够的存储空间来运行繁重的任务（取决于您将处理的数据大小），最好至少有 50GB 的免费磁盘存储空间（用于独立和 SQL 仓库）。

# 本书适合对象

由于 Python 和 R 是数据科学家常用的两种流行语言，因为有大量的模块或软件包可用来帮助他们解决数据分析问题。然而，这些工具的传统用法通常有限，因为它们在单台机器上处理数据，或者使用基于主存储器的方法处理数据，数据的移动变得耗时，分析需要抽样，并且从开发到生产环境的转换需要大量的重新设计。为了解决这些问题，Spark 提供了一个强大且统一的引擎，既快速又易于使用，这使您能够以交互方式解决机器学习问题，并且规模更大。

因此，如果您是学术界人士、研究人员、数据科学工程师，甚至是处理大型和复杂数据集的大数据工程师。此外，如果您想要加速数据处理管道和机器学习应用的扩展，这本书将是您旅程中的合适伴侣。此外，Spark 提供了许多语言选择，包括 Scala、Java 和 Python。这将帮助您将机器学习应用程序置于 Spark 之上，并使用这些编程语言之一进行重塑。

您应该至少熟悉机器学习概念的基础知识。了解开源工具和框架，如 Apache Spark 和基于 Hadoop 的 MapReduce，会很有帮助，但并非必需。我们期望您具备扎实的统计学和计算数学背景。此外，了解 Scala、Python 和 Java 是明智的。然而，如果您熟悉中级编程语言，这将有助于您理解本书中的讨论和示例。

# 约定

在这本书中，您会发现许多不同风格的文本，用以区分不同类型的信息。以下是一些这些风格的例子，以及它们的含义解释。

文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄显示如下: "我们可以通过使用 `include` 指令来包含其他上下文。"

在 Windows 环境中创建 Spark 会话的代码块设置如下:

```scala
[default]
SparkSession spark = SparkSession
                  .builder()
                  .appName("JavaFPGrowthExample")
                  .master("local[*]")
                  .config("spark.sql.warehouse.dir", "E:/Exp/")                  .getOrCreate();
```

或者从输入数据集创建简单的 RDD 设置如下:

```scala
[default]
            String filename = “input/dataset.txt”;
            RDD<String> data = spark.sparkContext().textFile(fileName, 1);
```

任何命令行输入或输出都以如下方式编写:

```scala
$ scp -i /usr/local/key/my-key-pair.pem  /usr/local/code/FPGrowth-0.0.1-SNAPSHOT-jar-with-dependencies.jar ec2-user@ec2-52-18-252-59.eu-west-1.compute.amazonaws.com:/home/ec2-user/

```

**新术语**和**重要单词**以粗体显示。您在屏幕上看到的单词、菜单或对话框中的单词等都会以这样的方式出现在文本中: "点击 **下一步** 按钮将您移动到下一个屏幕"。

### 注意

警告或重要说明会出现在这样的框中。

### 提示

提示和技巧会出现在这样。