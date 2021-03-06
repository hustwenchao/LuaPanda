# LuaPanda

LuaPanda 是一个基于 VS Code 的 lua 代码调试器。设计目标是简单易用，支持多种开发框架。它由两部分组成:

- VS Code Extension  调试器 VSCode 插件
- Lua Debugger  调试器的 debugger 部分

Debugger 主体使用 lua 实现，另含一个 C 扩展模块，以保证高速运行。
LuaPanda 支持 lua5.1- 5.3，运行环境要包含 LuaSocket。



# 特性

+ 支持单步调试，断点调试，协程调试
+ 支持lua5.1- 5.3, 支持 slua/xlua/slua-unreal 等框架
+ 在断点处可以监视和运行表达式，返回结果
+ 可以根据断点密集程度调整 hook 频率, 有较好高的效率
+ 支持 attach 模式，lua 运行过程中可随时建立连接
+ 使用 lua / C 双调试引擎。lua 部分可动态下发，避免打包后无法调试。C 部分效率高，适合开发期调试。



# 项目介绍和接入文档

[项目介绍](./Docs/Manual/feature-introduction.md)	| [快速开始](./Docs/Manual/quick-use.md) | [接入指引](./Docs/Manual/access-guidelines.md) | [FAQ](./Docs/Manual/FAQ.md) 

我们正在补全文档，以方便接入和开发，我们也非常欢迎您可以帮助完善文档。

更多文档请看[这里](./Docs/README.md)




# 快速开始

试用LuaPanda请 [参阅快速开始文档](./Docs/Manual/quick-use.md) ，其中包含 slua , xlua ,slua-unreal 的快速使用方法



# 依赖和适用性

调试器依赖 LuaSocket , 可运行于 slua，slua-unreal ，xlua 等已集成 LuaSocket 的 lua 环境，也可以在 console 中调试。lua 版本支持 5.1- 5.3。



# 参与贡献

我们非常期待您的贡献，无论是完善文档，提出、修复 Bug 或是增加新特性。
如果您在使用过程中发现文档不够完善，欢迎记录下来并提交。
如果发现 Bug，请通过 [issues](https://github.com/Tencent/LuaPanda/issues) 来提交并描述相关的问题，您也可以在这里查看其它的 issue，通过解决这些 issue 来贡献代码。

请将merge request提交在 `dev` 分支上，经过测试后会在下一版本合并到 `master` 分支。

[腾讯开源激励计划](https://opensource.tencent.com/contribution) 鼓励开发者的参与和贡献，期待你的加入。



# 技术支持

如有问题先参阅 [FAQ](./Docs/Manual/FAQ.md) 

QQ群：974257225
