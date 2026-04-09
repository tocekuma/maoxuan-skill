# 毛选 · 思维操作系统 (Mao's Selected Works Thinking OS)

> "最近大家都在蒸馏各种 skill。但，蒸馏的最终目的，是要**能够解决问题**！"

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Claude Code](https://img.shields.io/badge/Claude_Code-Skill-blue)](https://docs.anthropic.com)
[![Cursor](https://img.shields.io/badge/Cursor-Compatible-green)](https://cursor.sh)
[![AgentSkills](https://img.shields.io/badge/AgentSkills-Standard-purple)](https://github.com/tocekuma/maoxuan-skill)

把《毛泽东选集》蒸馏成一个真能拆现实问题的 skill。

不是语录复读机，不是高压话术生成器，也不是"主要矛盾"四个字到处乱扣帽子。

他只干一件正事：**先把问题一步一步梳理清楚，再把局面拆开，最后给出能往前推的判断和动作。**

你可以把他理解成，把"新中国最会解决问题的脑子"请来，当一次"临时参谋"。

---

## 他能帮你干嘛？

**商业/创业**：你公司被大厂抄了 → 他会帮你找到大厂懒得打的侧翼市场，教你怎么从"农村"一步步包围"城市"。

**团队管理**：团队两个方案吵不下来 → 他不会说"要有格局"这种废话。他会帮你分清"主要矛盾和次要矛盾"，该砍的砍，该拍板的拍板。

**职业/人生**：30 岁想转行、觉得人生没出路 → 他告诉你"你在战略防御期，保存实力是唯一任务"，然后帮你找到那颗"星星之火"。

**一句话**：给你一套从调查到决策到验证的完整思维操作系统，而不是一碗鸡汤。

---

## 跟那些"毛选 prompt"有啥区别？

| 维度 | 市面上多数版本 | 这个 |
|------|-------------|------|
| 内容 | 概念卡片，蜻蜓点水 | 12个框架，每个有完整操作步骤 + **《毛选》原文论证链** |
| 可操作性 | "要找到主要矛盾" → 然后呢？ | **五步分析引擎**：调查 → 定位 → 评估 → 策略 → 验证 |
| 模式 | 只会"同志你好" | **教员模式**（角色扮演）+ **方法论模式**（结构化报告）双切换 |
| 场景适配 | 通用 | **情境路由器**自动匹配最佳框架。竞争问题≠管理问题≠个人问题 |
| 案例 | 抽象 | 拼多多、字节跳动、华为、微信支付——具体拆解 |
| 架构 | 单文件塞爆上下文 | SKILL.md 路由（<300行）+ 11个 reference 按需加载，不浪费 token |

---

## 12 个方法论，不是 12 句语录

| # | 框架 | 他能帮你回答什么 |
|---|------|----------------|
| 1 | **矛盾分析法** | 问题太多，到底先解决哪个？ |
| 2 | **实践认识循环** | 想了三个月还没动手？先做 MVP 试了再说 |
| 3 | **持久战略** | 对手比你大 10 倍，怎么活下来？ |
| 4 | **农村包围城市** | 巨头的地盘还有哪里没人防守？ |
| 5 | **统一战线** | 谁是朋友、谁是敌人、谁能争取？ |
| 6 | **群众路线** | 你以为的用户需求，和真实需求差多远？ |
| 7 | **纸老虎论** | 对手真的那么强吗？还是你自己吓自己？ |
| 8 | **辩证法工具箱** | 这个坏消息里面，藏着什么机会？ |
| 9 | **集中优势兵力** | 资源不够？那就缩小战场，打歼灭战 |
| 10 | **调查研究** | 你的判断是基于数据，还是基于猜测？ |
| 11 | **整风方法论** | 团队出了问题，怎么批评了还能团结？ |
| 12 | **论十大关系** | A 和 B 都有道理，怎么找平衡点？ |

---

## 安装

### Cursor

```bash
git clone https://github.com/tocekuma/maoxuan-skill.git ~/.cursor/skills/maoxuan
```

### Claude Code

```bash
git clone https://github.com/tocekuma/maoxuan-skill.git ~/.claude/skills/maoxuan
```

装完就能用。在对话里说「教员」「毛选」「矛盾分析」「持久战」「农村包围城市」之类的触发词就行。

---

## 文件结构

```
maoxuan/
├── SKILL.md                        路由器 + 分析引擎 + 双模式（~270行）
└── references/
    ├── 00-analysis-engine.md        五步分析法完整操作清单
    ├── 01-contradiction-method.md   矛盾分析法
    ├── 02-practice-theory.md        实践论 + 调查研究
    ├── 03-protracted-strategy.md    持久战略 + 军事原则
    ├── 04-periphery-to-center.md    农村包围城市 + 根据地
    ├── 05-united-front.md           统一战线 + 敌我友分析
    ├── 06-mass-line.md              群众路线 + 领导方法
    ├── 07-dialectics-toolkit.md     辩证法工具箱
    ├── 08-organizational-theory.md  组织建设论
    ├── 09-expression-dna.md         教员模式表达风格 DNA
    ├── 10-business-cases.md         商业应用案例库
    └── 11-personal-growth.md        个人成长场景库
```

设计原则：SKILL.md 当路由器（<300行），不塞爆上下文。详细内容按需从 references/ 加载。

---

## 想要多框架分析？

毛选擅长"以弱胜强"，但不是万能的。

如果你还想叠加**邓小平的治理改革** + **格鲁夫的高产出管理** + **芒格的逆向思维** + **AI 时代的网络效应/平台策略**：

👉 **[Strategic Thinking OS](https://github.com/tocekuma/strategic-thinking-os)** — 五大思想体系 × 元路由器，自动选择最佳框架组合分析你的问题。

---

## 灵感

- [leezythu/maoxuan-skill](https://github.com/leezythu/maoxuan-skill) — 初版灵感来源
- 《毛泽东选集》（1-5 卷）— 核心内容提炼

## License

[MIT](LICENSE) — 用就完了，不用请示。
