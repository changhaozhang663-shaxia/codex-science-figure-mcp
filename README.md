# Codex 科研绘图 MCP

通过本地 MCP 连接桌面版 Adobe Illustrator 和 Microsoft PowerPoint，创建与修改可编辑科研图和演示文稿。

## 下载

- [下载 Illustrator MCP 0.2.0（Windows x64）](https://github.com/changhaozhang663-shaxia/codex-science-figure-mcp/releases/download/v2026.10.02/Illustrator-MCP-0.2.0-Windows-x64-20261002.zip)
- [下载 PowerPoint MCP 0.1.0（Windows x64）](https://github.com/changhaozhang663-shaxia/codex-science-figure-mcp/releases/download/v2026.10.02/PowerPoint-MCP-0.1.0-Windows-x64-20261002.zip)
- [完整发布说明与 SHA-256 校验文件](https://github.com/changhaozhang663-shaxia/codex-science-figure-mcp/releases/tag/v2026.10.02)

请下载上述对应安装包。源码、运行依赖、中文说明和测试均包含在安装包中；GitHub 自动生成的 Source code 压缩包不包含运行依赖。

## 安装

电脑需准备 Windows x64、x64 Node.js 22 或更新版本、Codex，以及可正常使用的对应桌面软件。PowerPoint 原生图表需要可用的 Excel 组件。

1. 完整解压 ZIP 到固定的可写目录，阅读“先看这里.txt”。
2. 双击 `setup.cmd`，按提示注册本地 STDIO MCP 服务。
3. 重启 Codex，开启新对话，打开对应软件。
4. 输入“检查 illustrator-local / powerpoint-local 的连接状态、版本和工具列表”。

两个连接器可同时安装。运行依赖随包附带，安装器不需要下载 npm 包；Node.js 与 Adobe/Office 软件需自行准备。

## 视频演示

- [用 Codex + Illustrator MCP 画科研机制图：完整绘制过程](https://www.bilibili.com/video/BV1QAa96QEFp/)
- [Codex 连接 PowerPoint：一张视网膜机制图是怎样画出来的？](https://www.bilibili.com/video/BV1iia96FETc/)

## 使用示例

Illustrator：

> 通过 Illustrator 连接器新建 180 × 120 mm 的 RGB 文档，绘制可编辑的细胞信号通路示意图。先检查字体，为对象命名并分层，分批刷新画面。完成后预检、预览，导出 AI、PDF、SVG 和 600 dpi PNG。

PowerPoint：

> 通过 PowerPoint 连接器新建 16:9 文稿，用原生可编辑文字、形状和连接线绘制实验流程图。给对象命名并分批刷新。完成后预检、预览，另存为 PPTX、PDF 和 600 dpi PNG。

## 检查与范围

`check.cmd` 检查文件完整性、运行依赖和 MCP 握手。实际桌面软件连接可在 Codex 中检查，或在包目录执行 `node src/doctor.mjs`。

分享包包含源码、依赖、中文说明、测试与完整性清单。第三方依赖保留各自的许可文件。工具的详细功能、恢复规则与验证范围见包内 README.md、PACKAGE-VERIFICATION.md 和 VERIFICATION.md。

2026-10-02 分享快照：Illustrator 14 项自动化测试通过，PowerPoint 10 项通过；两个 ZIP 的解压启动检查均通过。支持的应用版本与其他限制见各包说明。
