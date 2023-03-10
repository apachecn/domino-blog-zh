# 对数据科学工具“购买还是构建”的思考

> 原文：<https://www.dominodatalab.com/blog/reflections-on-buy-vs-build>

“购买 vs 制造”、“不在这里发明综合症”甚至“在这里发明综合症”已经被广泛地写过。我想分享一些关于这个话题的思考，基于我作为一名工程经理(在那里我必须决定是构建还是购买解决方案)和最近作为一名向其他公司销售[平台](https://www.dominodatalab.com?utm_source=blog&utm_medium=post&utm_campaign=reflections-on-buy-vs-build)的创始人的观察。

简而言之，我将使用术语“购买”来表示“使用第三方解决方案”(包括免费或开源的东西)。

## 这是关于你的业务，而不是你的技术

我看过无数的博客文章，从功能和所需的工程努力方面描述了建设与购买的利弊。你正在寻找的第三方解决方案的质量如何；它是否具备您需要的所有功能；学习/集成另一个解决方案与构建您自己的解决方案需要多长时间。

在我看来，这种类型的计算忽略了最重要的问题:你试图为你的公司的业务和竞争优势提供的能力是不是核心？如果你交付的能力是你业务的核心或者使你与众不同的东西，你应该有强烈的偏好去构建，这样你就可以控制自己的命运。如果你提供的是核心业务的外围功能或支持核心业务的功能，你应该倾向于购买，这样你就可以将宝贵的工程资源集中在你的差异化功能上。

这种框架代表了一种微妙但重要的心态转变，与大多数人处理购买还是建造问题的方式不同。考虑一个论点，比如“第三方产品拥有我们需要的所有功能，所以我们自己构建它是在浪费时间”——如果这些功能是您竞争优势的关键，您可能希望构建自己的产品，以便您可以根据需要精确地发展它们。相反，如果一个产品只有你想要的 80%，但它的功能不会成就或破坏你作为一个企业的成功，这可能是更好的选择，这样你就可以专注于你必须做的功能。

举例来说，对冲基金可能会建立自己的时间序列数据库，即使有很多强大的数据库解决方案，包括许多具有强大时间序列支持的解决方案。这是有意义的，因为时间序列的表示和操作对公司的竞争优势至关重要。另一方面，同一家公司管理自己的虚拟主机基础设施是疯狂的。相反，高容量的消费者 web 应用程序可能需要构建和管理自己的托管基础设施，但可能使用现成的数据库来存储指标(作为时间序列)。在做出购买还是构建的选择时，应该深刻、周到地了解什么对您的业务最重要。

这种思路的一个缺陷是，很容易将两种独立的能力混为一谈，而不是认识到一种能力是业务的核心，而另一种能力不是。例如，您可能有对您的竞争优势至关重要的预测模型——但是计算这些模型的网格基础设施可能是许多公司都有的一般性问题。

## 大多数工程师天生就有偏见

大多数工程师是工程师，因为他们喜欢建造东西。所以如果你问一个工程师是自己造好还是自己买好，大多数情况下，她默认的姿势会是自己造。工程师喜欢建造东西并不是坏事——事实上，这很好——但这确实意味着当你询问工程师的意见时，你需要记住这一点。

这是我收到的一封真实的电子邮件，发件人是一位数据科学家，他见过 Domino，认为这将有助于他的团队:

嘿，尼克，
很抱歉延迟回复。我已经和这里的一些开发者聊过了，他们已经决定在内部定制我们的平台。我不太清楚为什么，但这是[公司]的普遍趋势。谢谢你的时间。

或另一封电子邮件:

嗨，尼克，恭喜你！看起来是一个很棒的产品，我的团队对此印象深刻。我不认为它适合我们，因为我们更喜欢自己成长，在需要控制方面犯了错误，但如果这种情况有所改变，我们很乐意让你知道。

不幸的是，这种偏见也经常延伸到技术管理职位。我认识一位工程师，他正在构建自己的消息队列，因为，据他所说，“如果我一直建议现有的解决方案，而不是构建自己的解决方案，我会失去首席技术官的信任。”

当技术人员脱离了对业务的理解，他们自然倾向的影响就被放大了。如果你的工程师认为他们存在的理由是建造东西，而不是“最佳地使用技术来实现我们的关键战略业务目标”，那么你的工程组织，以及你的业务作为一个整体，将会受到影响。

## “我们自己建造一切”

我听到许多工程师和技术经理说他们在内部开发所有的技术。当然，这些公司还没有建立自己的操作系统、编程语言、数据库系统、电子邮件客户端、文本编辑器等。我怀疑他们永远不会考虑为这些功能构建内部解决方案。

我认为这一点认知失调突出了在实践中应用我之前的建议(考虑你的核心/差异化能力)的挑战。具体来说，我怀疑许多公司夸大了他们业务的核心，同时，我怀疑他们低估了构建自己的解决方案的成本。

## 需要考虑的问题

我上面的观察并不意味着购买还是构建总是一个简单的决定。这涉及到各种各样的因素——通常是相互冲突的。一个优秀的技术经理——对相关的业务考虑有着发自内心的理解——将能够切入问题的核心，确定这些问题中哪些与任何特定的环境最相关。

1.  最重要的是，列举您需要从解决方案中获得的功能，并确定哪些功能对您的业务至关重要，即，您需要控制哪些功能，以确保您与竞争对手相比保持差异化。批判性地思考分解这些能力，以识别哪些是特定的，哪些是通用的。例如，你的专有软件可能是一个区别，但这并不意味着你需要一个专有的编程语言；您的预测模型可能是一个优势，但这并不意味着您需要自己的网格解决方案来训练您的模型。
2.  考虑构建您自己的解决方案的机会成本:您的工程师可以做些什么？

3.  可视化持续维护(修复和改进)

-如果您正在构建解决方案，请记住**构建解决方案的 40-80%的“成本”来自持续的支持和维护**。你能承诺吗，或者你想让第三方来做吗？
——反过来，如果你购买一个解决方案，你的改进需求会与供应商或提供商或解决方案的利益一致吗？您会从更新中受益吗，或者解决方案会朝着与您的目标不一致的方向发展吗？

1.  当然，要考虑功能，与您的需求相匹配。第三方解决方案会给你 50%、80%或 100%的你想要的吗？如果有差距，它们是必须拥有的还是最好拥有的？(同样，您对差距的容忍度应该取决于功能对于区分您的业务有多重要。)

-你得到的功能有多复杂？建立和维护自己容易吗，或者实际上相当微妙和复杂？
-考虑集成第三方解决方案的成本。即使它拥有您需要的所有功能，与您现有的环境集成又有多少工作量呢？

## 我们自己的例子

这里有一些我们在构建 Domino 时所做决策的具体例子，关于买什么和构建什么。

*   **购买**:我们使用了第三方工具(Mixpanel)进行用户分析。这是一个普遍的问题，不是我们特有的，也不是我们竞争优势的核心。它很容易集成，虽然它没有做到我们理想中想要的一切，但差距不是大问题。
*   **Build** :我们构建了自己的作业调度器和“自动缩放器”,它们一起旋转 EC2 机器，并将用户的作业分配给集群中的不同机器。有些人认为这是一个疯狂的决定——毕竟，AWS 有自动缩放功能。但是我们发现

*   这个功能是我们产品的核心，所以我们希望对我们如何发展它进行细粒度的控制；
*   我们需要的基本功能集实现起来并不复杂。(我们有了第一个版本，在大约 4 周内部署并运行)
*   集成第三方作业调度程序可能会很麻烦，因为我们需要将我们的领域对象和词汇表映射到一个更通用、更一般化的领域。我们实现的特殊性——根据我们的领域精确定制——使我们在代码库中工作更加高效。

*   **混合**:对于我们的修订版文件存储(支持大文件)，我们采用了混合方法。我们在幕后使用 git，但是我们在此基础上构建了对大文件的支持。我们希望尽可能多地使用现成的，因为版本控制是一个众所周知的复杂问题，所以我们希望从解决这个问题的所有工程中受益。但是 git 不能处理大文件。

我们最终构建了一个与 Github 的[大文件存储](https://github.com/blog/1986-announcing-git-large-file-storage-lfs)非常相似的东西，但是我们差不多两年前就这么做了，那时 Github 的解决方案还不存在。(如果我们现在做，我们可能会使用他们的解决方案。)我们查看了 [git-annex](https://git-annex.branchable.com/) 和几个类似的解决方案，但它们似乎都没有给我们想要的控制，并且/或者集成的复杂性会令人尴尬。所以我们选择主要使用 git，并在上面进行我们自己的定制开发，尽可能做到最小化。