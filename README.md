# yourlanguage

**作者 / Author:** 魏珏然 (Mellow Wei)
**状态 / Status:** v2.0 — active development
**节点 / Node:** mellowwei.github.io/yourlanguage/

---

## 这是什么

yourlanguage 是一个语言教育体验网站。

它不教你关于语言的知识。
它让你经历语言正在对你做的事。

核心理论框架来自魏珏然原创的**四行为结构**：

```
命名行为 (naming)
    ↓
加压行为 (pressurizing)
    ↓
滑义行为 (meaning-sliding)
    ↓
相变行为 (phase transition)
```

道德语言不是谎言。
它是选择了携带方向的词，一步一步，带你到它想去的地方。

---

## 文件结构

```
yourlanguage/
├── index.html              ← 主体验 (yourlanguage.html)
├── game.html               ← 语言游戏 (yourlanguage-game.html)
└── README.md               ← 本文件
```

---

## 两个模块

### `index.html` — 主体验

访客以为在读一个关于语言的网站。
网站本身的语言正在对他们做命名→加压→滑义→相变。
揭示发生在过程中，不是结尾。

**四语路径，四种元语言机制：**

| 语言 | 元语言类型 | 颜色 | 伤口 |
|------|-----------|------|------|
| English | 命名元语言 | `#c8b89a` | 命名即占有现实。谁命名，谁拥有随之而来的现实。 |
| 中文 | 非线性元语言 | `#4a9eff` | 说了等于没说。但你感到被说了。非线性允许意义永远不落地，逃逸结构可以成为永不负责的通道。 |
| 日本語 | 省略元言語 | `#e8c547` | 言われなかったことが届く。省略は沈黙を語らせる。強制された沈黙と選ばれた沈黙は区別できない。 |
| Deutsch | 垂直压缩元语言 | `#b44fff` | Sprache spricht. Nicht du. je präziser die Analyse, desto schärfer die Waffe. 分析能力与它的历史伤口同时在场。 |

**隐藏第五层：**
访客走完全部四条路径后解锁。
内容：这个框架本身是一个命名行为。yourlanguage从来都不是你的。这个洞见也不是。

**交互机制（B型实时揭示）：**
- 悬停下划线词 → 底层注释浮出
- 点击词 → 全屏打断，底层接管表层
- 第四屏 → 页面分裂为表层/底层两列，悬停触发对应注释点亮
- 第五屏 → 底层视觉淹没表层，相变在页面上发生
- 第七屏 → 用户输入任意文本，AI用四行为结构实时拆解

---

### `game.html` — 语言游戏

Wittgenstein意义上的语言游戏：
每个关卡是一个规则系统。
进入就接受规则。
但规则是语言做的。
做游戏就是在执行语言规则。

**五关：**

```
关卡一 — 命名游戏
规则：给三个图形命名。任何名字。
揭示：你命名的不是图形。是你对它们的权力关系。
to name is not to point. to name is to claim.

关卡二 — 遵从游戏
规则：按顺序点击五条指令。
揭示：你从未问过这些指令的权威来自哪里。形式即权威。
obeying is understanding, not interpreting.

关卡三 — 描述游戏
规则：用一句话描述你看到的图像。
揭示：五个人对同一张图写出五种不同的现实。
description produces, not records.

关卡四 — 翻译游戏
规则：改写一句话三次，保持意义完全不变。
揭示：任务不可能完成。每次改写都产生意义偏移。AI实时分析。
meaning cannot survive transfer unchanged.

关卡五 — 规则游戏
规则：找出这个游戏的规则。
揭示：开始寻找的那一刻就已经在执行规则了。
there is no position outside the game from which to observe the game.
```

**结尾第五层：**
与主体验共享同一个底层命题——
这个框架本身是一个语言游戏。
yourlanguage was never yours.
Neither is this insight.

---

## 技术说明

**依赖：**
- Google Fonts: EB Garamond, Space Mono, Noto Serif SC, Noto Serif JP
- Anthropic API (`claude-sonnet-4-20250514`) — 用于关卡四翻译分析、关卡五规则响应、主体验第七屏文本拆解
- 无其他外部依赖，无框架

**API调用位置：**
```
主体验 → 第七屏用户输入分析
游戏   → 关卡四翻译偏移分析
游戏   → 关卡五规则响应
```

**System prompt核心（三处共享）：**
```
四行为结构拆解：
命名行为 → 加压行为 → 滑义行为 → 相变行为
精准、冷静、不做道德判断
只描述机制
```

**部署：**
```
GitHub Pages
mellowwei.github.io/yourlanguage/
├── index.html
├── game.html
└── README.md
```

主站节点链接：mellowwei.github.io/MellowWei/

---

## 理论来源

**四行为结构** — 魏珏然原创语言逻辑分析框架

**引用背景：**
- Wittgenstein, *Philosophische Untersuchungen* (1953) — 语言游戏，规则遵从
- Wittgenstein, *Tractatus Logico-Philosophicus* (1921) — "The limits of my language mean the limits of my world." (5.6)
- Klemperer, *LTI — Lingua Tertii Imperii* (1947) — 纳粹语言工程作为四行为结构的历史案例
- Heidegger, "Die Sprache" (1950) — *Sprache spricht* (语言在说话，不是人在说话)

**德语元语言的历史伤口：**
德语的垂直压缩元语言特质（Bedeutungsverschiebung、Volksgemeinschaft、Entartung）曾被纳粹语言工程精密利用。分析能力与被分析的历史同时在场。这不是背景信息，这是德语路径的核心设计参数。

---

## 设计原则

**B型实时揭示：**
揭示不在结尾。揭示发生在过程中。
底层注释在表层叙事进行时浮出，打断，然后还给表层继续。

**D型语言路径差异：**
表面是可切换的四语版本。
但每种语言版本里有其他版本没有的隐藏内容。
访客以为在选语言，实际上在选自己被操作的方式。

**第五层原则：**
任何关于语言操作的框架，本身都是一次语言操作。
yourlanguage不揭示这个矛盾然后解决它。
它揭示它，然后让它悬在那里。

---

*yourlanguage — 魏珏然 — 2026*
