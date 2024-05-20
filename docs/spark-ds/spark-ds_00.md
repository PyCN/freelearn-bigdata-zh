# 前言

在这个智能时代，数据分析是维持和促进业务增长的关键。每家企业都在尝试尽可能利用他们的数据，借助各种数据科学工具和技术沿着分析成熟度曲线前进。数据科学需求的突然增加是数据科学家短缺的明显原因。很难满足市场需求，因为独角兽数据科学家是统计学、机器学习、数学建模以及编程方面的专家。

独角兽数据科学家的可用性只会随着市场需求的增加而减少，并将继续如此。因此，需要一个解决方案，不仅能够赋予独角兽数据科学家更多的权力，而且还能创造 Gartner 所称的“公民数据科学家”。公民数据科学家不是其他人，而是开发人员、分析师、BI 专业人员或其他主要工作职能不在统计或分析之外，但足够热衷于学习数据科学。他们正在成为组织和整个行业中民主化数据分析的关键推动者。

有越来越多的工具和技术旨在促进大规模的大数据分析。这本书试图创建能够利用 Apache Spark 分布式计算平台进行数据分析的公民数据科学家。

这本书是一个实用指南，教授统计分析和机器学习，以构建可扩展的数据产品。它有助于掌握数据科学的核心概念，以及 Apache Spark，帮助您在任何实际的数据分析项目上快速启动。整本书的每一章都有足够的例子支持，可以在家用电脑上执行，以便读者可以轻松地跟踪和吸收概念。每一章都试图是独立的，以便读者可以从任何章节开始，并指向相关章节以获取详细信息。虽然章节从基础知识开始，供初学者学习和理解，但同时也足够全面，供高级架构师使用。

# 本书内容

第一章, *大数据和数据科学-简介*，本章简要讨论了大数据分析中的各种挑战，以及 Apache Spark 如何在单一平台上解决这些问题。本章还解释了数据分析是如何演变成现在的样子，也对 Spark 堆栈有了基本的了解。

第二章, *Spark 编程模型*，本章讨论了 Apache Spark 的设计考虑和支持的编程语言。它还解释了 Spark 的核心组件，并详细介绍了 RDD API，这是 Spark 的基本构建模块。

第三章, *数据框简介*，本章介绍了数据框，这是数据科学家最方便和有用的组件，可以轻松工作。它解释了 Spark SQL 和 Catalyst 优化器如何赋予数据框权力。还演示了各种数据框操作的代码示例。

第四章, *统一数据访问*，本章讨论了我们从不同来源获取数据的各种方式，以统一的方式 consolide 和工作。它涵盖了实时数据收集和操作的流方面。它还讨论了这些 API 的底层基础知识。

第五章，Spark 上的数据分析，本章讨论了完整的数据分析生命周期。通过大量的代码示例，它解释了如何从不同来源获取数据，使用数据清洗和转换技术准备数据，并进行描述性和推断性统计，以从数据中生成隐藏的见解。

第六章，机器学习，本章解释了各种机器学习算法，它们是如何在 MLlib 库中实现的，以及如何使用流水线 API 进行流畅的执行。本章涵盖了所有算法的基础知识，因此可以作为一个一站式参考。

第七章，使用 SparkR 扩展 Spark，本章主要面向想要利用 Spark 进行数据分析的 R 程序员。它解释了如何使用 SparkR 进行编程以及如何使用 R 库的机器学习算法。

第八章，分析非结构化数据，本章仅讨论非结构化数据分析。它解释了如何获取非结构化数据，处理它并对其进行机器学习。它还涵盖了一些在“机器学习”章节中未涵盖的降维技术。

第九章，可视化大数据，本章介绍了在 Spark 上支持的各种可视化技术。它解释了数据工程师、数据科学家和业务用户的不同可视化需求，并建议了正确的工具和技术。它还讨论了利用 IPython/Jupyter 笔记本和 Zeppelin，这是一个用于数据可视化的 Apache 项目。

第十章，将所有内容放在一起，到目前为止，本书已经分别讨论了不同章节中的大多数数据分析组件。本章是为了将典型的数据科学项目的各个步骤串联起来，并演示一个完整的分析项目执行的逐步方法。

第十一章，构建数据科学应用，到目前为止，本书主要讨论了数据科学组件以及一个完整的执行示例。本章提供了如何构建可以部署到生产环境中的数据产品的概述。它还介绍了 Apache Spark 项目的当前开发状态以及未来的发展方向。

# 您需要什么

在执行本书中提到的代码之前，您的系统必须具有以下软件。但是，并非所有章节都需要所有软件组件：

+   Ubuntu 14.4 或 Windows 7 或更高版本

+   Apache Spark 2.0.0

+   Scala：2.10.4

+   Python 2.7.6

+   R 3.3.0

+   Java 1.7.0

+   Zeppelin 0.6.1

+   Jupyter 4.2.0

+   IPython 内核 5.1

# 这本书适合谁

这本书适用于任何希望利用 Apache Spark 进行数据科学和机器学习的人。如果您是一名技术人员，希望扩展自己的知识以在 Spark 中执行数据科学操作，或者是一名数据科学家，希望了解算法在 Spark 中是如何实现的，或者是一名具有最少开发经验的新手，希望了解大数据分析，那么这本书适合您！

# 约定

在本书中，您将找到许多文本样式，用于区分不同类型的信息。以下是一些这些样式的示例及其含义的解释。

文本中的代码词、数据库表名、文件夹名、文件名、文件扩展名、路径名、虚拟 URL、用户输入和 Twitter 句柄显示如下：“当程序在 Spark shell 上运行时，它被称为带有用户`main`方法的驱动程序。”

代码块设置如下：

```scala
Scala> sc.parallelize(List(2, 3, 4)).count()
res0: Long = 3
Scala> sc.parallelize(List(2, 3, 4)).collect()
res1: Array[Int] = Array(2, 3, 4)
Scala> sc.parallelize(List(2, 3, 4)).first()
res2: Int = 2
Scala> sc.parallelize(List(2, 3, 4)).take(2)
res3: Array[Int] = Array(2, 3)
```

**新术语**和**重要单词**以粗体显示。您在屏幕上看到的单词，例如菜单或对话框中的单词，会以这种方式出现在文本中：“它还允许用户使用**数据源 API**从不受支持的数据源（例如 CSV，Avro HBase，Cassandra 等）中获取数据。”

### 注意

警告或重要提示会以这样的方式显示在框中。

### 提示

提示和技巧会显示为这样。