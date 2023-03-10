# 在社会科学中寻求再现性:探索与发现

> 原文：<https://www.dominodatalab.com/blog/seeking-reproducibility-within-social-science-search-and-discovery>

*[NYU 大学教授、经济学家、柯勒律治倡议的联合创始人 Julia Lane](https://wagner.nyu.edu/community/faculty/julia-lane) 在 Rev. Lane 上发表了题为“数据在哪里:社会科学搜索的新方法&发现”的演讲，描述了柯勒律治倡议正在采取的应对科学再现性挑战的方法。该方法旨在为政府分析师和研究人员提供远程访问安全数据设施中的机密数据的机会，并通过应用数据分析培训计划建立分析能力和协作。本文提供了 Lane 在 Rev 的演讲的摘要和文字记录。非常感谢 Julia Lane 在发表之前对本文提供了反馈。*

## 会话摘要

科学正面临着研究的可重复性挑战，这阻碍了数据科学家和研究人员加快工作速度和提供影响其组织的见解的能力。[自从多米诺成立](https://blog.dominodatalab.com/model-management-era-model-driven-business/)以来，我们[通过](https://support.dominodatalab.com/hc/en-us/articles/205032985-Sharing-and-collaboration)[持续更新](https://blog.dominodatalab.com/announcing-domino-3-4-furthering-collaboration-with-activity-feed/)平台的协作功能，解决了可再现性问题，以支持我们的客户，并为[博客](https://blog.dominodatalab.com/tag/reproducibility/)和行业[活动](https://blog.dominodatalab.com/managing-data-science-as-a-capability/)上的整体公众讨论做出了贡献，包括[修订](https://rev.dominodatalab.com/)。在 Rev 会议“数据在哪里:社会科学搜索&发现的新方法”中，Julia Lane 就柯勒律治计划如何通过为政府分析师和研究人员提供对机密数据的安全远程访问来应对可再现性挑战，以及如何通过应用数据分析培训项目建立分析能力和协作提供了见解。目标是使政府机构能够利用更高质量的数据做出更好的循证决策。Lane 忠于再现性的精神，讲述了如何使用这种方法来允许认可的分析师重用和吸收见解，以加速他们的工作。莱恩讨论了柯尔律治试图回答的问题；提高与使用关联数据相关的分析的严密性；柯勒律治如何建立和测试一套工具，用来识别哪些数据被用来解决不同的研究问题；以及当新的研究人员带着新的项目访问安全环境时，如何使用该方法来通知他们。Lane 在会议结束时谈到，该计划的目的是“建立基于证据的政策制定，从而获得更好的知识、更好的政策、更好地分配资源，并减少收集信息的成本和负担。”

本次会议的一些亮点包括

*   如何利用现代方法以更低的成本获得更高质量的数据，以帮助支持循证决策。
*   共享机密政府微观数据的独特挑战，以及访问在生成高质量推断中的重要性
*   风险-效用权衡的务实评估，或更多数据使用导致的风险与泄露或重新识别风险的权衡
*   讨论柯勒律治如何利用培训课程培养政府机构工作人员应对数据质量挑战的能力
*   研究人员培训与安全环境中的访问配对的重要性。

书面记录中提供了更多见解。

## 副本

朱莉娅·莱恩:

我是一名训练有素的经济学家，这也是我的工作重点。让我告诉你这个故事。我在 NYU，你可以从我浓重的纽约口音听出来，我职业生涯的大部分时间都在联邦统计机构工作，这些机构为你提供十年一次的人口普查、失业率、国内生产总值等等。在使用这些数据进行决策时，您面临的一个主要挑战是，收集数据的成本非常高，而且数据的质量正在下降。

你们中有多少人知道十年一次的人口普查将在明年进行？好吧。你认为美国大约有多少人？3.5 亿，3.6 亿，也许明年我们会发现更多。你认为收集…数一数这些人需要多少钱？三亿六千万美元。试试北边。20 亿美元，有人出 20 亿吗？好吧。有人想再高点吗？更高，更多，更多。170 亿美元，好吧，去数人数，问他们 10 个，也许 11 个问题。对吗？我们面临的挑战是数据质量正在下降。人们没有回应，他们给出了不好的回应，等等。

大约三年前，循证决策委员会成立，它汇集了来自全国各地的专家，研究如何开发数据，以更高的质量和更低的成本做出决策。他们提出了一系列建议，并于今年被纳入循证决策法案。

他们要求 NYU 建立一个环境来为委员会的审议提供信息，并展示如何将来自多个来源的数据汇集在一起，并在质量水平上理解它们，以便能够分配资源来做出决策。这就是为什么它被称为循证政策。

当然，整合数据的挑战在于数据，尤其是人类的数据，是相当复杂的。当它来自多个不同的来源时，就不仅仅是将它们混合在一起的问题了。你需要了解它们是如何产生的，问题是什么等等。除此之外，我们还建立了培训课程，培训政府机构工作人员、研究人员和分析师，他们希望处理数据、解决问题……以及如何处理数据。

挑战来了。当你处理复杂的数据时，当它是机密的时，因为它是关于人类的数据，所以很难找出以前对他们做过什么。每次有人开始处理数据时，都是一片空白。你搞不清楚是怎么回事。我们必须解决的挑战是我今天要和你们谈的挑战，那就是当你登陆一个新生成的数据集时，你如何发现，它没有以任何方式被策划....我怎么知道里面有什么，我怎么知道还有谁用过它？如果你仔细想想，这是一个 Amazon.com 问题，对吗？

杰夫·贝索斯赚了这么多钱的原因是他解决了弄清楚书里有什么的问题，通过其他人使用这本书的方式产生的信息来弄清楚，而不仅仅是人们生产这本书的方式。我们想要做的是为数据建立一个 Amazon.com，这就是我今天要讲的故事，让你们对我们试图建立的平台有一些了解。

我所说的新类型的数据是什么？过去，数据通常是由填写调查表的人生成的，对吗？一个统计机构收集它，策划它，记录它，发出它。也可能是管理记录，即从政府项目管理中生成的记录，如税务数据。如今，我们也在关注新类型的数据，由传感器生成的数据集，由您的刷卡生成的数据集，如零售贸易数据、万事达卡或 IRI 数据或您的 DNA。这些是复杂的数据集。它们不是精心策划的，但它们可以增加很多关于如何分配政策的理解。

这些数据需要共享。我们面临的挑战是，当它是人类的机密数据时，有许多关于分享知识的禁令，这是很正确的。与您习惯处理的开放数据世界相比，一切都更加孤立。例如，如这张幻灯片所示，每次有儿童死亡时，巴尔的摩市的委员们都会聚在一起，分享他们接触到的所有政府项目的信息。可能是住房、教育、福利、寄养等等。但他们唯一分享知识的时候是孩子死了的时候。我们在这里试图做的是建立一个知识基础设施，使我们能够在儿童死亡之前分享知识，以改善政策。

但挑战是，这是一个风险效用权衡，使用机密数据的价值在于，越多的人和越多的人使用它，政策就越有利，但泄露的风险也越大。你必须做的是，你必须尝试和管理这种披露。如果可以，你真的可以制定更好的政策。新西兰是一个很好的例子，这些幻灯片是由前总理比尔·英格利希制作的。像大多数国家或城市一样，你知道，有三大支出领域:教育、卫生、养老金。如果你想更好地分配资源，你要做的是更好地利用从多个政府项目中产生的综合数据。

例如，我所说的集成数据是什么意思？这是一个孩子，这个孩子的年龄在这里，底部是纳税人的成本，不仅仅是其他东西。你看看这个孩子如何打击儿童，青少年，家庭服务，虐待，寄养，教育，青少年司法，收入支持或福利，对不对？孩子出生，到大约两岁半的时候出现在儿童、青少年、家庭服务和虐待通知中。你开始看到孩子在这里，更多的虐待，更多的家庭服务的访问。开始接受教育，大约 9 岁，10 岁，11 岁，断断续续的接受教育，17 岁时被送去看护，他参加了青少年司法，然后去了收入补助。如果你把这些信息放在一起，这是很容易预测的。我不需要在这里反复讨论与之相关的问题。

那种信息，如果你把它放在一起，理解它，可以帮助分配资源。这是获得学校证书，教育资格。如果孩子在 18 岁时得到它，现在，在未来会有很好的状态。如果他们没有得到它，这是一个非常糟糕的指标。你可以根据数据进行排序，你可以对一个孩子在 18 岁之前获得或未获得学校证书的可能性进行排序，你可以找出哪些孩子没有获得证书的风险最高。如果你分配资源远离，你知道，像我的孩子一样的孩子，他们不需要干预。他们不需要这些孩子需要的服务。你可以重新分配资金，你可以极大地降低纳税人的成本，改变这些孩子的生活。

正是这种观点导致了循证决策法案的产生。最重要的是，你如何在一个信息交换中心安全地将数据放在一起？我所说的这种工作可以由政府分析师和研究人员以一种安全的方式实施，从而将重新鉴定的风险降至最低。

我们建立了一个清算所。我们称之为行政数据研究机构。我不喜欢清算所这个术语，原因有很多。它必须是项目…任务特定的，所以我更喜欢设施这个术语。但关键的事情不仅仅是建立信息交换机构，还要建立一个与之配合的培训项目。

我不会讲太多细节，但基本的想法是你会有一个安全的环境。当然，一个主要的挑战是你必须有遥测技术来判断谁在访问它。但是你也需要在数据周围有元数据。你需要有一个丰富的上下文，因为如果它只是 0 和 1，我不知道它是什么。你们中许多使用过开放数据的人会注意到，开放数据在质量方面可能有点不可靠。挑战的一部分是数据生成的方式，这有点…有大量的数据被放在一起进行汇总，并且没有任何电缆连接到微数据引擎。你真正需要的是你希望数据用户参与到元数据文档中。

换句话说，再一次，用统计系统做类比，机构产生数据的方式作为人类使用，他们非常辛苦地创建元数据文档，你得到一个关于所有变量的意义，它们是如何产生的等等的报告。高度手工的过程。我们想要做的是，我们想要生成一种自动的方法来找出数据中有什么信息，以及这些信息的质量如何。让我给你一点味道。在其中一个班里，我们有前科犯的资料。纲领性的问题是，获得工作的机会和社区特征对前罪犯的收入和就业结果有什么影响，以及他们随后的再犯率。

这就是我们所处的位置…为什么这一切都在[听不清 00:14:09]上，它们在来回移动。如果能把隐性知识编纂成册，这样当人们开始处理数据时，元数据文档就会自动生成，就像 Amazon.com 一样，这不是很好吗？对吗？这是基本的想法。你知道，不是你说，“数据从哪里来，它是如何根据它产生的方式被记录的，”而是社区告诉你一些关于数据是什么的事情。

好吧。这是我的挑战。我想弄清楚，当我登陆一个数据集时，还有谁在什么主题和什么结果上处理过数据。然后我想创建一个贡献知识的社区。这有点像数据的 Amazon.com。

好吧。我要怎么造一台能做到这一点的机器呢？还记得那些统计机构吗，我在开始的时候抨击过他们，但是，你知道，这些都是很棒的人。这些人工作努力，很棒，有很大的动力，但他们就像是工业革命前的数据工厂。现在，我们正在尝试建立一个现代化的数据工厂，一个自动化元数据生成的现代化方法。

本质上，我们要尝试并弄清楚如何做的是我们要确定问题的范围，将它提交给计算机科学社区，自然语言处理，机器学习社区，并说，“你能想出如何从中学习，自动化，冲洗和重复吗？”这是核心观点。我们感兴趣的是谁以前处理过这些数据，识别他们，然后弄清楚他们用这些数据做了什么。如果你想一想，所有这些知识都包含在出版物中，无论是出版的作品、工作论文还是政府报告。它在某个文件里。在那份文件中，如果是实证的，有人说，“这是我的问题，这是我要用它做什么，这是描述数据的部分。”

我想做的是，我想让计算机科学家们帮我找出数据集在哪里，以及语义上下文将把我指向哪里。好吧。然后我会让整个社区告诉我他们这样做是对还是错，然后从那里解决它。

本质上，我们与美国农业部合作的一个社区。但是不管怎样，美国农业部，你会看到他们关注的一个东西是 NHANES，营养教育数据集。你会看到这里，这里有写着分析样本的东西。他们说了一些关于数据的事情。我们想要的是计算机科学家去找出数据在哪里。

我们就是这么做的。我们举办了一场比赛。我们手动收集了一个语料库。社会科学数据仓库，公共使用的，坐落在全国不同的地方。一个是在密歇根大学，你有 ICPSR。有三个人，他们每天的工作是阅读论文，并手动说出哪个 ICPSR 数据集在该语料库中。然后他们把它写下来，然后把它贴出来，说已经做了什么。我们收集了这些语料，然后进行了一场比赛。我们有来自世界各地的 20 支队伍参赛。他们中的 12 个人提交了代码，这里有四个非常善良的人帮忙做了广告，非常感谢。然后我们有四个决赛选手。实际实现的模型是…我们很惊讶他们居然能做到这一点。

好好想想。如果我拿起一份出版物，它……你能告诉我里面引用的数据集是什么吗？答案当然是否定的。基线是零。胜出的算法所做的是，它正确识别了出版物中 54%被引用的数据集。这太神奇了，对吧？

现在还有很多工作要做。我已经跳过了所有的错误和问题等等，但它仍然是超级令人鼓舞的，对不对？因为现在，一旦我把数据集链接到出版物，这给了我丰富的背景，这给了我找到其他一切的潜力，因为有很多工作是由我在数字科学，UberResearch 的同事在出版物上做的。它们与过去 10 年的出版物相关联:拨款、政策文件、专利、临床试验等等。一旦我拿到那对，我就要去比赛了，对吗？这使我能够为一个特定的出版物找出围绕它的一切。这是我的目标。

围绕这一点，现在有许多工作要做。但是，举个例子，这是一个 Dimensions 网站，我没有时间去直播，因为我会被吼，但是我可以给你直播，你可以输入数据集，你会得到很多相关的信息。你找出研究人员是谁，相关主题是什么等等。这将给我带来我一直在寻找的知识。这是一个相当有缺陷的模型，尽管它是惊人的。你知道，有大量的工作要做。

现在我们想做的是去把那一对清理干净。最大的问题是，你可能已经发现了这一点，但我们搜索的是有标题的数据集。它被称为美国社区调查或 NHANES 或 PSID 或类似的东西。如果有很多人类处理的数据集，他们会说，“哦，我们在处理 LinkedIn 的数据，我们在处理 Twitter 的数据，”这些数据没有标签，或者没有零售 IRI，零售扫描仪数据，它们实际上没有一个你可以找到的标题。我们需要从语义语境中获得更好的知识。这意味着我们需要开发一个语料库，一个可以训练机器学习算法的带标签的语料库。

我们正在研究数字科学中的维度，我们也试图以多种不同的方式获得人类策划的输入。一个是与出版商合作，[听不清 00:22:01]，当作者提交出版物时，他们说，“你能给我们一些关键词吗，”我们可以告诉他们，“给我们一些…告诉我们那里有什么数据集。”对吗？如果他们告诉我们那里有什么数据集，我马上就能得到一个二元组。对吗？然后我就可以训练了。

当研究人员进入一个安全的环境，然后他们询问有什么数据集可用时，你也可以让他们贡献他们的知识。在课堂上，我们通过 300 名政府分析师，他们是主题专家，我们可以让他们告诉我们他们对可用于公共利益的数据集的了解。如果你们中有人是社会科学家，请到这里来，我们要求我们的同事来填写。事实证明，你知道，如果我们得到一千个精心策划的公共数据集文档，这将足以看到下一次迭代。

这是我们接下来要去的地方。给我们带来替代数据的那些数字科学家。事实证明，人们真的喜欢…他们去那个闪亮的小徽章，Altmetrics 徽章，并点击它。我们正在设计的是，如果你现在输入并寻找一个数据集，我们也与德意志联邦银行合作，它将会调出相关的出版物。这里的想法是，每一个被拉起的出版物，你得到那里的数据集上下文，它会说有多少专家，多少论文，多少代码书，有多少注释与它相关联。然后当你点击它，弹出更丰富的上下文，我可以找到所有的论文，其他论文，专家，代码书，注释和相关的数据集。然后这里是行动的号召，对吗？我们不需要让每个人都响应，但我们会尝试一下，看看我们在这方面做得如何。然后，当然，把它输入到这个方法中。

最后一步，也是与布莱恩·格兰杰和费尔南多·佩雷斯合作的一步，是将其构建到 Jupyter 笔记本中。Fernando 和 Brian 一直在做的一件事是，他们试图让练习册更具协作性。因为现在，这只是一个单一的计算叙事。他们也试图与他们合作，为了我所说的所有原因，能够与机密的微数据合作。

基本思路是这样的。目前，当你登陆一个数据集时，如果你幸运的话，你所得到的是数据集产生的方式所产生的数据。类比的例子还是杰夫·贝索斯。当你找一本书时，你发现了什么？ISBN 号，作者，书名，出版商，对吗？那是元数据，顺便说一句，书是制作出来的。你真正想要的是关于数据本身的知识。我不需要去书店寻找答案，我只需要找到像我一样的人使用了这些信息。同样，我们正在将这一点构建到 Jupyter 笔记本中，我们 Jupyter 团队正在与我们的团队合作，这里的概念是记住我们曾经的松散通信，将其构建到注释中。这是 Brian 和 Fernando 刚刚放入的内容，但将其构建到注释中，隐性知识被编码并构建到数据基础架构下的图模型中。

这就是故事的梗概。我们希望能够建立基于证据的决策，从而获得更好的知识、更好的政策、更好地分配资源，并降低收集信息的成本和负担。我们首先构建了一个安全的环境，并围绕它培养了员工能力。我们现在正处于这个阶段。我们的目标是建立一个平台。

如果你想了解更多信息，我们在风景优美的纽约州 NYU 招聘员工。很多信息都在这里，也在我们的网站上。你可能想知道为什么它被称为柯勒律治倡议。你们中有多少人听说过塞缪尔·泰勒·柯尔律治？太好了。好吧。因《老水手之歌》而出名，对吗？我们试图找出这个东西的名称，我们想，“为公众利益服务的数据科学”，[blech]“基于证据的政策”，[blech]。柯勒律治倡议似乎是显而易见的，对不对？《古舟子咏》“水，到处都是水，也没有一滴可以喝”，对吗？在这里，它是“数据，到处都是数据，我们必须停下来思考。”这就是为什么它被称为柯勒律治倡议。

为了便于阅读，本文经过了编辑。