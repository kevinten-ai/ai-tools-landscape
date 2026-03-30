# Claude Code vs Cursor 深度对比

> 两大 AI 编程工具的全面对比分析

---

## 基本信息

| | Claude Code | Cursor |
|---|---|---|
| **开发商** | Anthropic | Anysphere |
| **类型** | CLI + VS Code 扩展 | AI 原生 IDE（VS Code fork） |
| **首发** | 2025年2月（预览），5月（GA） | 2023年 |
| **当前版本** | 持续发布（74次/52天） | v2.5 |
| **定价** | Claude Max $100-200/月 | Free / Pro $20 / Ultra $200 |
| **ARR** | $25亿+ | ~$20亿 |

---

## 核心能力对比

### 模型质量

| 指标 | Claude Code | Cursor |
|---|---|---|
| SWE-bench Verified | **80.9%**（Opus 4.5） | 依赖外部模型 |
| Token 效率 | 基准（1x） | 5.5x（完成同等任务） |
| 上下文窗口 | **1M tokens** | 取决于所选模型 |
| 自主编码时长 | **30+ 小时** | 依赖 Cloud Agent |

### 开发体验

| 能力 | Claude Code | Cursor |
|---|---|---|
| 终端操作 | **原生终端，极致效率** | 内置终端 |
| 可视化编辑 | VS Code 扩展（基础） | **原生 GUI，inline diff** |
| 自动补全 | 无独立补全 | **Supermaven Tab 补全极快** |
| 多文件编辑 | 命令行驱动 | **Composer 多文件可视化** |
| 代码审查 | Agent SDK 集成 | **BugBot 自动 PR 审查** |

### 自主代理

| 能力 | Claude Code | Cursor |
|---|---|---|
| 并行代理 | Agent Teams（研究预览） | **8个并行 Cloud Agents** |
| 远程执行 | Desktop/iOS/Android 远程控制 | **Cloud Agents 无需本地** |
| 定时任务 | **/loop 定时执行** | Automations 事件驱动 |
| 浏览器控制 | Chrome 扩展 | **内置 Browser for Agent** |

### 可扩展性

| 能力 | Claude Code | Cursor |
|---|---|---|
| MCP 支持 | 完整支持 | 完整支持 |
| Hooks | Pre/Post ToolUse + Stop | Beta |
| 自定义指令 | **Skills 动态加载** | Team Rules + Commands |
| SDK | **Claude Agent SDK** | — |

---

## 定价详解

### Claude Code

通过 Claude 订阅使用：
- **Pro**: $20/月（有限使用量）
- **Max (5x)**: $100/月
- **Max (20x)**: $200/月
- **API**: 按 token 计费（Opus $5/$25 per M）

### Cursor

- **Free**: 2,000 补全 + 50 慢速请求
- **Pro**: $20/月（500 快速请求）
- **Pro+**: $60/月
- **Ultra**: $200/月（20x 用量）
- **Business**: $40/用户/月
- 超额按信用额度计费

---

## 适用场景

### 选 Claude Code

- 复杂重构、跨文件大规模修改
- 终端重度用户
- 需要最高编码质量
- 自主长时间任务
- 构建 AI Agent 应用（SDK）

### 选 Cursor

- 日常代码编辑
- 需要快速 Tab 补全
- 可视化代码审查
- 前端 UI 开发（内置浏览器）
- 团队需要并行 Cloud Agent

### 最佳组合

> 重活用 CC，日常编辑用 Cursor，GitHub 工作流用 Copilot

---

## 参考资料

- [Claude Code vs Cursor - Builder.io](https://www.builder.io/blog/cursor-vs-claude-code)
- [Claude Code vs Cursor - Northflank](https://northflank.com/blog/claude-code-vs-cursor-comparison)
- [Claude Code vs Cursor - Emergent.sh](https://emergent.sh/learn/claude-code-vs-cursor)
