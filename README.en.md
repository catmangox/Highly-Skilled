# Japan HSP Points Calculator · 高度人才评分系统

[简体中文](README.md) | [繁體中文](README.zh-TW.md) | [日本語](README.ja.md) | [한국어](README.ko.md) | **English**

A self-assessment tool for Japan's Highly Skilled Professional (高度専門職) visa points. Check the items that apply to you, per the official Immigration Services Agency point table (ministerial ordinance), and your score is calculated in real time: **70 points** qualifies for HSP status, and **80 points** unlocks the 1-year permanent-residency track.

**Try it online: [point.keihan.co](https://point.keihan.co)** · © KEIHAN JUGYO K.K. 京阪住業株式会社

## Features

- **Three categories**: Academic Research (イ) / Advanced Technical (ロ) / Business Management (ハ), each with its own point table and options
- **Complete point rules**: education, professional experience, age, annual income (including age-gated tiers), research achievements, position, Japanese proficiency, and special bonuses
- **Five languages**: Simplified Chinese / Traditional Chinese / Japanese / Korean / English, switchable in one click
- **Live score panel**: 70 / 80-point threshold status, list of benefits, progress bar
- **Rule-conflict warnings**: e.g. the N2 bonus cannot be combined with the Japanese-university bonus; the SME bonus only counts together with the innovation-support item
- **Gap-closing suggestions**: when short of the target score, the most effective bonus items are listed automatically
- **Light / dark theme**: one-click toggle, preference remembered locally
- **Mobile-friendly**: responsive layout plus a sticky bottom score bar

## Usage

Want to try it right away? No install needed — just visit **[point.keihan.co](https://point.keihan.co)**.

Run locally: a pure static page with no build step and no runtime dependencies:

```bash
# Just open it in a browser
open index.html
```

Or deploy to any static host (GitHub Pages, Netlify, etc.) — the repository root is the site.

## Project structure

```
├── index.html                 # Single-file app: page, styles, scoring logic
└── assets/
    └── logo-mark-zinc.png     # KEIHAN brand mark (auto-inverts with the theme)
```

Technically it is one self-contained HTML file: the Keihan design-system color and typography tokens are inlined, the scoring engine and multilingual rendering are implemented in vanilla JavaScript, and fonts load from Google Fonts with system-font fallbacks.

## Disclaimer

This tool is a reference calculation based on the ministerial-ordinance point table; the final determination rests with the Immigration Services Agency of Japan.
