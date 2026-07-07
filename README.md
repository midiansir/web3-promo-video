# Web3 Promo Video Skill

[中文说明](#中文说明) | [English Guide](#english-guide)

## 中文说明

`web3-promo-video` 是一个用于制作 Web3 项目品宣视频素材包的 Codex skill。

它适合把白皮书、项目叙事文档、代币机制说明、海报风格、品牌 VI、IP 角色和已有宣传素材，整理成可以继续放进 Seedance 2 这类图生视频工具里的制作包。

### 它能产出什么

- 30 秒、60 秒、90 秒或 120 秒的视频分镜结构
- 视频旁白台词
- 每个镜头的画面描述
- 每个镜头的 Seedance 2 视频提示词
- 每个镜头的 gpt-image-2 生图提示词
- 每个镜头对应的 16:9 横版分镜图
- 一张总览图，方便检查整条视频的视觉顺序
- 一个 Markdown 交付文档，包含时间轴、台词、分镜、提示词和检查项

### 适合什么场景

- Web3 项目上线前宣传片
- 代币叙事视频
- DeFi、GameFi、SportFi、SocialFi、RWA、AI + Web3 项目介绍视频
- 生态回流、协议飞轮、链上透明度、公示钱包、社区扩散等机制视频
- 品牌工作室或 Web3 服务品牌的获客视频

### 安装方式

把整个文件夹放到 Codex skills 目录：

```bash
~/.codex/skills/web3-promo-video
```

目录结构应类似这样：

```text
web3-promo-video/
├── SKILL.md
├── README.md
├── PROMOTION.md
├── agents/
│   └── openai.yaml
└── references/
    └── production-contract.md
```

### 怎么使用

在 Codex 里直接这样说：

```text
Use $web3-promo-video，把这个 Web3 项目的白皮书和海报风格，做成 90 秒宣传片分镜。需要视频台词、Seedance 2 提示词、每个镜头的 16:9 生图提示词，并生成每个镜头的图片。
```

也可以更具体：

```text
Use $web3-promo-video，参考 docs/whitepaper.md 和 assets/posters/，做一个 60 秒项目叙事视频。比例 16:9。每个镜头都要有台词、画面说明、Seedance 2 动态提示词和 gpt-image-2 生图提示词。
```

### 推荐输入

- 一份项目白皮书或叙事文档
- 一组海报、品牌 VI、官网截图或角色图
- 目标视频时长
- 画幅比例
- 是否需要直接生图
- 需要中文、英文，还是双语台词

### 工作流程

这个 skill 会先检查项目来源，再提炼视频叙事线。然后按时长拆成镜头，先写台词，再写分镜，再写 Seedance 2 提示词和生图提示词。需要生图时，会先生成第一张风格校准图，通过后再继续生成后续镜头。

默认 90 秒视频使用 12 个镜头，每个镜头约 7.5 秒。

### 风险边界

公开宣传内容只使用已确认的项目事实。不要把投资人、交易所、审计、TVL、用户量、收益承诺、合作方或上线计划写进视频，除非源文件已经明确确认。

## English Guide

`web3-promo-video` is a Codex skill for turning Web3 project materials into a promotional video production pack.

It is designed for whitepapers, narrative memos, token mechanics, poster styles, brand VI, mascots, product screenshots, and existing campaign assets. The output is ready for image-to-video tools such as Seedance 2.

### What It Produces

- Video structure for 30s, 60s, 90s, or 120s promos
- Voiceover script
- Shot-by-shot visual descriptions
- Seedance 2 prompt for every shot
- gpt-image-2 image prompt for every shot
- 16:9 storyboard frames when image generation is requested
- Contact sheet for visual review
- Markdown handoff document with timeline, voiceover, storyboard, prompts, and QA notes

### Best Use Cases

- Web3 launch videos
- Token narrative videos
- DeFi, GameFi, SportFi, SocialFi, RWA, and AI + Web3 product explainers
- Ecosystem return, protocol flywheel, transparent wallet, public ledger, and community-growth stories
- Client-acquisition videos for Web3 studios or service brands

### Installation

Place the folder under your Codex skills directory:

```bash
~/.codex/skills/web3-promo-video
```

Expected structure:

```text
web3-promo-video/
├── SKILL.md
├── README.md
├── PROMOTION.md
├── agents/
│   └── openai.yaml
└── references/
    └── production-contract.md
```

### How To Use

In Codex, ask:

```text
Use $web3-promo-video to turn this Web3 project whitepaper and poster style into a 90-second promo video storyboard. Include voiceover, Seedance 2 prompts, 16:9 image prompts for every shot, and generate the storyboard frames.
```

Or provide specific files:

```text
Use $web3-promo-video with docs/whitepaper.md and assets/posters/ to create a 60-second project narrative video. Use 16:9. Each shot needs voiceover, visual direction, Seedance 2 motion prompt, and gpt-image-2 image prompt.
```

### Recommended Inputs

- Whitepaper or narrative memo
- Poster set, brand VI, website screenshot, product UI, or mascot image
- Target duration
- Aspect ratio
- Whether frames should be generated
- Chinese, English, or bilingual voiceover preference

### Workflow

The skill checks the source material first, extracts one video narrative line, breaks it into timed shots, writes voiceover before visual prompts, then creates Seedance 2 prompts and image prompts. For larger batches, it generates the first frame as a style calibration frame before continuing.

The default 90-second structure uses 12 shots, around 7.5 seconds each.

### Safety Boundary

Public-facing videos should only use confirmed project facts. Do not add investors, exchanges, audits, TVL, active users, return promises, partnerships, or launch claims unless the source material explicitly confirms them.
