# AI 面试模拟器

> 全岗位 AI 面试练习工具，支持题库模式和 AI 对话模式，语音输入，智能打分，导出复盘报告。

![license MIT](https://img.shields.io/badge/license-MIT-blue)
![HTML](https://img.shields.io/badge/HTML-单文件-orange)
![AI](https://img.shields.io/badge/AI-实时对话-green)

---

## ✨ 功能特性

- **多岗位覆盖**：技术岗（后端/Java后端/前端/算法/AI Infra/数据工程/大模型应用/测试/移动端/DBA）+ 产品运营岗（产品经理/运营/数据分析/市场营销/UI设计/HR/销售）
- **自定义岗位**：输入任意岗位名称，AI 动态生成对应面试题
- **多面试轮次**：初试/技术一面/技术二面/HR面/终面等场景
- **多语种支持**：中文/全英文（北美外企）/全日文（赴日IT）/中英混杂
- **题库模式（免费）**：逐题作答，查看参考思路，支持 AI 点评回答
- **AI 对话模式**：模拟真实面试官，根据回答实时追问，结束后综合打分
- **语音输入**：支持麦克风语音作答，无需手动输入
- **AI 朗读**：面试官问题支持语音播报
- **Markdown 渲染**：AI 回答支持代码块、列表、加粗等格式
- **导出复盘报告**：面试结束后导出 .md 文件，包含题目、回答、参考答案、AI 点评
- **会话恢复**：刷新页面可恢复上次未完成的面试进度
- **历史记录**：自动保存最近 20 条面试记录

---

## 🚀 快速使用

### 方式一：直接下载使用

下载以下三个文件放在同一目录，用浏览器打开 `index.html` 即可：
- `index.html`
- `marked.min.js`
- `purify.min.js`

### 方式二：在线体验

- 主地址：https://jotarou.com/tools/interview
- 备用地址：https://jotaroustar.github.io/interview-simulator

---

## 🔑 两种使用模式

**【题库模式 · 免费】** 不需要 API Key，内置题库直接开始练习，可查看参考答案。

**【AI 对话模式 · 需 Key】** 填入 API Key，解锁 AI 面试官实时对话、追问、综合打分全部功能。

---

## 🤖 支持的模型

| 模型 | 说明 |
|------|------|
| gpt-4o-mini | 速度快，成本低，日常推荐 |
| deepseek-chat | 国内模型，中文理解好 |

支持自定义 BaseURL，可接入任意 OpenAI 兼容接口（包括 [Jotarou API](https://jotarou.com)）。

---

## 📚 题库覆盖岗位

**技术岗：**

| 岗位 | 题目数 |
|------|--------|
| 后端开发（通用/Go/C++） | 8 题 |
| Java 后端开发 | 8 题 |
| 前端开发 | 10 题 |
| 大模型应用开发 | 6 题 |
| 算法工程师 | 8 题 |
| AI Infra | 8 题 |
| 数据工程师 | 8 题 |
| DBA/数据库 | 4 题 |
| 测试开发(QA) | 8 题 |
| 移动端(iOS/Android) | 4 题 |

**产品运营岗：**

| 岗位 | 题目数 |
|------|--------|
| 产品经理 | 8 题 |
| 运营 | 6 题 |
| 数据分析 | 6 题 |
| 市场营销 | 1 题 |
| UI/UX 设计 | 1 题 |
| HR/行政 | 1 题 |
| 销售/大客户 | 1 题 |

---

## 🛠️ 技术栈

- 纯 HTML + CSS + JavaScript，本地化依赖（marked.js + DOMPurify）
- 调用 OpenAI 兼容接口，支持流式输出
- Web Speech API 语音输入/朗读
- localStorage 会话恢复与历史存储

---

## 📁 文件结构

```
.
├── index.html        # 主文件
├── marked.min.js     # Markdown 渲染库（本地化）
└── purify.min.js     # XSS 防护库（本地化）
```

---

## 📄 License

MIT License · 自由使用、修改、分发

---

## 🔗 相关项目

| 项目 | 说明 |
|------|------|
| [快递单号提取器](https://github.com/jotaroustar/express-number-extractor) | 批量提取快递单号，支持截图 AI 识别 |
| [简历优化器](https://github.com/jotaroustar/resume-optimizer) | 简历规则检查 / AI 改写 / JD 匹配 / 面试预测 |
| [日报周报生成器](https://github.com/jotaroustar/report-generator) | 日报周报一键生成，支持 AI 润色扩写 |
| [文案生成器](https://github.com/jotaroustar/copywriter-generator) | 朋友圈/社交媒体文案生成，支持多平台多风格 |
| [Jotarou API](https://jotarou.com) | AI API 中转服务，支持 Claude / GPT / DeepSeek |

---

<p align="center">
  Made with ❤️ by <a href="https://github.com/jotaroustar">jotaroustar</a>
</p>
