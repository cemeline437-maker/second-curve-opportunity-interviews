# 第二曲线实验室｜机会探索型用户访谈 Skill

**版本**：1.1.0（2026-10-21；原 v1.0 包另行保留）  
**适用**：尚无明确产品、对用户研究不熟悉、手上只有初步商业想法或简略精益画布的学员；可研究副业、创业、改行、拓展新执业领域。

## 选择你的 Agent，一句安装

这是**独立 Skill、独立仓库**，不需要安装平行人生或优势发掘器。

| 你使用的工具 | 最短入口 |
| --- | --- |
| **ChatGPT 电脑客户端（Work）** | [复制 ChatGPT 一句安装指令](#chatgpt-电脑客户端work)；不用切到 Codex，不用上架官方插件目录 |
| **Claude 客户端 / 网页版** | [上传 ZIP 并启用](#claude-客户端--网页版)；**不需要 Claude Code** |
| Codex（可操作本地文件） | [复制 Codex 一句安装指令](#codex) |
| Claude Code | [复制 Claude Code 一句安装指令](#claude-code) |
| Cursor | [复制 Cursor 一句安装指令](#cursor) |
| WorkBuddy | [复制 WorkBuddy 一句安装指令](#workbuddy) |

下面的自然语言发给对应 Agent；命令行方式在终端执行。安装后新开对话或刷新技能列表。安装器完成不等于 Agent 已发现：需确认文件中的 `name` 为 `second-curve-opportunity-interviews`、版本为 `1.1.0`，再确认技能列表可见。

### ChatGPT 电脑客户端（Work）

**适合直接使用 ChatGPT 的学员，不要求会编程或使用 Codex。** 在 ChatGPT 电脑客户端，选择 ChatGPT，再把输入框上方的模式从 Chat 切换到 **Work**。安装需使用能访问本机文件的 Work 环境；只有云端容器、未连接这台电脑的环境不能替你完成本机安装。

复制这一句发给 ChatGPT（普通聊天里发送也会先得到切换提示）：

```text
请安装并使用 NextMe 机会探索型用户访谈 Skill，按 https://raw.githubusercontent.com/cemeline437-maker/second-curve-opportunity-interviews/main/docs/install-chatgpt.md 操作；如果当前是普通 Chat 聊天，或不能访问这台电脑的文件，请先提示我在 ChatGPT 电脑客户端切换到 Work 并使用可访问本机的环境，再重新发送本句，先不要开始访谈，也不要说安装成功。
```

Work 中实际使用的一行安装命令与 Codex 共用：

```bash
npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a codex --copy -y
```

`-a codex` 是第三方安装器的目标名称，安装的是电脑上的本地 Skill 文件，**不表示必须进入 Codex 界面**。接收方需核对实际安装目录；当前目标是用户的 `~/.agents/skills/second-curve-opportunity-interviews/`。安装后新开 Work 对话，在可用的 Skills 列表或 `@` 菜单中确认该 Skill 可见，再开始使用。只下载或落盘还不能宣称客户端已启用。

如果没看到 Work、Skills，或无法连接本机，请先更新客户端并检查账号/工作区是否开放该能力；不要把云端临时目录当作本机，也不要声称普通聊天发一句话就已永久安装。这个本地分发方式**不要求上架 ChatGPT 官方插件目录**。详见 [ChatGPT 安装与切换说明](docs/install-chatgpt.md)。

### Claude 客户端 / 网页版

**Claude 和 Claude Code 都可以用；Claude 客户端不需要安装 Claude Code，也不需要执行下面的 Claude Code 命令。**

1. [下载完整 Skill ZIP](https://github.com/cemeline437-maker/second-curve-opportunity-interviews/raw/main/dist/second-curve-opportunity-interviews.zip)。
2. 在 Claude 中打开 **Customize（自定义）→ Skills → ＋ → Create skill → Upload a skill**。
3. 上传 ZIP 并启用；在 Settings → Capabilities 中确保 **Code execution and file creation** 已开启。
4. 新开聊天，请 Claude 使用 `second-curve-opportunity-interviews`；先确认该 Skill 可用。

若桌面客户端没有该入口，可在同一账号的 Claude 网页版操作；团队账号可能需要管理员开放创建/上传权限。将 ZIP 发到普通聊天附件中不等于安装到 Skills。

也可以把这一句发给 Claude 客户端，让它协助引导：

```text
请帮我启用 NextMe 机会探索型用户访谈 Skill，安装包是 https://github.com/cemeline437-maker/second-curve-opportunity-interviews/raw/main/dist/second-curve-opportunity-interviews.zip；我使用 Claude 客户端，请引导我在 Customize → Skills 上传 ZIP 并启用，不要让我安装 Claude Code，也不要把普通聊天附件当成已安装。
```

### Codex

复制这一句发给 Codex：

```text
请从 https://github.com/cemeline437-maker/second-curve-opportunity-interviews 为当前用户安装 second-curve-opportunity-interviews Skill，执行 npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a codex --copy -y；已有同名 Skill 时先告诉我，不直接覆盖，完成后核对 name、1.1.0 版本和完整模板文件，并确认新对话中可发现再开始使用。
```

或一行终端命令：

```bash
npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a codex --copy -y
```

### Claude Code

复制这一句发给 Claude Code：

```text
请从 https://github.com/cemeline437-maker/second-curve-opportunity-interviews 为当前用户安装 second-curve-opportunity-interviews Skill，执行 npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a claude-code --copy -y；已有同名 Skill 时先告诉我，不直接覆盖，完成后核对 name、1.1.0 版本和完整模板文件，并确认新对话中可发现再开始使用。
```

或一行终端命令：

```bash
npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a claude-code --copy -y
```

### Cursor

复制这一句发给 Cursor Agent：

```text
请从 https://github.com/cemeline437-maker/second-curve-opportunity-interviews 为当前用户安装 second-curve-opportunity-interviews Skill，执行 npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a cursor --copy -y；已有同名 Skill 时先告诉我，不直接覆盖，完成后核对 name、1.1.0 版本和完整模板文件，并确认新对话中可发现再开始使用。
```

或一行终端命令：

```bash
npx --yes skills add https://github.com/cemeline437-maker/second-curve-opportunity-interviews --skill second-curve-opportunity-interviews -g -a cursor --copy -y
```

以上命令需要 Node.js、npm/npx 和 Git；`skills` 是第三方开源安装器。若电脑尚未安装依赖，让 Agent 先说明缺少什么。`-g` 表示当前用户可跨项目使用；只装当前项目时删去 `-g`。

### WorkBuddy

复制这一句发给 WorkBuddy（通过 GitHub 安装，不依赖 SkillHub 审核完成）：

```text
请从 https://github.com/cemeline437-maker/second-curve-opportunity-interviews 安装 second-curve-opportunity-interviews Skill 到当前用户的 ~/.workbuddy/skills/second-curve-opportunity-interviews，使用 Git 克隆完整仓库，已有同名目录时先告诉我，不直接覆盖；完成后核对 SKILL.md 的 name、1.1.0 版本及 references/、assets/ 文件，并提示刷新技能列表，确认可发现后再使用。
```

或一行终端命令（macOS / Linux；需要 Git，目标目录须不存在）：

```bash
git clone --depth 1 https://github.com/cemeline437-maker/second-curve-opportunity-interviews.git "$HOME/.workbuddy/skills/second-curve-opportunity-interviews"
```

也可到 [SkillHub 独立页面](https://skillhub.cn/skills/user_ef208136/second-curve-opportunity-interviews) 使用“安装到本地 Agent”；**须以页面实际审核状态为准**，审核中时不保证概述、下载或安装可用。

### 只有聊天、没有本地安装能力时

ChatGPT 普通 Chat 聊天请按上文提示切换到电脑客户端的 Work；Claude 客户端请在 Customize → Skills 上传 ZIP。两者的入口不同。不要把“读取仓库”或“普通聊天附件上传”称为已经安装。更多细节见 [安装说明](docs/installation.md)。

安装后开始用：

```text
请用已安装的 NextMe 机会探索型用户访谈 Skill，陪我从模糊想法设计一轮机会探索；如果当前是 ChatGPT 普通 Chat 聊天，请先提醒我切换到电脑客户端的 Work 并重新发送本句，不要先开始访谈；准备好后一次只问我一两个问题，目标明确后默认交付完整定制研究计划。
```

## 它做什么

它**不是**一个“输入赛道→吐出 20 个访谈问题”的提示词。它陪学员从模糊想法构建**研究任务卡**、区分证据与假设、选择可触达受访者、拟定三种招募文案、定制半结构机会探索提纲、做好现场记录、试访复盘，并在学员**先独立写出固定三点印象（与证据复盘不同）**后，利用获授权的材料进行证据综合，保留人机分歧，落地成一个最优先下一步。

**默认一对一；默认机会发现；默认一次问 1–2 个关键问题。** 研究共识形成后，**默认直接向学员交付完整定制研究任务卡与完整研究计划文档**；聊天只展示简短摘要和真实可用文档链接，不再要求学员另外提出“要完整版”。 仅学员明确选小组时才走小组分支。To B 时追**真实采购/评估/实施事件中的角色动作**，而非猜职位权力。

## 文件索引

```text
second-curve-opportunity-interviews/
├── SKILL.md                        # AI 的核心操作指令：必需
├── README.md                       # 人看的快速指南
├── references/
│   ├── 01-onboarding.md            # 教练式对话、决策澄清
│   ├── 02-sampling-b2b.md          # To C/To B 人群与角色图
│   ├── 03-fieldwork.md             # 访谈、试访、小组
│   ├── 04-analysis.md              # 先人后 AI，证据层级，综合
│   └── 05-method-sources.md        # NN/g、Buying Center 等来源
├── assets/
│   ├── 01-research-brief.md        # 研究任务卡
│   ├── 02-recruiting-copy.md       # 朋友圈 / 群聊 / 私信文案和筛选题
│   ├── 03-interview-guide.md       # 完整五要素半结构提纲
│   ├── 04-field-notes.md           # 现场记录表
│   ├── 05-first-impressions.md     # 学员独立记录三点
│   ├── 06-cross-interview-synthesis.md # 单场及跨场综合
│   ├── 07-change-log.md            # 试访后修订记录
│   ├── 08-b2b-event-map.md         # To B 事件角色表
│   ├── 09-complete-research-plan.md # 正式完整文档装配清单（必须）
│   └── 10-field-quick-card.md      # 可选现场一页导航（不替代完整计划）
├── examples/mini-walkthrough.md   # To C、To B、会后分歧示例
└── tests/acceptance-checks.md     # 基础场景 + 交付/复盘/压力验收
```

## 开始用

将**整个文件夹**放入支持 [Agent Skills 规范](https://agentskills.io/specification) 的 AI Agent 的 Skills 目录或通过其 Skill 上传入口导入；仅复制一个 `SKILL.md` 可以启动核心对话，但模型将无法按需读取其余模板文件。对具体平台，优先按照该平台当期 Skill 安装说明设置；Codex 的项目级 Skills 通常放在项目 `.agents/skills/` 下，而不是将 ZIP 当普通聊天附件便自动安装。

开始时可直接对模型说：

> “使用 `second-curve-opportunity-interviews` Skill，陪我从头设计一轮机会探索。我有个模糊的想法：[你的想法]。一次只问我一两个问题。等研究目标明确后，默认给我一份完整定制研究计划文档，聊天里只发摘要和文件入口。”

若已约到人，可说：

> “用这个 Skill，基于这张研究任务卡帮我选择访谈对象、做三种招募文案和访谈提纲。我访的是 [To C/To B]，目前能约到 [人物角色/相关经历]。”

访后可说：

> “我做完第一场了。请先提醒我独立记下三点印象，再按 Skill 区分我的判断、受访者证据与 AI 分析。不要改写我的原话。”

## 使用与数据边界

1. 招募时诚实说明研究目的；绝不装作试用、销售或活动。
2. 访谈开始单独确认录音/AI 处理的授权范围；不同意照常访谈，不上传不获许可的材料。
3. 若需使用曾做过的 Knowing Whom 人际网络盘点，**学员明确同意后**才查相关历史信息；没有能力读到时不能假装知道。
4. 小样本只探索问题与机制，不估计市场比例；每次结尾推荐一个下一步研究动作，不替学员做最终事业决定。

## v1.1 的正式交付规则

交付时应先按 `assets/09-complete-research-plan.md` **生成一份独立完整文档**：任务卡、访谁及样本偏差、三渠道招募、完整五要素半结构提纲（★必问/○机动）、现场记录、独立第一印象三点、试访复盘、后续证据分析模板、唯一下一步。**完整指针对当次主题的必要结构齐全，不是机械堆表格**。信息缺口保留待确认；没有访谈就不写“调研发现”。

聊天正文只给**近期决定、研究情境、优先访谁、最大未知、唯一下一步**与完整文档内容范围。必须确认文件确实生成并链接指向当前学员可访问的文件；不支持文件的环境应通过完整可复制文档交付，不可以只发摘要或说“已经放附件”但对方拿不到。若链接无效，立即换为完整文本等可靠形式。

## 新版修订依据与验证边界

v1.1 根据 2026-10-21 提交的模拟诊断交接单修订：重点处理完整交付缺失、范围收窄校验、独立三点/证据复盘混淆、工具锚定、首访继续判断和一回合追问演练。该交接来源为**一次 11 轮的同模型分上下文模拟**，不是已完成真人用户研究，也不能声称“全流程验证通过”。原 v1.0 内容保留为独立 ZIP。

## 后续迭代建议（不是当前已完成的实测）

带着 `tests/acceptance-checks.md` 的全部验收场景在目标 AI 模型里跑一遍，对照教学现场：学员是否觉得问题易懂、是否能自然讲出最近的事件、能否在第一场之后保住自己的判断。当前版本完成的是**文档结构与规则检查**，不是实际学员的用户测试结论。

## 方法参考

见 `references/05-method-sources.md`，包含 NN/g 用户访谈、访谈引导偏差、情境研究、定性分析与组织采购中心。工作流为面向初学者的实践整合，并非逐字转载。
