# TR-1 最简单的开发环境

?> **该部分内容适合新手**<br/>如果你发现其中内容过于简单，请考虑**跳过以 TR 标识的章节**。

上一节是有关 Bukkit 的历史概要。说了这么多，不编写一个插件似乎说不过去……

?> **什么**？**这就要开始了**？<br/>在本教程中，我不会提前将那些本来应当由你自己发现的内容告诉你。这就像挖矿，使用 XRay 固然很快速，但使用 XRay 挖来的钻石，你能体验到第一次看到钻石的激动、小心挖开周围石头的谨慎、损失一块钻石的伤心吗？<br/>我希望插件开发对你而言是探索的快乐，而不是被迫的无奈。

那么我们要从哪里开始呢？当然是从安装开发工具开始了！

## 确认系统位数

我假设你在使用 Windows，如果你已经开始挑战 GNU/Linux 了，那么你已经知道的相当多，不需要阅读本部分了。

大多数 Windows 都是 64 位操作系统，但偶然也会有例外。我们的开发是需要 64 位操作系统的。

在桌面上右键「此电脑」（Windows 8/10）或「计算机」（Windows 7），单击「属性」，会弹出一个窗口。

取决于你系统的版本，弹出的窗口可能不一样。总之，在窗口中如果能够看到这样的字样就对了：

**64 位操作系统，基于 x64 的处理器**

如果你看到了，那恭喜你！你可以开始开发了！如果你看到的是 **32 位操作系统**，那很遗憾，尝试换一台 64 位的电脑吧。

---

如果系统位数正确（64 位），那我们就该开始设置开发环境了，说是「设置」，其实很简单，我们只需要安装三个软件就可以了。

## JDK 11

首先，下载 [这个文件](https://aka.ms/download-jdk/microsoft-jdk-11.0.18-windows-x64.msi)。

这是 **Microsoft Build of OpenJDK**，是自由软件，如果只是使用的话不存在版权问题，大家尽管使用~

下载完成后双击进行安装，安装过程很简单，一路单击「下一步」即可。中间有个地方需要勾选「我接受许可协议中的条款」，勾选即可。

到这个窗口时，就要小心了！

![SETUP.png](https://www.helloimg.com/images/2023/03/29/o3McBn.png)]

你要这样做：

![SELECT.png](https://www.helloimg.com/images/2023/03/29/o3MdtR.png)

*这让安装程序自动设置了环境变量，方便后续操作。*

单击「Set JAVA_HOME variable 」左边的图标，单击「将安装在本地硬盘上」，单击后，就可以单击「下一步」继续了。安装很快就完成了。

## 服务端

下载 [这个文件](https://cdn.getbukkit.org/spigot/spigot-1.16.5.jar)。这是**服务端核心**。

当然，你也许已经注意到了，这个文件的下载速度很慢（大概要十几分钟吧），但是我们也没办法，因此请大家忍耐一下，如果它下载需要很长时间，可以先做做别的事情。

下载后得到 `spigot-1.16.5.jar`，把它复制到一个合适的地方。

## IDE

下载 [这个文件](https://www.jetbrains.com/zh-cn/idea/download/download-thanks.html?platform=windows&code=IIC)。这是 **IntelliJ IDEA**，一个强大的开发工具。

下载后同样运行安装程序，同意许可协议，安装即可。

IDEA 的安装没有注意事项，全部「Next」就好啦~

---

就这么简单，我们不需要进行任何复杂的配置，只要上面三个都准备好了就 OK 啦~

## Java 语言

Minecraft 使用一种名为 Java 的语言进行开发。有点眼熟？你肯定已经不止一次在启动器中看到它啦！

既然 Minecraft 是 Java 在运行，我们的插件自然也要用 Java 来写。

我们只要把 Java 认识的东西交给它，它就会帮我们解决问题，后面的事情，我们就不管啦~

下一章我们就来编写一些 Java 代码。哦，没学过 Java？不需要！
