# Web3 Promo Video Skill Promotion

[中文宣传](#中文宣传) | [English Promo](#english-promo)

## 中文宣传

### 一句话介绍

把 Web3 项目白皮书、海报风格和品牌资产，直接整理成 90 秒宣传片分镜、生图提示词和 Seedance 2 镜头提示词。

### 短介绍

`web3-promo-video` 是一个面向 Web3 品宣视频制作的 Codex skill。它会先读取项目白皮书、叙事文档、海报风格和品牌素材，再把项目机制整理成视频叙事线，输出台词、分镜、Seedance 2 动态提示词和每个镜头的 gpt-image-2 生图提示词。

适合项目上线前宣传片、代币叙事视频、生态飞轮解释、链上透明度展示、社区扩散内容和 Web3 服务品牌获客视频。

### GitHub 仓库简介

```text
Codex skill for creating Web3 promotional video production packs: storyboard, voiceover, Seedance 2 prompts, gpt-image-2 prompts, and 16:9 generated frames.
```

### 中文发布帖

```text
我整理了一个 Web3 品宣视频制作 skill：web3-promo-video。

它可以把项目白皮书、叙事文档、海报风格、品牌 VI 和角色素材，整理成完整的视频制作包：

1. 视频时间轴
2. 旁白台词
3. 分镜表
4. Seedance 2 镜头提示词
5. gpt-image-2 生图提示词
6. 每个镜头的 16:9 分镜图
7. 总览图和交付检查

适合 Web3 项目上线宣传片、代币叙事视频、生态飞轮视频、SportFi / GameFi / DeFi 机制解释视频。
```

### 中文长介绍

很多 Web3 项目已经有白皮书、机制、视觉和社区传播素材，但这些材料经常还没有被整理成一条适合视频表达的线。

`web3-promo-video` 的作用是把项目资料先变成视频叙事，再变成可以执行的镜头资产。它默认会先区分已确认公开事实、内部信息、未证实表达和 `待确认`，避免把未确认的投资人、交易所、收益承诺、TVL、用户量或合作方写进公开视频。

默认 90 秒视频会拆成 12 个镜头。每个镜头包含画面内容、拍摄方式、构图、角色动作、台词、声音、画面氛围、Seedance 2 提示词和生图提示词。如果需要生图，会先生成第一张风格校准图，再继续生成整组镜头图。

## English Promo

### One-Line Description

Turn Web3 whitepapers, poster styles, and brand assets into a 90-second promo video storyboard, image prompts, and Seedance 2 shot prompts.

### Short Description

`web3-promo-video` is a Codex skill for Web3 promo video production. It reads project source materials, extracts a mechanism-driven video narrative, and produces voiceover, storyboard, Seedance 2 motion prompts, and gpt-image-2 image prompts for every shot.

It is useful for launch videos, token narrative videos, ecosystem flywheel explainers, public-ledger transparency videos, community-growth content, and client-acquisition videos for Web3 studios.

### GitHub Repository Description

```text
Codex skill for creating Web3 promotional video production packs: storyboard, voiceover, Seedance 2 prompts, gpt-image-2 prompts, and 16:9 generated frames.
```

### English Launch Post

```text
I created a Codex skill for Web3 promo video production: web3-promo-video.

It turns whitepapers, narrative docs, poster styles, brand VI, and mascot assets into a full production pack:

1. Timeline
2. Voiceover
3. Storyboard table
4. Seedance 2 shot prompts
5. gpt-image-2 image prompts
6. 16:9 storyboard frames
7. Contact sheet and QA checklist

It is designed for Web3 launch videos, token narrative videos, ecosystem flywheel explainers, and SportFi / GameFi / DeFi mechanism videos.
```

### Long Description

Many Web3 teams already have source material, but their whitepaper, token mechanics, visual system, and community story are not yet shaped into a video-ready narrative.

`web3-promo-video` turns those materials into an executable production pack. It separates confirmed public facts from internal notes, unsupported claims, and `TBC` items, so the video does not accidentally invent investors, exchange listings, return promises, TVL, active users, or partnerships.

The default 90-second structure uses 12 shots. Each shot includes visual direction, camera movement, composition, character action, voiceover, sound direction, atmosphere, Seedance 2 prompt, and image prompt. When frame generation is requested, the workflow generates the first frame as a style calibration frame before continuing with the rest of the set.
