# 安装说明

本仓库只提供 `second-curve-opportunity-interviews`，与 `nextme-parallel-lives-cn`、`nextme-strength-finder-cn` 分别独立安装、更新和使用。

## 一句安装指令

README 按 Codex、Claude Code、Cursor、WorkBuddy 分别给出可复制给 Agent 的一句话和一行终端命令。根目录直接包含 `SKILL.md`，不需要进入其他 Skill 仓库或选择子目录。

前三者使用 Vercel Labs 的开源 Skills CLI，指定 `--skill second-curve-opportunity-interviews` 和对应 `-a`，`--copy` 安装完整文件副本。需要 Node.js、npm/npx、Git 和公开 GitHub 访问。`-g` 为当前用户跨项目安装；不加 `-g` 则只安装到当前项目。

WorkBuddy 使用 Git 克隆到 `~/.workbuddy/skills/second-curve-opportunity-interviews`；目前不把不存在的 `-a workbuddy` 参数写作受支持命令。Windows 用户可把 README 的自然语言发给 WorkBuddy，由其解析当前用户目录，不照抄 macOS / Linux 的 `$HOME` 命令。

## 完整上传包

- 通用包：[`dist/second-curve-opportunity-interviews.zip`](../dist/second-curve-opportunity-interviews.zip)
- SkillHub / WorkBuddy 上传包：[`dist/second-curve-opportunity-interviews-skillhub.zip`](../dist/second-curve-opportunity-interviews-skillhub.zip)
- 文件校验和：[`dist/SHA256SUMS`](../dist/SHA256SUMS)

两个 ZIP 内容相同：第一层为 `second-curve-opportunity-interviews/`，包含原始 v1.1.0 的全部 20 个文件。README 和本安装文档属于仓库分发说明；ZIP 保留已提交 SkillHub 的原始版本，不改动研究规则。Claude 网页版支持自定义 Skills 的账号需要手动上传 ZIP 并启用；普通聊天界面读取了链接不等于永久安装。

## 安装后检查

1. 确认目标目录内直接有 `SKILL.md`，不是又套了一层目录。
2. 确认 `name: second-curve-opportunity-interviews`、版本 `1.1.0`。
3. 确认 5 个 `references/` 文件、10 个 `assets/` 模板，以及示例与验收文件都在。
4. 新开对话或刷新技能列表，确认 Agent 能发现该名称；未发现时查看安装器显示的实际目录。
5. 用“请用 NextMe 机会探索型用户访谈 Skill 陪我设计一轮机会探索”启动。

安装器日志和文件完整性检查仅证明分发与落盘，不代替真实模型执行或学员试访验证。

## SkillHub 状态

独立页面：https://skillhub.cn/skills/user_ef208136/second-curve-opportunity-interviews 。审核状态以平台实时显示为准；未通过时可先用 GitHub 安装。不要因为基本介绍页存在，就宣称已上架或可下载。

## 依据

- [Skills CLI](https://github.com/vercel-labs/skills)：按 Agent 选择与全局安装参数。
- [支持的 Agent 与安装目录](https://github.com/vercel-labs/skills/blob/main/docs/agents.md)。
- [OpenAI Skills 说明](https://learn.chatgpt.com/docs/build-skills)：目录结构和发现机制。
- [SkillHub 安装说明](https://skillhub.cn/install/skillhub.md)：WorkBuddy skills 目录及安装源。
