# R 的重大更新需要重新安装软件包

> 原文：<https://www.dominodatalab.com/blog/significant-update-to-r-requires-re-installation-of-packages>

R 的最新更新于 4 月 24 日下降，将统计计算语言带到了 4.0 版本。该更新包含新功能、错误修复和对现有函数的底层行为和语法的更改，有助于优化代码的实现和可重用性。

由于 R 4.0 中核心组件的变化，R 包将需要重新安装，以确保它们能够正常工作，因为核心库的工作方式发生了根本的变化。这一更新可能会带来模型再现性问题，并带来确保数据科学家团队版本一致的古老挑战，使他们能够共同开发模型，并确保在他们的机器上开发的模型能够由其他数据科学家运行并部署到生产中。

在 R 4.0 中所做更改的完整列表可以在[综合 R 存档网络](https://cran.r-project.org/doc/manuals/r-devel/NEWS.html)中找到。

## 环境管理

环境管理是 Domino 平台的一个关键组件。它使团队能够配置和维护多个分析环境，这些环境可以以安全、无缝的方式轻松应用于他们的项目和工作台，只需最少甚至不需要 It 交互。它不需要开发人员配置他们自己的本地机器或设置新的虚拟环境来测试更新或新的包，并且在部署后可以很容易地推广到其他团队成员。

该功能通常用于创建“黄金标准”生产环境，在该环境中，所有软件包和软件版本都已经过测试和评估，适合生产；此外，在研发环境中，数据科学家可以测试最新、最棒的软件包和软件更新。

与 Domino 中的所有功能一样，环境管理是完全受版本控制的，这意味着可以随时跟踪变化，并且在底层包或软件组件发生重大变化的情况下，可以恢复完整的环境。这对于像 R 4.0 这样的重大升级来说是至关重要的，否则这些升级可能是破坏性的，导致您的模型崩溃。关键是要有一个平台，能够回忆并使用重现模型所需的确切环境，即使是多年以后。

那么 Domino 如何提供帮助呢？

1.  计算环境可以跨用户共享。一旦管理员创建了一个新的 R 4.0 环境，他们可以让每个人立即使用它。没有电子邮件爆料说“这里有关于如何在你的笔记本电脑或环境上升级 R 的说明”。
2.  Domino 允许您拥有多个计算环境，并在它们之间轻松切换。更新 R 需要你重新安装所有的软件包，这很可能会升级你的软件包版本。所以有很多地方可以进行突破性的改变。在 Domino 中，您可以创建一个新 R4.0 计算环境，然后在其上测试您的代码。如果它不起作用，因为你可能依赖于一些维护者还没有更新的包，那么你几乎可以立即切换回来。否则，您将升级您的笔记本电脑/服务器，然后测试您的测试材料，然后再次降级。如果你是单个用户，这是一件痛苦的事，但是如果你有很多用户，这就更让人头疼了。没有电子邮件爆炸出去说“我们今晚升级，所以每个人都可以在 EOD 之前测试他们的东西，让我知道是否有问题”。
3.  最后，由于 Domino 版本和跟踪环境是自动的，升级不会破坏您的旧工作，因为您的旧东西仍然可以在旧环境中运行。事实上，您有代码工作的确切环境和环境版本的记录。没有电子邮件爆料说“有人记得吉姆在离开之前，为我们的季度报告创作情节时使用的是什么版本的 R 吗？”

## 结论

支撑数据科学的工具和技术在不断发展。数据科学团队通常采用的方法是将虚拟机环境作为开发中心，并在为每个数据科学家发布指令以更新他们的开发环境之前测试软件包。这种方法通常意味着包和版本不兼容，需要故障排除，并阻碍数据科学家的进步。

环境管理使数据科学家可以轻松测试新的软件包和软件更新，但更重要的是，这些环境可以在数据科学团队之间轻松共享，这意味着花费数小时来设置环境以测试同事工作的日子已经一去不复返了。

这使数据科学家能够建立值得信赖的黄金标准生产环境，而不会牺牲他们尝试新出现的软件包和软件的自由或灵活性。

有关 Domino 如何管理环境的更多信息，请查看我们的[环境管理概述](https://docs.dominodatalab.com/en/4.1/reference/environments/Environment_management.html)或[联系我们](https://www.dominodatalab.com/contact-us/)进行演示。

[Twitter](/#twitter) [Facebook](/#facebook) [Gmail](/#google_gmail) [Share](https://www.addtoany.com/share#url=https%3A%2F%2Fwww.dominodatalab.com%2Fblog%2Fsignificant-update-to-r-requires-re-installation-of-packages%2F&title=Significant%20update%20to%20R%20requires%20re-installation%20of%20packages)