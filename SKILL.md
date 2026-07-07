---
name: web3-promo-video
description: Create Web3 promotional video production packs from whitepapers, narrative docs, tokenomics notes, poster styles, brand VI, mascot assets, or existing campaign materials. Use when the user asks for Web3 品宣视频, 宣传片, 项目叙事视频, Seedance 2 分镜, 视频文案台词, image generation for every shot, storyboard frames, launch video assets, or a repeatable Web3 promo video workflow.
---

# Web3 Promo Video

Turn Web3 project source material into a production pack for image-to-video tools such as Seedance 2: timeline, voiceover, storyboard, image prompts, generated 16:9 frames, and handoff checks.

## Source Intake

Read project rules first when working inside a repo or project folder. Then inspect the smallest source set needed:

- Project docs: whitepaper, narrative memo, tokenomics, launch plan, pitch deck, README, or campaign copy.
- Visual references: posters, brand VI, mascot, logo, site screenshots, app screens, previous image prompts.
- Current output directory patterns so the deliverable lands beside related campaign assets.

Before writing public copy, separate:

- confirmed public facts
- internal-only facts
- unsupported claims
- `待确认`

Do not turn assumptions, market hopes, investor hints, user growth claims, TVL, audit status, exchange plans, or partner names into public facts unless the source confirms them.

## Narrative Build

Extract one clear video line from the source. Prefer mechanism-driven Web3 narratives over generic slogans.

Common structures:

- Protocol or infrastructure: problem -> mechanism -> user action -> network effect -> public proof.
- DeFi or liquidity: user demand -> liquidity path -> incentive logic -> transparency -> ecosystem loop.
- GameFi or SportFi: gameplay -> on-chain result -> reward or tax flow -> ecosystem pool -> community expansion.
- Launch or ecosystem coin: parent ecosystem -> value source -> return path -> market support -> community spread.
- Studio or service brand: hard product logic -> market-understandable language -> content or visual system -> acquisition path.

If the source has a mascot, IP character, or token emblem, use it as the visual anchor. If it does not, anchor the film on product UI, protocol map, token flow, or ecosystem scene.

## Production Flow

1. Define specs: duration, ratio, platform, language, subtitle plan, image count, and whether to generate frames.
2. Build the timeline. Default to 90 seconds with 12 shots, about 7.5 seconds per shot.
3. Write voiceover before image prompts. Keep each line short enough for the shot duration.
4. Write a full shot table with camera, composition, character action, sound, atmosphere, Seedance 2 prompt, and image prompt.
5. If frame generation is requested, generate one style-calibration frame first for large batches.
6. Generate each final frame with gpt-image-2. If the active image tool cannot use or guarantee gpt-image-2, state the blocker and prepare exact prompts.
7. Copy final images from the generator default location into the project output folder. Do not leave project assets only under `$CODEX_HOME/generated_images`.
8. Normalize every frame to the requested ratio and delivery size. Default landscape delivery is 1920x1080 unless the user asks for 4K.
9. Create a contact sheet or total-view image when there are more than six frames.
10. Save the handoff document beside the frames.

For detailed fields, shot math, prompt schema, folder names, and quality checks, read `references/production-contract.md`.

## Visual Rules

- Match the current project's visual system, not a generic Web3 template.
- Use actual source motifs: mascot, token symbol, product UI, chain, gameplay, community, data flow, map, dashboard, or official brand colors.
- For generated frames, avoid dense text inside the image. Put Chinese copy, title, and subtitles into the video edit unless the user explicitly wants text baked into the frame.
- Keep title-safe empty space in opening and ending frames.
- Maintain character consistency across frames: hair, outfit, palette, emblem placement, body proportion, props.
- Avoid unsupported financial promises, guaranteed returns, pump language, fake partnerships, fake audit claims, and fake public-wallet execution.

## Output

Save a Markdown handoff containing:

- source files used
- video specs
- total video description
- timeline and voiceover table
- per-shot Seedance 2 prompts
- per-shot image prompts
- generated frame file list
- quality check notes

When returning to the user, report the skill path, final output paths, generated image count, ratio verification, and any unresolved `待确认`.
