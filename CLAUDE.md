# 🍅 番茄钟 - Pomodoro Timer

一个简洁优雅的桌面番茄钟应用，帮助提升专注效率。

## 项目结构

```
CC_Project/
├── pomodoro.html          # 主应用（纯 HTML/CSS/JS 单文件）
├── .vscode/
│   ├── settings.json      # VS Code 工作区设置
│   ├── tasks.json         # 快捷任务
│   └── extensions.json    # 推荐扩展
└── CLAUDE.md              # 本文件
```

## 技术栈

- **纯前端** — 单个 HTML 文件，无依赖，开箱即用
- **数据存储** — `localStorage`（任务、设置、统计）
- **音频** — Web Audio API（完成提示音）
- **通知** — Web Notification API

## 运行方式

- 直接在浏览器打开 `pomodoro.html`
- 或用 Live Server 预览（VS Code 右下角 → "Go Live"）

## 功能模块

| 区域 | 说明 |
|------|------|
| 计时器 | SVG 环形进度条 + 倒计时显示 |
| 模式切换 | 专注 / 短休息 / 长休息 |
| 统计面板 | 今日番茄数、总计、专注时长、连续天数 |
| 任务列表 | 添加/完成/删除任务，关联番茄数 |
| 设置面板 | 自定义时长、自动开始等 |

## 键盘快捷键

- `Space` — 开始/暂停
- `R` — 重置
- `S` — 跳过当前阶段
- `1` / `2` / `3` — 切换到专注 / 短休息 / 长休息

## 代码规范

- 使用 2 空格缩进
- CSS 变量定义在设计系统 `:root` 中
- JavaScript 使用 vanilla JS，无框架
- 状态管理集中在 `state` 和 `settings` 对象中
