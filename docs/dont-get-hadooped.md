# 不要被 Hadooped 化

> 原文：<https://www.dominodatalab.com/blog/dont-get-hadooped>

![Hadoop elephant](img/c95e761891f32b87312817a96452a003.png)

我见过许多公司对提高他们的分析能力感兴趣，我注意到一个令人不安的模式:在许多情况下，公司被 Hadoop(或 Spark，或类似的解决方案)所吸引，不是因为它解决了他们的实际问题，而是因为它是一项闪亮、时尚的技术。

不要误解我的意思:Hadoop(及其同类产品)是一项了不起的技术，有很多问题需要它。但这并不意味着这对每个人都是正确的，甚至是有益的。我想描述当人们非理性地被 Hadoop 吸引时，我看到的三个常见错误。

## 1:中等数据

有人说“大数据就像高中的性:每个人都在谈论它，每个人都声称他们正在做，但几乎没有人在做。”通常，当有人告诉我他们有大数据时，我问他们实际上有多少数据，他们不好意思地回答大约 10 到 100GB。

### 如果您的数据可以容纳在标准 EC2 机器的内存中，那么您就没有大数据

对于真正的大型数据集:互联网规模的数据、生物信息数据、一些金融交易数据等，Hadoop 是一个很好的解决方案。但是如果你的内存小于 250GB，那么你的整个数据集可以放在一台机器上。这台机器甚至有 32 个内核，这使它成为运行一些地图缩减工作的一个非常好的工具。

## 2: Hadoop！=地图-缩小

我还听说有人将 Hadoop 和 map-reduce 混为一谈。Hadoop 是一个强大的 map-reduce 版本，但是使用 R、Python 和其他统计语言的强大库，在单台机器上运行 map-reduce 分析非常容易。所有这些语言都有很好的工具来[将你的任务映射到多个内核上](http://blog.dominoup.com/simple-parallelization/)。您甚至可以使用 IPython Notebook 中的[集群来跨内核映射您的任务。](http://ipython.org/ipython-doc/2/parallel/parallel_intro.html)

同样，除非您的数据规模需要超过 100 个内核或几千兆字节的内存，否则您可能不需要 Hadoop 的复杂性和维护成本。在一台机器上使用 Map-reduce 可能对您有好处。

## 3: Hadoop 是一种技术，而不是解决方案

我看到的公司陷入的最常见、也是最微妙的陷阱可能是，当他们并不真正了解他们的实际问题时，他们期望 Hadoop(或其他一些热门技术)成为解决方案。通常情况下，当一家公司想要提高其分析能力，但不知道如何开始时，就会出现这种情况。他们听说时尚的技术产品，他们相信将这些产品带到船上可以让他们朝着正确的方向开始。

## 在寻求“大数据解决方案”之前...

当我们深入了解公司时，我们经常会发现一系列需要不同解决方案的问题。没错，它们更复杂，但它们是基础问题，一旦得到解决，将会产生真正的影响。

我接触过的公司最大的问题通常是缺乏一个标准化的工作流程来促进最佳实践。当我就如何支持现代分析能力给出建议时，通常会从良好的卫生习惯开始:

*   保持工作集中化，以实现共享和知识管理。
*   使用版本控制，这样您就可以复制过去的工作。

*   组织您的工作，使其便于携带，也就是说，它不依赖于任何特定人的机器。(这包括移除对绝对文件路径、系统级库等的隐藏依赖。)

*   编写您的代码，使其模块化，以便可以重用正确的部分，并公开正确的参数(而不是硬编码)。

*   在模型的整个生命周期中使用单一语言进行工作(交互式的探索性工作，通过细化，直到部署)。不要创造一个在过程的不同阶段需要在不同语言之间翻译代码的世界。

Hadoop 不是这些问题的解决方案。事实上，在 Hadoop 上构建一个分析工作流，而不考虑你真正的问题是什么，你很容易就会制造一个不可持续的混乱。

## 诊断你真正的问题

以下是您在寻求“大数据”解决方案之前应该问的一些问题:

*   围绕您当前的分析能力，您最大的问题和痛点是什么？如果你可以“挥动魔杖”改变你的分析过程，那会是什么？
*   大数据解决方案能否真正解决您的痛点？如果是，还需要哪些*或*才能将一项技术(例如 Hadoop)转化为实际的商业价值？例如，是否有任何工作流或业务流程需要更改？这些改变将花费或需要什么(例如，改变当前代码以在 Hadoop 范例中工作)？

*   根据内核和内存，通过分析计算出您实际需要多少计算资源。你可以通过一些简单的数学计算来做到这一点:

    *   你有多少数据？
    *   它能被分成多少个独立的“部分”？

    *   你计算每一部分要花多长时间？

    *   您希望在多少时间内完成整个计算？

举个简单的例子:我和一家成熟的分析咨询公司谈过，这家公司坚持认为他们需要在 Apache Spark 之上建立一个内部解决方案。当我询问他们的具体使用情形时，他们表示需要处理包含 10，000 条记录的数据集，其中每条记录需要 10 秒钟的处理时间，并且他们需要一个能够在几个小时内完成计算的解决方案。但是在一台 32 核的机器上，这需要不到一个小时。

## 替代解决方案

如果我没有简单地提到我们已经建成了一个[数据科学平台](https://www.dominodatalab.com?utm_source=blog&utm_medium=post&utm_campaign=dont-get-hadooped)，在整个分析生命周期中促进最佳实践，那将是我的失职。当然，Domino 可以很好地与 Hadoop 集成——Domino 可以运行和跟踪 Hadoop 作业，就像它可以运行和跟踪 R、Python 和其他语言中的任务一样——但可能实际上并不需要 Hadoop。或者至少，你可能需要*和*一个精心设计的平台来放置它。

## 散布消息

如果你或者你认识的其他人曾经是闪亮技术综合症的受害者，并且在你不需要 Hadoop 的时候爱上了它，请把这个分享给他人。