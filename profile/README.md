<div align="center">

# ζ0Hub · ZetaZeroHub

**始于零，臻于极。**

*We create engaging AI-native products.*

[![Organization](https://img.shields.io/badge/GitHub-ZetaZeroHub-181717?logo=github)](https://github.com/ZetaZeroHub)
[![Website](https://img.shields.io/badge/官网-zzh.app-6366f1?logo=globe)](https://zzh.app)
[![GitHave](https://img.shields.io/badge/产品-GitHave-0ea5e9)](https://zzh.app/githave)
[![FlashMemory](https://img.shields.io/badge/产品-FlashMemory-f59e0b)](https://zzh.app/flash-memory)

</div>

---

## 摘要

**ZetaZeroHub**（ζ0Hub）是一个专注于 **AI 原生产品**研发的技术开源社区与组织。我们的愿景是：*Defining the Scale of Intelligence — From FlashMemory indexing to Zeta-scale inference.*

本组织目前已得到**亚信的企业经费赞助**，核心贡献成员不仅来自成电、兰交大、南邮、新国立等国内外高校，也包含了来自全球各地（德国、无锡、武汉、广东等）的卓越开源开发者。我们拥抱开源和 AI，鼓励大家通过 Vibe Coding 快速产出实用且富有创意的 AI Native MVP（最小可行产品）。若产品具增长潜力，组织将提供声量宣发、人员及经费支撑，共同在此平台生根发芽、共建生态！

---

## 目录

- [摘要](#摘要)
- [一期研发计划：AI 编程生态（灰度测试中）](#一期研发计划ai-编程生态灰度测试中)
- [社区共建与招募](#社区共建与招募)
- [组织产品线概览](#组织产品线概览)
- [仓库导航](#仓库导航)
  - [🌐 Web 门户层](#-web-门户层)
  - [🤖 AI 核心层](#-ai-核心层)
  - [🔧 后端服务层](#-后端服务层)
  - [📦 轻量级生态层](#-轻量级生态层)
  - [🗃️ 内部项目](#️-内部项目)
- [产品线架构](#产品线架构)
- [CookBook (代码烹饪书)](#cookbook-代码烹饪书)
- [相关链接](#相关链接)

---

## 一期研发计划：AI 编程生态（灰度测试中）

目前我们正在推进一条 **AI 编程主线产品（GitHave 与 FlashMemory）**，该产品线目前处于 0 宣发、0 推广的灰度测试阶段，暂未全量合并至当前组织主仓。我们的对标竞品包括：*Google CodeWiki, DeepWiki-Open, Context7, Zread.ai, Open Code, Cursor, Qoder* 等。

第一期研发计划主要围绕以下**四大核心子产品线**展开，旨在构建从底层基础设施到多端应用层的完整生态：

1. 🌐 **GitHave AI (Web 在线门户)**：线上流量入口与核心服务门户 ([githave.com](https://githave.com/home))。
2. 💻 **GitHave Pro (桌面端 App)**：面向企业私有化部署与高阶开发者定制的专业版工具。
3. 📦 **GitHave (跨端工具链)**：面向大众开发者的轻量级生态（含 App 客户端、VS Code 插件、Chrome 插件及 MCP/Skill 服务），实现多场景触达。
4. ⚡ **FlashMemory (终端底层引擎)**：支持去中心化部署的 AI 上下文索引基础设施。

---

## 社区共建与招募

我们正在建立开源社区交流群，聚集一群开发者小伙伴和早期产品体验用户：
- 💡 **参与产品打磨**：我们会在群里定期发布新的 AI Native 产品以及制定研发计划，欢迎测试用户提出体验问题及 Bug 反馈。
- 🚀 **Idea 到 MVP**：如果你有好的点子，欢迎通过 Vibe Coding 快速实现并申请合并到组织。
- 🤝 **推广共建**：如果你身边有信得过的开源同好，欢迎邀请加入，共同建设更繁荣的社区。

---

## 组织产品线概览

| 产品 / 方向 | 定位 | 访问地址 |
|:---|:---|:---|
| **GitHave** | AI 驱动代码仓库助手（在线平台版） | [zzh.app/githave](https://zzh.app/githave) |
| **GitHave Pro** | 开源专业版 AI 编程助手 | [GitHub](https://github.com/ZetaZeroHub/GitHavePro) |
| **FlashMemory** | 去中心化 AI 上下文索引引擎 | [zzh.app/flash-memory](https://zzh.app/flash-memory) |
| **Tech Report** | 技术洞察与行业报告 | [zzh.app/tech-report](https://zzh.app/tech-report) |
| **Official** | 官网 | [zzh.app](https://zzh.app) |

---

## 仓库导航

### 🌐 Web 门户层

#### [`githave-web`](https://github.com/ZetaZeroHub/githave-web) — GitHave Web 核心门户（Monorepo）

> GitHave 系列产品线 Web 门户的核心代码集合，采用 Monorepo 架构，包含网关、多个前端客户端及周边配套设施。

| 属性 | 信息 |
|:---|:---|
| 技术栈 | Go（网关）+ React/TypeScript（前端） |
| 架构 | Monorepo，含 `githave-gateway`（API 网关）+ 多端前端 |
| 核心能力 | JWT 认证、AI 对话代理、MCP/Tool 注册、Agent 编排、流式 SSE 输出 |

---

#### [`mlops-front`](https://github.com/ZetaZeroHub/mlops-front) — AI Chat 前端核心

> AI Chat Front Core — 涵盖从数据处理、模型训练、模型部署到算力运营、AI 应用等全链路功能的前端项目。

| 属性 | 信息 |
|:---|:---|
| 技术栈 | JavaScript / React + TypeScript + Arco Design |
| 核心功能 | 多会话管理、Agent 切换、MCP 编辑器、流式输出、Web 搜索、深度思考模式 |
| 端口 | 开发模式 `:8373` |

---

### 🤖 AI 核心层

#### [`FlashMemory`](https://github.com/ZetaZeroHub/FlashMemory) — 去中心化 AI 上下文索引引擎

> **全球首个去中心化分布式 AI 上下文索引引擎**，同时也是 GitHave 和 GitHave AI（在线门户）的索引服务后端。后期将独立运作，成为管理个人终端的本地知识库中枢。

| 属性 | 信息 |
|:---|:---|
| 定位 | 底层索引基础设施 + 个人知识库中枢 |
| 核心特性 | 去中心化分布式、上下文持久化、本地优先 |
| 产品页面 | [zzh.app/flash-memory](https://zzh.app/flash-memory) |

---

#### [`GitHavePro`](https://github.com/ZetaZeroHub/GitHavePro) — 开源 AI 编程助手（专业版）

> 原 [kinglegendzzh/GitHave](https://github.com/kinglegendzzh/GitHave)，已迁移至组织。开源的 AI 驱动代码仓库助手，"让 AI 帮您深度理解代码仓库，提供智能搜索、代码分析、文档生成等强大功能"。

| 属性 | 信息 |
|:---|:---|
| 开源状态 | ✅ 开源（Public） |
| 核心能力 | 智能仓库搜索、代码语义分析、文档生成 |

---

### 🔧 后端服务层

#### [`BotGo`](https://github.com/ZetaZeroHub/BotGo) — 智能代码助理（核心服务）

> GitHave 系列产品的后端核心服务，前身为亚信 OA 代码仓库监控助理，现演化为通用智能代码助理后端。

| 属性 | 信息 |
|:---|:---|
| 技术栈 | Go |
| Stars | ⭐ 1 |
| 角色 | GitHave 系列产品后端引擎 |

---

### 📦 轻量级生态层

#### [`githave-omini`](https://github.com/ZetaZeroHub/githave-omini) — GitHave 轻量级多端插件生态

> **GitHave-Omini（轻量级应用与多端插件生态）**：面向大众开发者，包含 App 客户端、VS Code 插件、Chrome 插件及 MCP/Skill 服务，实现多场景触达。

| 属性 | 信息 |
|:---|:---|
| 覆盖端 | Mobile App · VS Code Extension · Chrome Extension · MCP 服务 |
| 定位 | 轻量级生态，最大化触达场景 |

---

### 🗃️ 内部项目

#### [`cpcnc-pricing-repository`](https://github.com/ZetaZeroHub/cpcnc-pricing-repository) — 算力定价与 AI 知识库

> 内部项目，包含算力网络定价模型（Vue）及 `cfn_chatbot` RAG 知识库问答服务（Python + Langchain-Chatchat），支撑算力评估、意图识别、ChatBI 等能力。

| 属性 | 信息 |
|:---|:---|
| 技术栈 | Vue + Python |
| 核心模块 | `cfn_chatbot`（RAG + FastAPI，端口 `:7863`） |
| 知识库WebUI | 启动后访问 `http://127.0.0.1:8504` |

---

#### `README.md`（本仓库）

> ZetaZeroHub 组织综合看板，作为所有仓库和产品线的导航入口。

---

## 产品线架构

```
ZetaZeroHub 生态全景
━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━━

  用户 / 开发者
       │
       ├── 🌐  zzh.app            官方门户 & 产品展示
       │
       ├── 💻  githave-web        Web 前端 + API 网关（Monorepo）
       │         ├── githave-gateway   Go API 网关（认证/代理/Agent）
       │         └── 前端客户端 ...
       │
       ├── 📱  githave-omini      多端轻量级生态
       │         ├── App 客户端
       │         ├── VS Code 插件
       │         ├── Chrome 插件
       │         └── MCP / Skill 服务
       │
       ├── 🖥  mlops-front        AI Chat 全功能前端（独立部署）
       │
       ├── 🤖  BotGo              后端核心服务（Go）
       │
       ├── ⚡  FlashMemory        分布式 AI 上下文索引引擎
       │         └── → GitHave / GitHavePro 的索引服务
       │
       ├── 🛠  GitHavePro         开源 AI 编程助手（专业版）
       │
       └── 🗄  cpcnc-pricing      算力定价 + cfn_chatbot RAG 知识库
```

---

---

## CookBook (代码烹饪书)

为方便大家快速查阅详细的架构设计与部署指引，我们将包含从前端到核心底层模型的**端到端项目部署与联调指南**独立整理成了 CookBook：

👉 **[ZetaZeroHub CookBook (完整版看板与部署指南)](https://github.com/ZetaZeroHub/README.md)**

如果您是希望参与本组织生态共建或进行二次开发的开发者，强烈建议您阅读上述 CookBook，其中包含了：

- `githave-web` API网关与核心服务说明
- `mlops-front` AI Chat前端的全功能和多Agent配置指南
- `cfn_chatbot` RAG知识库和算力定价模型的完整推理运行手册

---

## 相关链接

| 资源 | 地址 |
|:---|:---|
| 🏠 官网首页 | [zzh.app](https://zzh.app) |
| 👤 关于我 | [zzh.app/me](https://zzh.app/me) |
| 🤖 GitHave 产品页 | [zzh.app/githave](https://zzh.app/githave) |
| ⚡ FlashMemory 产品页 | [zzh.app/flash-memory](https://zzh.app/flash-memory) |
| 📊 Tech Report | [zzh.app/tech-report](https://zzh.app/tech-report) |
| 🐙 GitHub 组织主页 | [github.com/ZetaZeroHub](https://github.com/ZetaZeroHub) |
| 📦 githave-web | [github.com/ZetaZeroHub/githave-web](https://github.com/ZetaZeroHub/githave-web) |
| 📦 githave-omini | [github.com/ZetaZeroHub/githave-omini](https://github.com/ZetaZeroHub/githave-omini) |
| 📦 BotGo | [github.com/ZetaZeroHub/BotGo](https://github.com/ZetaZeroHub/BotGo) |
| 📦 FlashMemory | [github.com/ZetaZeroHub/FlashMemory](https://github.com/ZetaZeroHub/FlashMemory) |
| 📦 GitHavePro | [github.com/ZetaZeroHub/GitHavePro](https://github.com/ZetaZeroHub/GitHavePro) |
| 📦 mlops-front | [github.com/ZetaZeroHub/mlops-front](https://github.com/ZetaZeroHub/mlops-front) |
| 📦 cpcnc-pricing-repository | [github.com/ZetaZeroHub/cpcnc-pricing-repository](https://github.com/ZetaZeroHub/cpcnc-pricing-repository) |

---

## 🤝 贡献指南

如果您希望参与本组织的生态共建，或者申请加入我们的核心贡献者行列，可以通过以下方式联系我们：

- 📧 **邮箱申请**：[kinglegendzzh@163.com](mailto:kinglegendzzh@163.com)
- 📺 **哔哩哔哩**：[@_章浩_](https://space.bilibili.com/39322300)
- 🌐 **官网联络**：[zzh.app/me#contact](https://zzh.app/me#contact)
- 💬 **微信联系**：`kinglegendchew` / `zhanghao_busi`
  
  <div align="center">
    <img src="./images/wechat1.jpeg" width="200" alt="微信二维码1"/>
    <img src="./images/wechat2.jpeg" width="200" alt="微信二维码2"/>
  </div>

---

## 🐛 反馈与支持

如果您在产品体验过程中遇到任何问题、Bug 或有功能建议，请随时提交 Issue：
👉 **[提交反馈](https://github.com/ZetaZeroHub/README.md/issues/new)**

---

<div align="center">

*ζ0Hub · 始于零，臻于极*

</div>
