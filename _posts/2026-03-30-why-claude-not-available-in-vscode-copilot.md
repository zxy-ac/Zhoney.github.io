---
title: '为什么在 VS Code Copilot 中无法使用 Claude 但可以使用 GPT 5.4？'
date: 2026-03-30
permalink: /posts/2026/03/why-claude-not-available-in-vscode-copilot/
tags:
  - GitHub Copilot
  - VS Code
  - Claude
  - AI
---

很多用户反映在 VS Code 的 GitHub Copilot 插件中可以使用 GPT 5.4，却无法使用 Claude 模型。本文解释其中的常见原因以及解决方法。

## 主要原因

### 1. 订阅套餐限制

Claude 模型（由 Anthropic 提供）在 GitHub Copilot 中的可用性取决于你的订阅套餐：

- **Copilot Free / Individual（个人版）**：仅提供部分模型，Claude 系列可能不在其中。
- **Copilot Business（商业版）** 或 **Copilot Enterprise（企业版）**：通常可以访问更多模型，包括 Claude。

如果你使用的是免费或个人版套餐，可以在 [GitHub Copilot 套餐页面](https://github.com/features/copilot) 确认你的套餐是否包含 Claude 模型访问权限。

### 2. 地区可用性

GitHub Copilot 的某些模型在特定地区尚未开放。Claude 模型可能在你所在的地区仍处于受限或未上线状态，而 GPT 系列模型覆盖的地区更广。

### 3. VS Code 插件版本过旧

较旧版本的 GitHub Copilot 插件可能不支持 Claude 模型。请确保将 VS Code 及 GitHub Copilot 插件更新到最新版本：

1. 打开 VS Code，进入 **Extensions（扩展）** 面板（`Ctrl+Shift+X` 或 `Cmd+Shift+X`）。
2. 搜索 **GitHub Copilot** 和 **GitHub Copilot Chat**。
3. 如果有可用更新，点击 **Update（更新）**。

### 4. 模型处于测试阶段（Beta）

某些 Claude 模型可能仍处于 Beta 测试阶段，需要手动启用或等待 GitHub 向你的账号开放。你可以在 GitHub 账号设置中检查是否有相关的功能预览（Feature Preview）开关。

## 如何检查并切换模型

在 VS Code 中切换 Copilot 使用的模型：

1. 打开 **GitHub Copilot Chat** 面板。
2. 点击模型选择器（通常显示当前使用的模型名称，位于输入框附近）。
3. 查看下拉列表中是否有 Claude 模型可选。

如果列表中没有 Claude，说明你当前的账号或套餐暂不支持该模型。

## 总结

| 原因 | 解决方法 |
|------|----------|
| 订阅套餐不包含 Claude | 升级到 Copilot Business/Enterprise |
| 地区限制 | 等待该地区开放，或关注 GitHub 官方公告 |
| 插件版本过旧 | 更新 VS Code 及 Copilot 插件 |
| 模型处于 Beta | 在账号设置中启用功能预览 |

如需了解最新的模型可用性信息，请参考 [GitHub Copilot 官方文档](https://docs.github.com/en/copilot/using-github-copilot/asking-github-copilot-questions-in-your-ide)。
