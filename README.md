

> **开发者Anna QQ群: 1076321843**  
> **GitHub开源**：[https://github.com/crispvibe/windsurf-infinite-ask](https://github.com/crispvibe/windsurf-infinite-ask)

![License](https://img.shields.io/badge/license-MIT-blue.svg) ![Version](https://img.shields.io/badge/version-1.0.0-green.svg)
# WindsurfChat - Windsurf 无限对话插件

> 让 Windsurf AI 助手真正成为你的编程伙伴，突破单轮对话限制，实现无缝连续协作

## 为什么需要 WindsurfChat？

在使用 Windsurf 进行 AI 辅助编程时，你是否遇到过这些问题：

- AI 完成一个任务后就"结束对话"，需要手动开启新对话继续
- 有多个连续任务要做，却需要一个个手动输入
- AI 的回复被截断，无法继续之前的上下文
- 多个项目窗口切换时，对话状态混乱

**WindsurfChat 完美解决这些痛点！**

## 核心功能

### 1. 无限对话模式
通过 MCP 协议，AI 在每次回复结束时会**自动询问**是否继续。你可以：
- 一键继续，保持对话上下文
- 输入新指令，AI 立即执行
- 随时结束对话

### 2. 消息队列
预先规划多个任务，让 AI 按顺序自动执行：
- 支持最多 50 条消息排队
- 拖拽排序，灵活调整执行顺序
- 自动发送，无需手动干预
- 支持暂停/继续队列执行

### 3. 图片支持
直接向 AI 发送截图或设计稿：
- 支持拖拽上传
- 支持粘贴剪贴板图片
- 多图同时发送

### 4. 智能辅助
- **指令优化**：使用 AI 优化你的指令，让表达更精准
- **对话摘要**：自动生成对话摘要，方便回顾
- **历史记录**：保存对话历史，支持重发

### 5. 多窗口支持
每个 Windsurf 窗口独立工作，互不干扰：
- 基于工作区自动识别
- 独立的消息队列
- 独立的对话历史

## 使用效果

```
你: 帮我创建一个 React 登录页面
AI: [完成登录页面代码...]
    → 调用 windsurf_chat 询问是否继续

你: 继续，添加表单验证
AI: [添加验证逻辑...]
    → 调用 windsurf_chat 询问是否继续

你: 再加上记住密码功能
AI: [实现记住密码...]
    → 调用 windsurf_chat 询问是否继续

你: 完成，结束对话
AI: 好的，祝您编码愉快！
```

**整个过程无需开启新对话，上下文完整保留！**

## 技术实现

- **MCP 协议**：通过 Model Context Protocol 实现 AI 与插件的双向通信
- **VSCode Extension API**：深度集成 Windsurf/VSCode 编辑器
- **文件系统通信**：高效的进程间通信机制
- **安全验证**：设备绑定 + Token 验证，保障使用安全

## 系统要求

- Windsurf 编辑器（基于 VSCode）
- Node.js 16+
- macOS / Windows / Linux

## 获取方式

WindsurfChat 为付费插件，提供稳定的服务和持续的更新支持。

**购买链接**：[点击购买](https://pay.ldxp.cn/shop/windsurftool)

**使用教程**：[查看文档](https://www.yuque.com/anna-9fryq/am5iw9/nd9tv7q5axewbmbc)

**技术支持**：[加入 QQ 群](https://qm.qq.com/q/KN0vj0VhCK)

## 常见问题

### Q: 为什么需要 Node.js？
A: MCP Server 需要 Node.js 运行环境来处理 AI 与插件之间的通信。

### Q: 支持多少个设备？
A: 一个激活码绑定一台设备，支持换绑（需要原激活码）。

### Q: 如果 AI 没有调用 windsurf_chat 怎么办？
A: 确保已正确配置 MCP 和 .windsurfrules 规则文件，详见使用教程。

### Q: 支持 Cursor 吗？
A: 目前专为 Windsurf 设计，Cursor 暂不支持。

## 版本信息

**当前版本**：v3.0.8

## 免责声明

本插件为第三方工具，与 Windsurf/Codeium 官方无关。使用本插件即表示您同意自行承担使用风险。

---

**让 AI 编程更高效，从无限对话开始！**
