# 贡献指南

感谢你愿意为 Handwriting-pulse 做出贡献！

## 报告问题

- 提交前请先搜索 [已有 Issue](https://github.com/lazytype666/Handwriting-pulse/issues)，避免重复。
- 使用仓库提供的 Issue 模板：
  - **Bug 报告**：描述问题、复现步骤、期望行为与环境信息。
  - **功能建议**：说明使用场景与期望效果。
- 请勿在 Issue 中粘贴密码、Token 等敏感信息。

## 提交代码

1. 从 `main` 创建功能分支，不要直接在主分支上开发：

   ```bash
   git checkout main
   git pull origin main
   git checkout -b feature/your-feature-name
   ```

2. 分支命名约定：

   | 前缀 | 用途 | 示例 |
   | --- | --- | --- |
   | `feature/` | 新功能 | `feature/export-pdf` |
   | `fix/` | 缺陷修复 | `fix/login-error` |
   | `docs/` | 文档修改 | `docs/update-readme` |
   | `refactor/` | 代码重构 | `refactor/cleanup-api` |

3. 提交信息请使用 [Conventional Commits](https://www.conventionalcommits.org/zh-hans/) 格式：

   ```
   <type>(<scope>): <subject>
   ```

   常用 type：`feat`、`fix`、`docs`、`style`、`refactor`、`test`、`chore`。

4. 推送分支并发起 Pull Request：

   ```bash
   git push -u origin feature/your-feature-name
   ```

## Pull Request 规范

- 填写 PR 模板中的检查清单。
- 一个 PR 只做一件事，避免混合无关改动。
- 提交前请自行测试，确保不破坏现有功能。
- 本仓库只允许 **Squash merge**，合并后源分支会自动删除。
- 合并后请删除本地已合并分支：

  ```bash
  git checkout main
  git pull origin main
  git branch -d feature/your-feature-name
  ```

## 代码风格

- 遵循项目现有的代码风格与目录结构。
- 不要提交构建产物、依赖目录或本地配置文件，相关规则见 `.gitignore`。

## 许可证

提交代码即表示你同意以本仓库的 [MIT 许可证](LICENSE) 授权你的贡献。
