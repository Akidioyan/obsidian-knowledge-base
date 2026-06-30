# Codex 协作流程

## 什么时候用

当你希望 Codex 帮你整理 Obsidian vault、生成项目笔记、改写 Markdown、补充任务清单、沉淀决策或批量调整结构时，用这套流程。

## 标准流程

1. 在 `10-Projects/` 或 `20-Specs/` 写清楚目标、背景、限制和完成标准。
2. 让 Codex 读取那篇笔记，并明确说明不能删除旧笔记。
3. Codex 先给计划，再执行修改。
4. 修改完成后，Codex 把过程摘要写入 `80-Agent-Logs/YYYY-MM-DD.md`。
5. 你用 Git 查看差异，确认后提交。

## 推荐提示词

```text
读取 10-Projects/某项目.md。
根据里面的目标整理相关笔记和任务。
不要删除旧笔记。
重要决策写入 30-Decisions/。
完成后把总结追加到 80-Agent-Logs/YYYY-MM-DD.md。
最后告诉我改了哪些文件。
```

## Git 检查

```bash
git status
git diff
git add .
git commit -m "Update vault notes"
```

## 安全规则

- 大批量修改前先让 Codex 列计划。
- 不要让 Codex 直接删除私人笔记。
- 重要修改先看 Git diff。
- API key、token、账号信息不要写进普通笔记。
