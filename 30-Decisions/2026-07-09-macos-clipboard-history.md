# macOS 剪贴板历史工具选择

## 日期

2026-07-09

## 背景

macOS 默认没有像 Windows `Win + V` 那样明显的剪贴板历史入口。需要一个轻量、可长期运行、支持键盘唤起和搜索历史记录的工具。

## 选项

- 方案 A：Maccy。开源、轻量，专注剪贴板历史，支持键盘搜索和菜单栏使用。
- 方案 B：Raycast Clipboard History。功能更综合，但依赖 Raycast 作为启动器和工作流中心。
- 方案 C：Paste。商业工具，界面完整，但不是当前最小必要方案。

## 决策

选择 Maccy 作为当前 macOS 剪贴板历史工具。

## 原因

- 与 Windows 剪贴板历史的核心需求最接近：保存历史、搜索、快速粘贴。
- 官方来源清晰：`https://maccy.app/` 和 `https://github.com/p0deje/Maccy`。
- 本机已存在 `/Applications/Maccy.app`，版本为 `2.6.1`，Bundle ID 为 `org.p0deje.Maccy`，已通过 `open -a Maccy` 启动。
- 启动后用系统事件确认 `Maccy` 进程存在。

## 影响

- 之后复制的新内容会进入 Maccy 的历史记录。
- 不在知识库中记录任何剪贴板具体内容，避免泄露私密信息。
- 如果自动粘贴或快捷键不可用，可能需要在 macOS 系统设置里给 Maccy 授予辅助功能权限。

## 后续行动

- [ ] 在 Maccy 偏好设置里确认快捷键和开机启动是否符合个人习惯。
- [ ] 如遇到粘贴失败，检查系统设置中的辅助功能权限。
