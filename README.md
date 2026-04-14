---
home: true
heroImage: /dortania-logo-clear.png
heroText: Dortania's OpenCore Install Guide
actionText: Getting Started→
actionLink: prerequisites.md

meta:
- name: description
  content: Current supported version 1.0.6
---

# OpenCore是什么？这个指南是为谁准备的？

OpenCore就是我们所说的 "引导加载程序" – 它是一款复杂的软件，用于为macOS做准备 – 具体而言，是通过注入 SMBIOS、ACPI 表和 kexts 等 macOS 所需的新数据。该工具与 Clover 等其他工具的区别在于，它在设计时就将安全性和质量放在首位，使我们能够使用真实 Mac 上的许多安全功能，例如 [SIP (系统完整性保护)](https://support.apple.com/en-ca/HT204899) 和 [FileVault (文件保险箱)](https://support.apple.com/en-ca/HT204837)。更深入的解析请参阅此处：[为何选择 OpenCore 而非 Clover 及其他方案](why-oc.md)。

本指南主要关于这两方面:

* 在基于 X86 的 PC 上安装 macOS
* 讲解黑苹果系统运行的原理

因此，您需要阅读、学习，甚至使用 Google 进行搜索。这并非简单的 “一键安装” 。

请注意，OpenCore 仍处于早期阶段且目前为测试版。尽管其稳定性相当高，甚至可以说在几乎所有方面都远胜于 Clover，但它仍在频繁更新，因此配置内容会经常变动（例如新 quirks 会取代旧的）。

最后，遇到问题的用户可以访问[r/Hackintosh subreddit](https://www.reddit.com/r/hackintosh/) 和 [r/Hackintosh Discord](https://discord.gg/u8V7N5C) 获取更多帮助。
