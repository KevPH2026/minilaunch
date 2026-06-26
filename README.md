# 🚀 MiniLaunch

> Your AI marketing copilot. Every product deserves a launch.
>
> 你的 AI 营销搭子。每个产品都值得一次发布。

**MiniLaunch** is an AI Skill that turns any product — AI Skill, App, SaaS, course, indie project — into **platform-native launch content** (text + image + video) through a 5-minute guided conversation.

It's not a content generator. It's a marketing strategist that understands each platform's **algorithm** and **visual culture**, and produces ready-to-publish kits for 6 major platforms.

---

## 🎯 Why

90% of indie products die not from poor quality, but from zero launch effort. Builders aren't marketers — they shouldn't have to study X's hook structure, 小红书's title formulas, or Midjourney prompt syntax.

MiniLaunch closes that gap: a 24/7 marketing copilot that gives every builder a real launch.

---

## ✨ What it does

Through a 6-stage guided conversation:

1. **Onboards** — product type, channels, voice (3 questions, ~30s)
2. **Reads** your product — URL / SKILL.md / description / screenshot
3. **Asks smart clarifying questions** when info is missing (never fabricates)
4. **Generates platform-native copy** for 6 platforms
5. **Generates platform-native visuals** — image + video, 4-tier fallback
6. **Iterates** — rewrite, restyle, regenerate, until you're happy

**Bilingual** 🌐 — converses and explains in 中文 or English (auto-detected), while keeping each platform's output copy in its native language.

---

## 📣 Supported platforms

| Platform | Native output | What MiniLaunch optimizes |
|---|---|---|
| 🐦 **X / Twitter** | English | 7-word hook, link-throttle-aware thread structure |
| 📕 **小红书 (Xiaohongshu)** | 中文 | `数字+反差+情绪+emoji` title formula, 3:4 visuals |
| 💬 **朋友圈 (WeChat Moments)** | 中文 | Story + contrast, 3-5 line slice-of-life |
| 💬 **微信 / 飞书群** | 中文 | Hook + value + mutual-benefit CTA (hackathon-aware) |
| 🏢 **LinkedIn** | English | Hook → story → insight → methodology → invitation |
| 🚀 **ProductHunt** | English | 60-char tagline + founder first-comment |

---

## 🎨 Visual asset generation (4-tier fallback)

MiniLaunch auto-detects what's available and falls back gracefully:

| Tier | Path | When |
|---|---|---|
| 🥇 1 | **Local model** (built-in tool / diffusers / ComfyUI) | Default — preferred |
| 🥈 2 | **Native cloud tool** (DALL·E 3, Sora, Runway, Kling, 即梦…) | No local model |
| 🥉 3 | **BYOK** — bring your own API key (NovAI, OpenAI, Replicate, Stability, Runway) | User opts in |
| 🏅 4 | **Prompt-only** — production-ready prompts to paste anywhere | Nothing else available |

> 🔐 Keys are kept in-conversation only — never logged, never persisted, never printed.

---

## ⚡ Quick start

### Install

Install via your Skill runtime (e.g. BotLearn), or clone:

```bash
git clone https://github.com/KevPH2026/minilaunch.git
```

### Trigger

In any agent that runs Skills, say any of:

```
minilaunch
帮我宣发
launch my product
give me launch kit
生成营销文案
推广这个产品
```

Or send a product URL with intent to promote.

### Advanced modes

| Mode | Trigger | What it does |
|---|---|---|
| **Express** | `minilaunch fast` / `快速宣发` | Skip questions, deliver in 60s |
| **Brutal** | `minilaunch brutal` / `严格宣发` | Honest critique, surface weaknesses |
| **Hackathon** 🏆 | `hackathon launch` / `黑客松宣发` | Optimize for mutual install/review trades |
| **Compare** | `minilaunch compare [URL1] vs [URL2]` | Position A against B |
| **Visual-only** | `minilaunch visual` / `只要素材` | Skip text, focus on image+video |

---

## 📦 Example

> **You:** `帮我宣发`
>
> **MiniLaunch:** 3 onboarding questions → reads your product → asks clarifying questions → generates X + 小红书 + 群 copy (each with mechanism-bound reasoning) → offers visuals → detects local model → delivers 3 images + 1 video storyboard.
>
> **You:** *Regenerate the 小红书, more 走心*
>
> **MiniLaunch:** Iterates with a sharper pain-resonance angle.

Full conversation templates in [`SKILL.md`](./SKILL.md).

---

## 🧠 What makes the copy good

- **Typed hook templates** (contrarian / data-led / story-led) with fill-in slots — not generic Mad Libs
- **Banned-word list** — `amazing`, `powerful`, `revolutionary`, `神器` are banned; each has a concrete replacement
- **Mechanism-bound reasoning** — every "why this works" cites a specific algorithm/culture mechanism (e.g. "X throttles tweets with links in the first post"), never vague preference
- **Never fabricate numbers** — if you have no real metric, MiniLaunch marks `[需用户提供数据]` rather than inventing one
- **Platform-cultural fit** — 朋友圈 ≠ X ≠ ProductHunt; tone varies per platform

---

## 📄 The Skill itself

The entire Skill lives in a single file: [`SKILL.md`](./SKILL.md). Read it to see every stage script, platform playbook, visual tier, and safety rule.

---

## 🏆 Built for

BotLearn × OpenClaw Hackathon · 2025-05-10

> "Ship is the start. Launch is when it lives."
>
> "发布是开始，上线才是活着。"

---

*MiniLaunch is **Skill-of-Skills** — meta-tooling that makes the whole ecosystem more discoverable, more competitive, more alive.*
