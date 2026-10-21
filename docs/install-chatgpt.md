# ChatGPT 电脑客户端：安装与开始使用

这是学员可复制给 ChatGPT 的安装流程。使用本地 Skill，不要求进入 Codex，也不要求上架官方插件目录。仓库独立提供 `second-curve-opportunity-interviews`。

## 先确认环境

- 如果当前是普通 Chat 聊天，先提示：“请在 ChatGPT 电脑客户端选择 ChatGPT，把输入框上方的 Chat 切换到 Work，使用能够访问这台电脑的环境，再把刚才那句安装指令发一次。”先不要开始研究访谈，不要声称已经安装。
- 如果无法确定当前是否为 Work，明确说明无法确认，先请学员按上述路径检查；不要凭模型名称推断。
- 即使当前有云端代码执行工具，也不等于能访问学员的电脑。只有在能读取并写入该电脑的用户目录时才继续；云端临时目录不能作为本机安装成功的证据。
- 如果不能打开本文件，复制 README 中的完整 ChatGPT 安装段落；无法读取时不要仅凭简介启动访谈。
- 如果账号没有 Work 或本机访问能力，说明当前条件不满足，让学员检查客户端更新和账号/工作区设置；不要声称切换一定能突破账号限制。

## 在可访问本机的 Work 中安装

1. 检查本机是否已有同名 Skill；已有时说明名称、路径与版本，不直接覆盖。先检查 `~/.agents/skills/second-curve-opportunity-interviews/`，并留意安装器实际报告的其他位置。
2. 使用完整公开仓库：`https://github.com/cemeline437-maker/second-curve-opportunity-interviews`。需要 Git、Node.js 和 npm/npx；缺少依赖时先说明具体缺口，不静默安装其他软件。
3. 在学员电脑上执行：

```bash
npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a codex --copy -y
```

`codex` 是安装器的目标名称；该命令把 Skill 放到本机用户的标准 Skills 目录，不要求学员切换到 Codex。按安装器实际输出定位文件，不把路径名称当作客户端发现的证据。

4. 核对 `SKILL.md` 的 `name` 为 `second-curve-opportunity-interviews`、版本为 `1.1.0`；检查 5 个 `references/` 文件、10 个 `assets/` 模板以及示例和验收文件均可读。研究规则与模板必须完整，不能只复制入口文件。
5. 准确区分状态：“文件已安装”与“ChatGPT 已发现并能调用”。提示学员新开 Work 对话，检查 Skills 列表或 `@` 菜单是否出现该名称；未出现时刷新或重启客户端并排查实际目录，不直接宣布启用成功。

## 开始使用

确认当前 Work 对话可以加载此 Skill 后，再读取完整 `SKILL.md` 并按其中的流程开始。入口问题每次最多 1–2 个；达到研究共识后默认交付完整定制研究计划，实际文件链接应能打开。不要因为换到 Work 就重新收集已经明确的信息。

若学员后来回到普通 Chat，在再次发送本说明或 README 的启动语句时仍先提示切换。**这是一段复制给 AI 的环境检查指令，不是客户端级拦截器，无法强制所有未加载它的聊天自动弹提示或自动切换模式。**

## 检查范围

安装器的落盘与文件完整性可以单独检查；ChatGPT 界面内的可发现、调用和完整文档交付需要在目标学员的 Work 环境中确认。不能把 Codex 中安装成功、云端可执行代码或文件已下载当作这些环节已经通过。

## 官方依据

- [ChatGPT 电脑客户端](https://learn.chatgpt.com/docs/app)：选择 ChatGPT，再在 Chat 与 Work 之间切换。
- [Build skills](https://learn.chatgpt.com/docs/build-skills)：电脑客户端支持独立 Skill；目录结构与调用方式。
- [Skills CLI](https://github.com/vercel-labs/skills)：本机安装器与 Agent 参数。
