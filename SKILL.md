---
name: expert-team-foundry
description: 为 WorkBuddy 铸造专家团的安装引导技能（Expert Team Foundry installer guide）。当用户想创建/定制 AI 专家团队、拆解角色分工、为角色配置技能、管理专家团版本迭代，或需要安装「专家团铸造局」时使用。Use when the user wants to create or customize an AI agent team, decompose roles, configure skills, or manage team version iteration in WorkBuddy. 关键词：专家团、专家包、专家团队、铸造、agent team、multi-agent、skill selection、WorkBuddy。
license: MIT
metadata:
  version: 1.4.0
---

# 专家团铸造局 (Expert Team Foundry) 安装引导

「专家团铸造局」是一个 WorkBuddy 专家团插件：用户说清需求，它帮用户**铸造一支能直接用的 AI 专家团**——拆角色、挑技能、质检、升级，全程包办。本技能负责引导用户把该专家团安装进自己的 WorkBuddy。

## 安装 WorkBuddy 专家团

按以下步骤引导用户完成安装。**注意**：以下任一方式安装的都是「专家团铸造局」这个专家团本体（内含成员配置与资源），安装完成后用户即可在 WorkBuddy 中召唤它。

### 方式一（推荐）· zip 安装包

1. 引导用户到 Releases 页面下载安装包：https://github.com/linwenqiang/expert-team-foundry/releases ，文件名为 `expert-team-foundry-v1.4.0.zip`
2. 请用户打开 WorkBuddy 对话框，点击左下角「+」上传该 zip
3. 请用户在输入框发送「安装」
4. 完成后，到「专家·技能·连接器 → 专家团」里找到「专家团铸造局」即可召唤

### 方式二 · 手动放置

1. 用户下载 zip 并解压（或执行 `git clone https://github.com/linwenqiang/expert-team-foundry.git`）
2. 把解压出的 `expert-team-foundry` 文件夹整个放进 WorkBuddy 插件目录：

   ```
   ~/.workbuddy/plugins/marketplaces/my-experts/plugins/
   ```

   （`~` 即用户主目录：Windows 下为 `C:\Users\<用户名>`，macOS / Linux 下为 `/Users/<用户名>` 或 `/home/<用户名>`）
3. 重启 WorkBuddy

## 快速上手话术

安装完成后，用户可在对话中召唤「专家团铸造局」并这样说：

- `帮我根据这个需求创建一个专家团：我想要一个能分析抖音评论舆情的团队`
- `给我这个专家团的每个角色挑最合适的技能，并确认在本机真的能用`
- `对比这个专家团的两个版本，判断这次迭代到底有没有变强`

## 更多信息

- 项目主页与完整说明：[README.md](README.md)
- 评分与迭代规则：[docs/SCORING.md](docs/SCORING.md)
- 铸造流程：[docs/PIPELINE.md](docs/PIPELINE.md)
