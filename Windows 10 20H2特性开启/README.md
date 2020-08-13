## 可能是 Windows 五年以来最大变化的「新功能」，教你抢先一步用上

原创 化学心情下2 [少数派](javascript:void(0);) *昨天*

今年是 Windows 10 操作系统发布的第五年，作为这个操作系统中最为重要的组成部分之一，开始菜单一直以来都更像是 Windows 8.x 动态磁贴与经典开始菜单的融合产物，在这五年当中的变化并不算大。

![img](images/README/640)

当前 Windows 10 的开始菜单

好在随着微软全新设计语言 Fluent Design 一步步从视频「画饼」走向落地，Windows 10 开始菜单也随之迎来了人们期待已久的升级：今年 3 月，微软在一段视频中展示了将在未来的 Windows 10 版本中亮相的全新文件资源管理器、上下文菜单以及开始菜单，其中开始菜单采用了全新设计的应用图标，动态磁贴本身也从「大色块」设计变成了与菜单背景更加和谐统一的半透明标准磁贴，视觉上更加简洁明快。

![img](data:image/gif;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVQImWNgYGBgAAAABQABh6FO1AAAAABJRU5ErkJggg==)

未来开始菜单的变化，图片来自：blogs.windows.com

也许是 Insider 测试过程中收获了太多好评，虽然上面提到的这些新设计大多都要到 20H2 更新中才会实装，新版开始菜单却提前来到了正式版 Windows 10 v2004 当中——虽然它并非默认开启，我们依然可以通过一些简单的操作进行开启。

![img](images/README/640)

首先确认当前的 Windows 10 版本是最新的 v2004，版本号 19041（可在「Windows 设置 > 系统 > 关于」中查看），也就是最新的 Windows 10 五月更新。

![img](images/README/640)

确保版本为 2004

紧接着打开 Windows 更新设置：「Windows 设置 - 更新和安全 - Windows 更新」，查找更新后选择「可选更新」，找到「2020-07 适用于 Windows 10 Version 2004 x64 系统 (KB4568831)的累积性更新」后勾选安装并且重启系统。

![img](data:image/gif;base64,iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAYAAAAfFcSJAAAADUlEQVQImWNgYGBgAAAABQABh6FO1AAAAABJRU5ErkJggg==)

安装这个可选更新

重启后建议创建一个系统还原点，然后打开文本编辑器（记事本即可），粘贴以下内容，将其保存为 20H2.reg 并放置在桌面：

```regedit
Windows Registry Editor Version 5.00
[HKEY_LOCAL_MACHINE\SYSTEM\CurrentControlSet\Control\FeatureManagement\Overrides\0\2093230218]
"EnabledState"=dword:00000002
"EnabledStateOptions"=dword:00000000
```

双击刚才新建的 20H2.reg 文件，在弹出的警告中点击「是」，然后再次重启电脑。

![img](images/README/640)

点击「是」确定

重启完毕之后点击开始按钮，采用全新设计的开始菜单就出现在我们眼前了。

![img](images/README/640)

是不是比开头那张图里的效果好看多了？

随之而来的还有新版 Alt+Tab 界面和新的系统通知设计，如果你正在使用采用 Chromium 内核的新版 Edge 浏览器，新版 Alt+Tab 界面会把浏览器标签页面直接整合在任务切换操作当中。

![img](images/README/640)

整合了浏览器标签页面的多任务切换

![img](images/README/640)

新的通知设计

当然了，如果你的 Windows 电脑为非生产设备，想要快速体验新版开始菜单还有一个更加「正式」的方法——加入 Windows Insider 计划。

目前 Windows insider 预览计划中分为不同的频道，其中 Dev 频道已经开始测试 21H1 的相关内容，而如果你只希望可以稍微提前一点获得 Windows 10 新功能（比如上面提到的新版开始菜单），直接加入 Beta 频道参与测试即可。

![img](images/README/640)

Windows Insider 官网介绍

加入方法也很简单， 在「Windows 设置 - 更新和安全 - 预览体验计划」中点击开始，选择对应频道后点击 Windows 更新就能获取到测试版系统更新推送了。

![img](images/README/640)

预览体验计划设置

当然，最后还是再强调一次：**Insider 版本不推荐在生产设备上进行安装。**如果你单纯只是想体验更漂亮的开始菜单，使用第一种方法更为稳妥。