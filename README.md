# Agently Mail Skills

为 AI Agent 提供邮件操作能力的 Skill，支持登录授权、读取邮件、搜索邮件、发送邮件、回复、转发、移动到已删除、上传和下载附件。

更多指引访问官网地址：[agent.qq.com](https://agent.qq.com)。

## 安装

```bash
npx skills add Tencent/AgentlyMail -g
```

## 配置

使用前需要安装 CLI 并完成授权：

```bash
npm install -g @tencent-qqmail/agently-cli
agently-cli auth login
agently-cli +me
```

## 使用

安装后直接用自然语言与 Agent 对话即可：

```text
"帮我看看最近 10 封邮件"
"搜索标题里有周报的邮件"
"读取这封邮件的正文和附件"
"给 alice@example.com 发一封邮件"
"回复这封邮件，说明我今天晚点处理"
"把这封邮件转发给 bob@example.com"
"下载这封邮件里的附件"
```

## 功能

| 能力 | 说明 | 详细文档 |
|------|------|----------|
| 登录授权 | OAuth 登录、查看授权状态、登出 | [`SKILL.md`](skills/SKILL.md) |
| 当前用户 | 获取当前邮箱地址和 alias 列表 | [`SKILL.md`](skills/SKILL.md) |
| 邮件列表 | 按文件夹、时间、未读、附件条件列出邮件 | [`SKILL.md`](skills/SKILL.md) |
| 邮件读取 | 读取邮件正文、收件人、附件等完整信息 | [`SKILL.md`](skills/SKILL.md) |
| 邮件搜索 | 按关键词、发件人、收件人、时间、附件条件搜索 | [`SKILL.md`](skills/SKILL.md) |
| 写邮件 | 发送、回复、转发，支持附件和两阶段确认 | [`SKILL.md`](skills/SKILL.md) |
| 附件 | 上传和下载附件 | [`SKILL.md`](skills/SKILL.md) |

## 许可证

[Apache-2.0](./LICENSE) — Copyright © 2026 Tencent
