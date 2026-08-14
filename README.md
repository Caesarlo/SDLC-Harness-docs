# SDLC Harness 中文文档

这是 [SDLC Harness](https://github.com/Caesarlo/sdlc-harness) 的中文用户文档站点，面向使用该工具的开发者和编码 Agent 用户。站点使用 Mintlify 和 MDX。

## 内容范围

- 快速接入、生成文件和 Agent onboarding。
- 功能生命周期、验证、证据、评审和完成门禁。
- Solo/Team 协作、claim、租约和 Git worktree。
- 需求追溯、环境检查、会话收尾、CI/GitHub 和反馈闭环。
- 全量命令、配置、`feature_list.json`、审核结论和故障排查参考。

页面导航配置在 `docs.json`。用户文档使用简体中文；命令、路径、JSON 字段和字面状态值保持原始技术形式。

## 本地预览

安装 Mintlify CLI 后在本目录运行：

```bash
mint dev
```

或使用 npx：

```bash
npx mint dev
```

## 编写规范

- 遵循根目录 `AGENTS.md` 的术语和内容边界。
- 每个 `.mdx` 页面包含 YAML frontmatter。
- 示例优先使用可直接执行的 `npx @caesarlo/sdlc-harness ...`。
- 明确区分 `verify`、`validate`、`feature complete` 和 `provider github check`。
- 只记录当前 CLI 和仓库模板已经支持的用户行为。
- 新增、重命名或移动页面时同步更新 `docs.json`。

## 发布

合并到文档仓库的发布分支后，由现有 Mintlify 站点配置构建和发布。
