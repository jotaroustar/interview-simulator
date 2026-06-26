# 📝 AI 面试模拟器 (AI Interview Simulator)

> \*\*全行业岗位 · 多语种支持 · 智能打分 · 纯前端单文件\*\* > 
> 基于纯原生前端打造的沉浸式 AI 面试练习工具。支持\*\*内置经典题库\*\*与\*\*AI自由对话追问\*\*双模式，配备语音输入、AI朗读及深度复盘报告导出功能，助你零成本通关大厂面试。

[!\[HTML](https://img.shields.io/badge/HTML-单文件纯前端-orange?style=flat-square)](./index.html)
[!\[AI](https://img.shields.io/badge/AI-实时流式对话-green?style=flat-square)](https://jotarou.com)
[!\[License](https://img.shields.io/badge/Copyright-©2026\_jotarou.com-brown?style=flat-square)](#)

\---

## ✨ 核心特性

* **双练习模式切换**：

  * **📚 题库模式**：精选全岗经典真题，支持一键查看参考思路、草稿自动保存，并可调用 AI 针对你的回答进行犀利点评。
  * **🤖 AI 对话模式**：模拟真实面试官。引入 **STAR 法则**与多轮递进式深度追问，拒绝机械问答，带来拟真施压体验。
* **全球化语种与地区场景**：完美支持 🇨🇳 **纯中文**、🇺🇸 **全英文**（北美/外企）、🇯🇵 **全日文**（赴日 IT），以及高度还原真实外企环境的 🔤 **中英混杂**（外企黑话）模式。
* **全行业岗位兜底 \& 动态出题**：

  * 内置技术研发、产品设计、运营、数分、市场、HR等数十个核心岗位真题。
  * **支持自定义任意岗位**（如：*Web3游戏策划*、*医疗器械销售*）。若内置题目不足，AI 将基于 API 实时**动态生成全新面试题**。
* **多维度可视化评估报告**：对话结束后，AI 将从 **专业深度**、**逻辑思维**、**表达沟通**、**综合得分**四大维度进行量化打分，并附带多维度综合复盘评语。
* **无缝无感辅助工具**：

  * 🎙️ **语音输入**：基于 Web Speech API 实时识别，支持中/英/日多语种语音作答。
  * 🔊 **AI 朗读**：一键播报面试官文本，沉浸式还原听力面试环境。
  * 💾 **一键导出**：一键将面试题目、个人草稿、参考思路及 AI 点评导出为标准 Markdown 复盘报告。
* **极简且安全**：纯前端架构，数据绝不上传第三方服务器。内置 **localStorage 自动锁机制**，刷新页面可完美恢复上次未完成的面试进度，自动存档最近 20 条历史记录。

\---

## 🚀 快速使用

### 方式一：本地直接运行

1. 克隆或下载本仓库。
2. 确保以下三个文件处于同一目录下：

   * `index.html`（主程序）
   * `marked.min.js`（Markdown 渲染引擎）
   * `purify.min.js`（XSS 安全防护库）
3. 双击 `index.html` 即可在任意现代浏览器中完美运行。

### 方式二：在线体验

* **主站点**：[https://jotarou.com/tools/interview](https://jotarou.com/tools/interview)
* **备用镜像**：[https://jotaroustar.github.io/interview-simulator](https://jotaroustar.github.io/interview-simulator)

\---

## 🔑 模式与配置

|模式|API Key 依赖|核心功能|适用场景|
|-|:-:|-|-|
|**📚 题库模式**|**可选**|内置题库离线作答、查看参考答案。*（若需 AI 深度点评或自定义岗位则需要 Key）*|经典基础概念自测、面试速记背诵|
|**🤖 AI 对话模式**|**必填**|实时流式追问、动态提示/跳过、可视化四大维度综合打分报告|全真模拟面试、压力测试、临场表达训练|

### 🤖 支持的模型接入

系统默认支持并提供以下两款主流大模型的流式接入，兼容标准 OpenAI 接口：

* `gpt-4o-mini`：推理速度极快，响应敏捷，日常训练成本极低。
* `deepseek-chat`：国内顶尖大模型，中文及特定业务场景理解更为细腻。

> 💡 接口默认请求 BaseURL 为 `https://jotarou.com/v1`，支持无缝对接 \[Jotarou API](https://jotarou.com) 服务。

\---

## 📚 内置经典题库覆盖

**💻 技术研发岗：**

* **后端开发（通用/Go/C++）**：涵盖 HTTP/HTTPS 原理、B+ 树索引失效、死锁防御、Redis 三大高并发痛点、Kafka 高吞吐架构、大并发红包系统设计等。
* **Java 后端开发**：直击 JVM 运行时数据区、CMS/G1 垃圾回收区别、HashMap 线程不安全演验、Spring Boot 自动装配原理、线程池优化及 ThreadLocal 内存泄漏等。
* **前端开发**：包含浏览器 Event Loop、虚拟 DOM 树 Diff 算法、跨域 CORS、闭包及内存释放、前端性能全链路优化、TypeScript 泛型、微前端架构等。
* **大模型应用开发 (LLM/RAG)**：覆盖 RAG 核心架构、Prompt 幻觉抑制、LangChain/LlamaIndex 核心生态、Agent ReAct 自主规划、向量数据库 ANN/HNSW 索引等。
* **其他核心硬核岗位**：算法工程师（Transformer/XGBoost）、AI Infra（模型量化/PagedAttention/ZeRO三阶段/算子融合）、数据工程师（数据倾斜/Exactly-Once/数仓分层）、DBA/数据库、测试开发(QA)、移动端(iOS/Android)。

**📊 产品设计与运营岗：**

* **产品经理**：DAU 暴跌 30% 异常排查、Kano/RICE 需求优先级打分、MVP 闭包验证、研发工期博弈、B端与C端深度决策链差异。
* **运营**：AARRR 增长模型冷启动、大促活动全链路节奏拆解、社群活跃度度量、用户流失预警机制。
* **数据分析**：连续 3 天登录 SQL 留存算法、A/B 测试辛普森悖论漏斗陷阱、极高流失率向下钻取。
* **全链路协同岗位**：市场营销、商务拓展 (BD 评估矩阵)、UI/UX 设计 (Design System)、HR/行政、销售/大客户。

\---

## 📁 项目文件结构

.

├── index.html        # 主程序文件 (集成古典雅致的微醺棕皮肤 UI)

├── marked.min.js     # 本地化 Markdown 解析库

└── purify.min.js     # 本地化 XSS 攻击防护库

\---



<p align="center">

&#x20; Made with ❤️ by <a href="https://github.com/jotaroustar">jotaroustar</a>

</p>



<p align="center" style="font-size: 11px; color: #7a6550;">

&#x20; Copyright © 2026 jotarou.com. All rights reserved.<br>

&#x20; 未经授权许可，禁止直接复制本系统源码用于任何形式的商业产品或盈利性服务。

</p>

