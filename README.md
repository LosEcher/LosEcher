# Los

我关注本地推理、coding agent 和开发工具，平时主要用 Rust 写小而确定的命令行工具。

*Local inference, coding agents, developer tools, and Rust.*

## 在做的东西

**[RepoGuide](https://repoguide.pages.dev)**：中文的开发者精选资讯与工具目录，关注 AI 编程、开源工具和开发实践，每条都附上编辑点评。

**[hud-console-framework](https://github.com/LosEcher/hud-console-framework)**：用 design token 驱动的科幻 HUD 风格界面框架，支持深色和浅色两套配色，不依赖任何库。[在线演示](https://losecher.github.io/hud-console-framework/)

### 给 AI agent 用的 Rust 工具

agent 跑命令、改代码、做验证时，结果要能被程序直接判断。下面这几个工具都只做一件事，并且返回明确的退出码或 JSON。

| 工具 | 用途 |
|---|---|
| [unirun](https://github.com/LosEcher/unirun) | 跨平台执行命令，把不同 shell、编码和本地或 SSH 环境下的输出统一成一份 JSON 结果 |
| [verify-gate](https://github.com/LosEcher/verify-gate) | 按 TOML 清单检查文件、命令、HTTP、git、JSON，用退出码 0 / 1 / 2 表示通过、失败、工具出错 |
| [sandbox-run](https://github.com/LosEcher/sandbox-run) | 在 git worktree 或 jj workspace 里跑构建和测试，不弄脏主工作区 |
| [fmtguard](https://github.com/LosEcher/fmtguard) | 只格式化指定范围的 Rust 代码，格式化前后都有检查 |
| [cargogc](https://github.com/LosEcher/cargogc) | 根据构建记录清理 cargo 不会再用到的缓存，构建进行中时拒绝删除 |
| [rustopt](https://github.com/LosEcher/rustopt) | 实际构建多组 release 配置，选出最小且安全的一组，体积超出预算时让 CI 失败 |

unirun、verify-gate、fmtguard、cargogc 已经发布到 crates.io，可以用 `cargo install` 安装。

### DeepSeek Harness 插件

为 [DeepSeek Harness](https://github.com/deepseek-ai/deepseek-harness) 写的一些插件，包括定时任务、jj 版本控制、Telegram 接入和终端渲染，清单见 [dsplugins](https://github.com/LosEcher/dsplugins)。

## 联系

X：[@LosEcher](https://x.com/LosEcher)
