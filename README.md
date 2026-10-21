# 老百姓 agent 回复 skill

这个 skill 给不懂代码的人用。

agent 做完任务后，不许讲技术，必须交一张验收卡。卡片上只有四样东西：

1. 一句话结果
2. 用户能看见的变化
3. 用户自己怎么检查
4. 明确没做的事

没有别的功能。

## 别人怎样交给自己的 agent 用

把本仓库里的 `SKILL.md` 放进你的 agent 读取 skill 的目录，目录名用 `laobaixing-agent-reply`。

Claude Code 用这个目录：

```text
~/.claude/skills/laobaixing-agent-reply/SKILL.md
```

放好后新开一轮对话。你说「我不懂代码，做完用老百姓的方式回复」，agent 就会按这张验收卡答复。

其他支持 Agent Skills 的 agent，把同一个 `SKILL.md` 放进它自己的 skills 目录，目录名同样用 `laobaixing-agent-reply`。