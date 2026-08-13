# SDLC Harness 文档

这是 [SDLC Harness](https://github.com/Caesarlo/sdlc-harness) 的用户文档站点，用 [Mintlify](https://mintlify.com) 构建，内容全部是 `.mdx`。

SDLC Harness 是一个仓库原生的 SDLC 治理 CLI：把需求、功能状态、依赖、验证证据和交付规则保存在代码仓库里，让开发者和编码 Agent 按同一套可执行规则协作，而不是依赖聊天记录和自我声明的"已完成"。这个仓库只维护文档，工具本身的源码在 `sdlc-harness` 主仓库。

## 文档结构

| 目录 | 内容 |
| --- | --- |
| `index.mdx` | 首页：工具是什么、最重要的特点 |
| `concepts/why-sdlc-harness.mdx` | 为什么需要它：真实失效模式与对应机制 |
| `concepts/how-it-works.mdx` | 工作原理：仓库状态、功能生命周期、九阶段工作流 |
| `quickstart.mdx` | 5 分钟接入指南 |
| `guides/` | 日常工作流、团队与多 Agent 协作 |
| `reference/` | 命令参考、配置参考、审核结论参考 |
| `help/troubleshooting.mdx` | 常见问题排查 |

页面之间的导航结构定义在 [`docs.json`](docs.json)。

## 本地预览

安装 Mintlify CLI：

```bash
npm i -g mint
```

在仓库根目录（`docs.json` 所在目录）运行：

```bash
mint dev
```

在 `http://localhost:3000` 查看本地预览。

## 编写规范

- 所有页面使用简体中文，代码块、命令、字段名保持原样（不翻译标识符）。
- 涉及命令、配置字段或校验行为的内容，必须先对照 `sdlc-harness` 源码（`src/`、`templates/`）核实，不凭记忆或推测编写。
- 流程性内容优先用 Mermaid（`flowchart`、`sequenceDiagram`、`stateDiagram-v2`）而不是大段文字描述状态流转。
- 修改反映工具行为的页面后，运行一次 `sdlc-harness` 对应命令或读一遍相关源码，确认没有引入过时或虚构的字段。

## 发布

在 [Mintlify Dashboard](https://dashboard.mintlify.com) 安装 GitHub App 后，推送到默认分支会自动部署到生产环境。

## 相关链接

- [Mintlify 文档](https://mintlify.com/docs)
