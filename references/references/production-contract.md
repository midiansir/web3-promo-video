# Web3 Promo Video Production Contract

Use this file when creating a Web3 promotional video production pack, especially when the user needs Seedance 2 prompts, generated storyboard frames, or a repeatable campaign workflow.

## Default Deliverable Shape

Default folder when the project has no stronger convention:

```text
02_生图素材与Prompt/YYYY-MM-DD_<ProjectName>宣传片/
├── <ProjectName>宣传片_<duration>_分镜台词与Seedance提示词.md
├── <ProjectName>宣传片_<duration>_镜头总览.png
└── frames/
    ├── shot-01-opening-hero.png
    ├── shot-02-...
    └── shot-12-final-hero.png
```

Use the current project's existing naming style when it is already clear.

## Shot Count

Use these defaults unless the user specifies otherwise:

| Duration | Shot Count | Per Shot |
|---:|---:|---:|
| 30s | 5 to 6 | 5 to 6s |
| 45s | 7 to 8 | 5 to 6s |
| 60s | 8 to 10 | 6 to 7.5s |
| 90s | 12 | 7.5s |
| 120s | 14 to 16 | 7 to 8.5s |

For Web3 explainers, do not overload a shot with several mechanism steps. One shot should express one event, one transition, or one proof point.

## 90 Second Story Patterns

### Ecosystem Return Pattern

Use for sub-token, revenue return, fee return, protocol flywheel, or ecosystem-pool stories.

```text
01 opening system hero
02 parent ecosystem or core product activity
03 on-chain proof or transparent result
04 value source appears
05 value enters pool or treasury
06 pool branches into support actions
07 project token or mascot receives narrative role
08 second growth path or market route
09 public wallet, ledger, or disclosure
10 community amplification
11 value flywheel
12 final hero and tagline frame
```

### Product Capability Pattern

Use for wallet, DApp, AI tool, infrastructure, analytics, or SaaS-like Web3 products.

```text
01 market pain or high-level promise
02 user enters product
03 core workflow begins
04 key technical mechanism
05 first useful result
06 integration or ecosystem connection
07 trust layer or security proof
08 scale or automation
09 user outcome
10 community or partner ecosystem
11 product flywheel
12 final hero and CTA frame
```

### Brand Studio Pattern

Use for Web3 service brands, studios, agencies, or content-operation offers.

```text
01 category pain
02 hard product logic is invisible to market
03 studio translates logic into narrative
04 visual system makes it recognizable
05 content system makes it repeatable in channels
06 website or deck becomes sales entry
07 short video and motion explain the mechanism
08 X, Medium, community, and campaign assets distribute it
09 lead or user action appears
10 proof without fake claims
11 ongoing operation loop
12 final service promise
```

## Shot Table Fields

Use these fields in the handoff table:

| Field | Requirement |
|---|---|
| 镜号 | `01`, `02`, `03` |
| 时间 | Start and end time |
| 画面文件 | Relative frame path |
| 画面内容 | What happens in the frame |
| 拍摄方式 | Fixed, push, pull, pan, track, orbit, handheld |
| 拍摄参数 | Focal length, height, depth, light, duration, transition |
| 景别 | Extreme wide, wide, medium, close-up, detail |
| 构图 | Subject position, foreground, midground, background, safe area |
| 角色动作 | Character action, expression, prop movement |
| 台词 | Voiceover or dialogue |
| 声音 | Music, ambience, SFX |
| 画面氛围 | Palette, light, emotion, rhythm |
| Seedance 2 提示词 | One complete prompt for image-to-video |
| 生图提示词 | One complete prompt for gpt-image-2 |

## Voiceover Rules

- Write for speech first, not poster copy.
- Use one sentence per shot when possible.
- Avoid financial promises and exaggerated certainty.
- For 7.5 seconds, keep Chinese voiceover roughly 18 to 32 characters unless the sentence is slow and simple.
- Put complex mechanism words into visuals only when they are source-confirmed and important.

## Seedance 2 Prompt Shape

Write each prompt in this order:

```text
作品类型与项目类型，主要角色或主体，场景和道具，当前动作，镜头运动，景别和构图，光线和色调，情绪，画质要求，禁止项。
```

One prompt should describe one continuous shot. Do not pack a before-and-after sequence with several locations into one prompt.

## Image Prompt Shape

Use English image prompts for gpt-image-2 unless the user requests Chinese prompts.

```text
16:9 landscape. <Scene/backdrop>. <Main subject>. <Project-specific visual motifs>. <Style and medium>. <Composition>. <Lighting and palette>. <Materials and textures>. Text constraints. Avoid list.
```

For generated frames:

- Include exact ratio.
- Include project-specific visual anchors.
- Ask for no watermark.
- Ask for no dense text unless text is required.
- Ask for clean empty space when later title or subtitles are expected.
- Name the intended shot number and use.

## Image Generation Sequence

For batches:

1. Generate shot 01 as style calibration.
2. Inspect shot 01 for ratio, style, character, and project symbols.
3. Continue with the remaining shots if the visual language works.
4. Copy each selected image into the project folder.
5. Resize to delivery dimensions.
6. Verify all dimensions.
7. Create a contact sheet.

Suggested filenames:

```text
shot-01-opening-hero.png
shot-02-source-engine.png
shot-03-proof-layer.png
shot-04-value-source.png
shot-05-ecosystem-pool.png
shot-06-distribution-paths.png
shot-07-token-hero.png
shot-08-growth-path.png
shot-09-public-ledger.png
shot-10-community-heat.png
shot-11-flywheel.png
shot-12-final-hero.png
```

## Quality Check

Before finishing, verify:

- All frames have the requested ratio and size.
- Project name, token name, mascot, logo, palette, and scene motifs are consistent.
- Images do not contain unwanted dense Chinese text or fake UI labels.
- No public claim exceeds the source material.
- `待确认` items remain marked.
- The handoff document includes Seedance 2 prompts and image prompts for every shot.
- The final file list points to local project paths, not only generator cache paths.
- Contact sheet exists when the frame count is more than six.
