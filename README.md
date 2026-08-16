# SDLC Harness 文档

这是 [SDLC Harness](https://github.com/Caesarlo/sdlc-harness) 的双语用户文档仓库，面向使用该工具的开发者和编码 Agent 用户。站点使用 Mintlify 和 MDX，默认语言为英文，简体中文页面位于 `/zh/` 路径下。

## 内容范围

- 快速接入、生成文件和 Agent onboarding。
- 功能生命周期、验证、证据、评审和完成门禁。
- Solo/Team 协作、claim、租约和 Git worktree。
- 需求追溯、环境检查、会话收尾、CI/GitHub 和反馈闭环。
- 全量命令、配置、`feature_list.json`、审核结论和故障排查参考。

页面导航配置在 `docs.json`。英文页面位于仓库根目录，对应的简体中文页面位于 `zh/`。命令、路径、JSON 字段和字面状态值保持原始技术形式。

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
- 英文页面作为默认版本放在根目录，简体中文译文放在 `zh/` 的对应路径。
- 新增或修改页面时，保持英文和简体中文内容及导航结构同步。
- 示例优先使用可直接执行的 `npx @caesarlo/sdlc-harness ...`。
- 明确区分 `verify`、`validate`、`feature complete` 和 `provider github check`。
- 只记录当前 CLI 和仓库模板已经支持的用户行为。
- 新增、重命名或移动页面时同步更新 `docs.json`。

## 发布

合并到文档仓库的发布分支后，由现有 Mintlify 站点配置构建和发布。根路径发布默认英文站点，`/zh/` 发布简体中文站点；发布前应确认两种语言的页面清单一致且链接有效。
