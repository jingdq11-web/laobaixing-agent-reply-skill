# 老百姓 agent 回复 skill

这个 skill 给 Codex、Claude Code、DSH，以及其他认 Agent Skills 的 agent 用。同一份 `SKILL.md`，放进各自的 skills 目录即可。

工作做完、要总结时，agent 先给三个选项：

1. 通俗易懂
2. 完整表达（用于开发者）
3. 图标清楚显示

选 1：用大白话、带一点幽默把事情讲明白，再交一张验收卡。卡片只有四样：一句话结果、用户能看见的变化、用户自己怎么检查、明确没做的事。

选 2：按开发者要看的完整说明来写。

选 3：用图标把做成了什么、能看见什么、没做什么亮出来。

没有这三样以外的功能。

## 怎样交给自己的 agent

先拿到仓库里的 `SKILL.md`，放进一个名叫 `laobaixing-agent-reply` 的文件夹。下面路径里的 `~` 就是你的用户主目录。Windows 上多半是 `C:\Users\你的用户名`。

### Codex

```text
~/.codex/skills/laobaixing-agent-reply/SKILL.md
```

也可以对 Codex 说：用 skill-installer，从这个仓库安装 `laobaixing-agent-reply`。仓库地址：

https://github.com/jingdq11-web/laobaixing-agent-reply-skill

### Claude Code

个人常用，所有项目都能用：

```text
~/.claude/skills/laobaixing-agent-reply/SKILL.md
```

只给当前项目用：

```text
.claude/skills/laobaixing-agent-reply/SKILL.md
```

### DSH（DeepSeek Harness）

```text
~/.dsh/skills/laobaixing-agent-reply/SKILL.md
```

### 其他 agent

Gemini CLI、Cursor、Windsurf、GitHub Copilot，以及其他认 Agent Skills 的 agent，把同一个文件夹放进它自己的 skills 目录。名字保持 `laobaixing-agent-reply`，里面是这份 `SKILL.md`。

| Agent | 放置位置 |
| --- | --- |
| Gemini CLI | `~/.gemini/skills/laobaixing-agent-reply/SKILL.md` |
| Cursor | `~/.cursor/skills/laobaixing-agent-reply/SKILL.md` |
| Windsurf | `~/.codeium/windsurf/skills/laobaixing-agent-reply/SKILL.md` |
| GitHub Copilot | `~/.copilot/skills/laobaixing-agent-reply/SKILL.md`，或项目里的 `.github/skills/laobaixing-agent-reply/SKILL.md` |

放好后新开一轮对话。工作做完要总结时，直接说「用老百姓的方式总结」。agent 会先问你要 1、2 还是 3。
