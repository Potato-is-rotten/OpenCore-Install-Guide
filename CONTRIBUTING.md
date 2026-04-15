# 支持指南

**Note**: 这是一个社区运行的指南，没有被Acidanthera官方认可。请不要就本指南的问题打扰Acidanthera。

想要支持这本指南? 这里有几种方法!

[[toc]]

Note: 希望提供经济支持的朋友们，我们深表感谢，但是我们是一个非盈利组织。我们制作这个是为了教学而不是赚钱。如果你手头有闲置的钱我们强烈建议您将其捐赠给慈善机构。如果您还没有决定捐赠对象，我们推荐 [Crohn's and Colitis Canada (加拿大克罗恩病与肠结石炎协会)](https://crohnsandcolitis.donorportal.ca/Donation/DonationDetails.aspx?L=en-CA&G=159&F=1097&T=GENER)。

## 通过 issue 进行贡献

通过 issue 进行贡献非常简单，但是也有一些规则:

* issue 标签页仅用于讨论指南的问题**禁止个人黑苹果问题**。这不是一个用来讨论安装问题的地方。
* 如果是关于错别字或者需要进一步说明，请注明具体页码。请不要让我们费力去寻找这些问题所在的位置。

你可以在这里找到bug追踪器: [bugtracker (Bug追踪器)](https://github.com/dortania/bugtracker)

## 通过 PR 进行贡献

一些在提供 PR 时的原则:

* 动动你的脑筋(求你了)。
* 请仔细检查你提交的 PR。
* 如果我们认为您的 PR 不符合要求或包含模糊的信息，我们可能会予以拒绝。不过，我们通常会告诉您被拒的原因，或要求您进行修改。
  * 对于较大的提交，若能提供来源信息，我们将非常感谢，因为这有助于我们核实您提供的消息是否属实。
* 图片必须托管在仓库本地的 `../images/`  文件夹下。
* 您的 PR 必须通过 Markdown 语法检查，且所有问题均已解决。
* 通常情况下，尝试避免使用 "非Acidanthera官方" 的工具。一般来讲，我们想要避免使用第三方工具 —— 但如果别无他法，您可以提供相关链接。
  * 明确禁止使用的工具:
    * UniBeast, MultiBeast 和 KextBeast
      * 更多信息详见此处: [Tonymacx86-stance](https://github.com/khronokernel/Tonymcx86-stance)
    * TransMac
      * 已知会导致损坏的 USB 驱动器
    * Niresh Installers
      * 我们希望避免指南涉及盗版行为

### 如何贡献

测试提交内容并确保其格式正确的最佳方法是下载 Node.js 然后运行 `npm install` 来安装依赖项。当你运行 `npm run dev` 时， 它会配置一个本地 Web 服务器，你可以连接到该服务器查看你所做的更改。 `npm test` 还会向你报告任何关于格式和拼写的错误。如果你希望 `markdownlint` 自动修复格式问题，运行 `npm run fix-lint`。

简单的分步指南:

* [Fork此仓库](https://github.com/dortania/OpenCore-Install-Guide/fork/)
* 安装所需的工具:
  * [Node.js](https://nodejs.org/)
* 修改。
* 构建网站:
  * `npm install` (安装所有必须的插件)
  * `npm run dev` (预览网站)
    * 访问地址为 `http://localhost:8080`
* 检查格式和拼写:
  * `npm test`
  * `npm run lint` and `npm run spellcheck` (逐一检查)
  * `npm run fix-lint` (修复潜在的问题)
  * 对于不受默认拼写检查的单词，请将他们添加到 [dictionary.txt](./dictionary/dictionary.txt) 然后运行 `npm run sort-dict`

### 小提示

以下是一些让贡献过程更轻松的工具:

* [Visual Studio Code](https://code.visualstudio.com)
* [Typora](https://typora.io) 实时 MarkDown 渲染。
* [TextMate](https://macromates.com) 简单而强大的批量查找/替换功能。
* [GitHub Desktop](https://desktop.github.com) 更友好的图形界面。

## 通过翻译经行贡献

虽然 Dortania 的指南主要以英文为基础，但是我们知道世界上还有很多其他语言，并非所有人精通英语。如果您愿意帮助我们将指南翻译成其他语言，我们非常乐意为您提供支持。

主要的注意事项:

* 翻译版本必须是独立的分支，且不会合并回 Dortania 的官方指南
* 分支必须注明是 Dortania 的翻译版本，且非官方版本
* 分支必须遵守我们的协议 [License](LICENSE.md)

只要满足上述条件，您可以自由托管您的翻译版本，不会有任何问题！ Dortania 的网站基于 [VuePress](https://vuepress.vuejs.org) 构建，使用 [GitHub Actions](https://github.com/features/actions) 进行部署，并最终托管在 [GitHub Pages](https://pages.github.com)，因此您自行托管的翻译版本无需任何费用。

如果您对翻译或托管有任何疑问或者顾虑，欢迎通过我们的 [Bugtracker](https://github.com/dortania/bugtracker) 来联系我们。

目前已知翻译:

* [InyextcionES](https://github.com/InyextcionES/OpenCore-Install-Guide)(西班牙语)
* [macOS86](https://macos86.gitbook.io/guida-opencore/)(意大利语，不再维护)
* [Technopat](https://www.technopat.net/sosyal/konu/opencore-ile-macos-kurulum-rehberi.963661/)(土耳其语)
* [ThrRip](https://github.com/ThrRip/OpenCore-Install-Guide)(中文，不再维护)
* [sumingyd](https://github.com/sumingyd/OpenCore-Install-Guide)(中文)
* [Potato-is-rotten](https://potato-is-rotten.github.io/OpenCore-Install-Guide/)(中文，正在翻译)
* [Shijuro](https://github.com/shijuro/OpenCore-Install-Guide)(俄语)
* [viOpenCore](https://github.com/viOpenCore/OpenCore-Install-Guide)(越南语)

请注意，这些翻译版本可能因作者偏好、翻译变更及人为失误而有所不同。阅读时请务必留意，因为它们已不再是官方的 Dortania 指南。
