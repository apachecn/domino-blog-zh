# 从科学的再现性危机中吸取教训

> 原文：<https://www.dominodatalab.com/blog/learn-reproducibility-crisis-science>

*关键亮点来自 Clare Gollnick 的演讲《推论的极限:数据科学家能从科学中的再现性危机中学到什么》，在这篇多米诺数据科学领域笔记中有所涉及。完整视频可在[这里](https://www.youtube.com/watch?v=bvU-q61mWsY&t=560s)观看。*

## 介绍

在 Clare Gollnick 的圣何塞演讲“推理的极限:科学家可以从科学的再现性危机中学到什么”中，Gollnick 讨论了如何将数据转化为见解是一项挑战。虽然推理是数据科学家可能用来揭示洞察力的工具，但通过持续搜索、 [p-hacking](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1002106) ，以及机器学习中的[过度拟合](https://www.youtube.com/watch?v=u73PU6Qwl1I)，有可能打破推理。这潜在地导致了科学界的再现性危机。Gollnick 是一名前数据科学家，现在是铽实验室的首席技术官，他提倡数据科学家从科学中的再现性危机中吸取教训，认识到推理的局限性，并将推理作为解决适当问题的工具。

## 再现危机

在 2011 年[,一位风险投资人提到](https://lifescivc.com/2011/03/academic-bias-biotech-failures/),一条“潜规则是至少 50%的研究发表在顶级学术期刊——《科学》、《自然》、《细胞》、《PNAS》等...——工业实验室不能重复得出同样的结论”。在 Gollnick 的演讲中，Gollnick 引用了多项研究，包括[拜耳 2011 年研究](https://www.nature.com/articles/nrd3439-c1)、[安进研究](http://sitn.hms.harvard.edu/flash/2013/house-of-cards-is-something-wrong-with-the-state-of-science/)，以及许多实验室复制项目，指出了科学中的再现性危机。这种可复制性危机可能已经导致数百人在可能并不存在的重大影响下学习和创造职业。正如演讲的标题所言，数据科学家有机会从科学的再现性危机中吸取教训。Gollnick 还指出“我们用来从数据中进行推断的逻辑系统中的一个根本缺陷”导致了科学中的再现性危机。

## 推理的局限性

Gollnick 在谈话中指出“推理被搜索打破”。例如，Gollnick 提到“假设检验中的 p 值是对惊奇的量化”。人们寻找惊喜的次数越多，就越容易看到惊喜。或者，有人越频繁地运行和重新运行相同数据的模型，直到他们得到他们想要的重要结果，打破推理，这也被称为 [p-hacking](http://journals.plos.org/plosbiology/article?id=10.1371/journal.pbio.1002106) 。另一个打破推理的例子是机器学习中的[过拟合](https://www.youtube.com/watch?v=u73PU6Qwl1I)。当有人“搜索太多模型，当[他们]愿意一次考虑太多假设，当[他们]搜索太多参数，或给模型太多自由度”时，过度拟合就会发生。然而，交叉验证在机器学习中被用来修复过度拟合。交叉验证包括“分离你的训练数据，在此基础上生成假设和模型，然后测试一次”。Gollnick 在演讲中还建议数据科学家设计问题，这样他们就可以“尽可能少地进行物理推断……依靠从尽可能少的数据中学习，因为演绎法是比归纳法强得多的逻辑体系。

## 假阳性的潜在影响

在演讲中，Gollnick 谈到，理解推理的局限性会导致“对数据作为一种工具的强大理解，你可以利用它成为一名更好的数据科学家。”例如，Gollnick 引用了过去十年中广泛的癌症筛查是如何导致假阳性的。筛查方案已经变得不那么频繁，并考虑该人是否属于高危人群。虽然有些人可能更喜欢假阳性，但 Gollnick 也要求观众考虑“我们可能正在治疗他们没有患的癌症的可能性。想想化疗的作用……人们可能会死于癌症治疗。”Gollnick 提到“寻找更少和更有针对性的人群”的方法目前正在使用，“因为当你的搜索更有针对性时，数据和证据会更好地发挥作用。”

## 结论

在 [Strata talk](https://www.youtube.com/watch?v=bvU-q61mWsY&t=560s) 中，Gollnick 讲述了数据和推断是如何成为工具的。有潜力有效解决正确问题的工具。然而，工具也有局限性。例如，Gollnick 提到了那些没有考虑如何“理解数据，推断的极限”的科学家是如何导致再现性危机的。Gollnick 在结束讲话时重申，数据是一种工具，“当你是数据科学的从业者时，如果你有选择，就选择正确的问题。”

*^(Domino 数据科学领域笔记提供数据科学研究、趋势、技术等亮点，支持数据科学家和数据科学领导者加快工作或职业发展。如果您对本博客系列中涉及的数据科学工作感兴趣，请发送电子邮件至 writeforus(at)dominodatalab(dot)com。)*