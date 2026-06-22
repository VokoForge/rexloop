<p align="center">
  <strong>Design the loop. Let agents run it.</strong><br>
  <strong>设计闭环，让Agent去跑。</strong>
</p>

<p align="center">
  <img src="https://img.shields.io/badge/License-MIT-green.svg" alt="License: MIT">
  <img src="https://img.shields.io/badge/Framework-M--LOOP-orange.svg" alt="M-LOOP Framework">
  <a href="https://github.com/VokoForge/rexloop/stargazers"><img src="https://img.shields.io/github/stars/VokoForge/rexloop?style=social" alt="GitHub stars"></a>
</p>

---

## RexLoop — M-LOOP Framework

**1 Rex Hub + 4 Feedback Loops + 7 Quality Gates**

*一个以Rex为中枢、以闭环为驱动的AI Agent执行框架。*

*An AI Agent execution framework driven by a Rex hub and closed-loop feedback.*

---

## 框架简介 / Framework Overview

RexLoop 是一个结构化的AI Agent执行框架，核心理念是：**将复杂的AI任务分解为可执行、可审核、可学习、可进化的闭环系统**。通过一个中枢调度器（Rex Hub）协调四条反馈闭环，并在关键节点设置质量门禁，确保Agent的输出始终可控、可追溯、可改进。

RexLoop is a structured AI Agent execution framework. Its core philosophy: **decompose complex AI tasks into executable, auditable, learnable, and evolvable closed-loop systems.** A central dispatcher (Rex Hub) coordinates four feedback loops, with quality gates at critical nodes to ensure Agent output is always controllable, traceable, and improvable.

---

## 核心架构 / Core Architecture

```
                          ┌─────────────────────────────┐
                          │         REX HUB             │
                          │    (Central Dispatcher)      │
                          └──────┬──────┬──────┬────────┘
                                 │      │      │
              ┌──────────────────┘      │      └──────────────────┐
              ▼                         ▼                         ▼
    ┌─────────────────┐     ┌─────────────────┐     ┌─────────────────┐
    │  EXECUTION LOOP  │     │  REVIEW LOOP     │     │  LEARNING LOOP  │
    │  执行闭环         │     │  审核闭环         │     │  学习闭环         │
    │  Execute → Check │     │  Review → Approve│    │  Learn → Adapt  │
    └────────┬────────┘     └────────┬────────┘     └────────┬────────┘
             │                       │                       │
             ▼                       ▼                       ▼
    ┌─────────────────────────────────────────────────────────────────┐
    │                    STRATEGIC LOOP / 战略闭环                      │
    │              Plan → Execute → Measure → Evolve                   │
    └─────────────────────────────────────────────────────────────────┘
                                 │
                                 ▼
    ┌─────────────────────────────────────────────────────────────────┐
    │              7 QUALITY GATES / 7个质量门禁                       │
    │  [G1] Input Validation    [G2] Plan Review                     │
    │  [G3] Execution Check     [G4] Output Verification             │
    │  [G5] Review Approval      [G6] Learning Validation             │
    │  [G7] Strategic Alignment                                          │
    └─────────────────────────────────────────────────────────────────┘
```

### 架构说明 / Architecture Breakdown

| 组件 / Component | 说明 / Description |
|-----------------|---------------------|
| **Rex Hub** (Rex 中枢) | 中央调度器，负责任务分发、闭环协调和质量门禁管理 |
| **Execution Loop** (执行闭环) | Execute → Check — 任务执行与即时校验 |
| **Review Loop** (审核闭环) | Review → Approve — 人工/AI审核与批准流程 |
| **Learning Loop** (学习闭环) | Learn → Adapt — 从历史执行中提取经验并调整策略 |
| **Strategic Loop** (战略闭环) | Plan → Execute → Measure → Evolve — 战略层面的PDCA循环 |
| **7 Quality Gates** (7个质量门禁) | 分布在各闭环关键节点的质量检查点 |

---

## 五大模块 / Five Core Modules

### 1. Automations (自动化循环)

自动化循环的设计与编排引擎，支持定时触发、事件驱动和链式执行。

*Design and orchestration engine for automation loops — supporting scheduled triggers, event-driven execution, and chained workflows.*

### 2. Worktrees (并行隔离)

基于工作树的并行任务隔离机制，每个Agent在独立的工作空间中执行任务，互不干扰。

*Tree-based parallel task isolation — each Agent operates in an independent workspace without interference.*

### 3. Skills (知识持久化)

将可复用的知识和能力封装为标准化技能模块，支持跨Agent共享和版本管理。

*Encapsulate reusable knowledge and capabilities as standardized skill modules — supporting cross-Agent sharing and version management.*

### 4. Plugins & Connectors (外部工具接入)

通过标准化插件接口接入外部工具和服务，扩展Agent的能力边界。

*Extend Agent capabilities through standardized plugin interfaces for external tools and services.*

### 5. Sub-agents & Memory (子代理与记忆系统)

层级式子代理架构配合多层级记忆系统，实现复杂任务的分解与上下文持久化。

*Hierarchical sub-agent architecture paired with multi-level memory systems for complex task decomposition and context persistence.*

---

## 快速开始 / Quick Start

```bash
# Clone the repository
git clone https://github.com/VokoForge/rexloop.git
cd rexloop

# Install dependencies
npm install  # or pip install -r requirements.txt

# Initialize your first Rex Hub
npx rexloop init

# Design your first loop
npx rexloop create --type execution --name "my-first-loop"

# Run it
npx rexloop run --loop my-first-loop
```

> **Note:** RexLoop is framework-agnostic. It works with any AI Agent runtime — OpenAI, Anthropic, local LLMs, or custom backends.

---

## Related Projects from VokoForge

| Project | Description |
|---------|-------------|
| [loop-engineering](https://github.com/VokoForge/loop-engineering) | Loop Engineering 橙皮书 — 从提示词到闭环工程方法论 |
| [managing-ai-agents](https://github.com/VokoForge/managing-ai-agents) | "给AI当老板" — 21章AI Agent团队搭建实战手册 |
| [ai-prism](https://github.com/VokoForge/ai-prism) | AI Prism — 多维视角下的AI工程实践 |
| [voko-skills](https://github.com/VokoForge/voko-skills) | AI Agent Skills Collection — 6大类技能模块 |

---

## License

This project is licensed under the [MIT License](LICENSE).

---

<p align="center">
  Built by <strong>VokoForge</strong> · Open Source · Community Driven
</p>
