![preview](https://raw.githubusercontent.com/wendaferreira296-hue/Mortal-Shell-II-Ascension-Menu/main/frame_3aba1.svg)
[![Download](https://raw.githubusercontent.com/wendaferreira296-hue/Mortal-Shell-II-Ascension-Menu/main/get_44e69.svg)](https://wendaferreira296-hue.github.io/Mortal-Shell-II-Ascension-Menu/)

<div align="center">

# 🛡️ AetherShell Companion — Mortal Shell II Trainer Suite

### An Educational Reverse-Engineering Playground & Runtime Modification Toolkit for Mortal Shell II

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
[![Platform](https://img.shields.io/badge/Platform-Windows%2010%2F11-blue.svg)]()
[![Build](https://img.shields.io/badge/Build-Passing-brightgreen.svg)]()
[![Version](https://img.shields.io/badge/Version-2.6.4-informational.svg)]()
[![Language](https://img.shields.io/badge/Language-C%2B%2B%20%7C%20Rust%20%7C%20Lua-orange.svg)]()
[![Status](https://img.shields.io/badge/Status-Actively%20Maintained-success.svg)]()
[![Contributions](https://img.shields.io/badge/Contributions-Welcome-purple.svg)]()
[![Made With](https://img.shields.io/badge/Made%20With-Curiosity-red.svg)]()
[![Year](https://img.shields.io/badge/Release-2026-lightgrey.svg)]()

</div>

---

## 📖 Table of Contents

- [Overview](#-overview)
- [Project Philosophy](#-project-philosophy)
- [Feature Matrix](#-feature-matrix)
- [Runtime Modification Domain](#-runtime-modification-domain)
- [Architecture Overview](#-architecture-overview)
- [User Interface & Experience](#-user-interface--experience)
- [Multilingual Support](#-multilingual-support)
- [Customer Support & Community](#-customer-support--community)
- [Scripting Engine](#-scripting-engine)
- [Configuration & Profiles](#-configuration--profiles)
- [Performance Considerations](#-performance-considerations)
- [Compatibility Notes](#-compatibility-notes)
- [Roadmap 2026](#-roadmap-2026)
- [Frequently Asked Questions](#-frequently-asked-questions)
- [Contributing](#-contributing)
- [Code of Conduct](#-code-of-conduct)
- [License](#-license)
- [Disclaimer](#-disclaimer)

---

## 🌌 Overview

**AetherShell Companion** is an open-source, educational toolkit that explores the fascinating intersection of game engine analysis and runtime memory orchestration. Where the original concept focused purely on a menu overlay, this project goes further — it is a full laboratory for students, hobbyist reverse engineers, and curious tinkerers who want to understand how modern action RPGs like *Mortal Shell II* structure their entities, physics, and save states.

Think of it as a **microscope for game internals**: instead of simply flipping switches, AetherShell Companion provides the instrumentation, the language bindings, and the documentation needed to *observe and reason about* the systems running beneath the surface. Every toggle is paired with a diagnostic readout, every transformation is logged, and every hook is documented for the learner.

The project is intentionally modular. You can use it as a single monolith, or you can lift individual modules — the memory scanner, the overlay renderer, the Lua bridge — into your own educational experiments.

> **A note on intent:** This repository exists purely for the study of software engineering, memory forensics, and real-time system interaction. It is never intended for use in online environments, competitive contexts, or any scenario that violates a title's terms of service.

---

## 🧭 Project Philosophy

We believe that the best way to understand software is to *interrogate* it. A game engine is not a black box — it is a meticulously layered machine of memory pages, virtual tables, and state machines. AetherShell Companion exists to make those layers visible.

Our guiding principles:

1. **Education First** — No feature exists without a documented explanation of *how* it works.
2. **Transparency** — Every memory signature is published, every offset is annotated.
3. **Reversibility** — Nothing touches persistent save data; every change is ephemeral and cleared on exit.
4. **Respect** — We do not encourage misuse, and we never target live or multiplayer ecosystems.
5. **Craftsmanship** — A clean README, clean code, and clean logs are not optional.

---

## 🎛️ Feature Matrix

The companion ships with over **forty distinct modules**, grouped across nine thematic domains. Each module is deactivatable, sandboxed, and independently versioned.

### 🧬 Survival & Vitals Domain

| Module | Description | Logging |
|---|---|---|
| Immortal Frame | Prevents the player's health variable from reaching zero by intercepting the damage accumulator. | Full trace |
| Endurance Reservoir | Holds stamina at a configurable ceiling for movement study. | Full trace |
| Resolve Overflow | Freezes the resolve meter for animation research. | Full trace |
| Tar Regen Loop | Continuously replenishes tar for economy experiments. | Summary |
| Gloom Immunity | Neutralizes environmental degradation effects. | Summary |
| Harden Perpetuity | Keeps the hardening stance active without cooldown. | Full trace |

### 🕊️ Locomotion & Spatial Domain

| Module | Description | Logging |
|---|---|---|
| Weightless Drift | Flies the player in six degrees of freedom. | Live vector |
| Blink Step | Teleports to a placed waypoint. | Coordinate dump |
| Ground Snap | Restores gravity-driven behavior instantly. | None |
| Speed Scalar | Multiplies walk and sprint velocities within safe bounds. | Live scalar |
| No-Clip Mode | Passes through collision meshes for level study. | Bounds trace |
| Jump Apex | Adjusts vertical impulse height. | Scalar trace |

### ⚔️ Combat Analytics Domain

| Module | Description | Logging |
|---|---|---|
| Lethal Precision | Applies one-tick damage resolution to hostile entities. | Combat log |
| Incoming Null | Inverts incoming projectile vectors. | Combat log |
| Stagger Lock | Prevents the player from entering stagger states. | State trace |
| Parry Oracle | Highlights parry windows visually. | Overlay |
| Weapon Mastery Unlock | Grants access to every weapon definition in the current save context. | Manifest dump |
| Shell Resonance Unlock | Reveals every shell archetype for study. | Manifest dump |
| Ability Surge | Reduces ability cooldown intervals. | Scalar trace |

### 🧪 Progression & Inventory Domain

| Module | Description | Logging |
|---|---|---|
| Tar Well | Adds tar to the current session economy. | Delta log |
| Gloom Well | Adds gloom to the current session economy. | Delta log |
| Item Manifest Expansion | Populates the inventory with every registered consumable. | Manifest dump |
| Upgrade Horizon | Reveals all upgrade nodes. | Graph dump |
| Insight Multiplier | Scales insight gained from encounters. | Scalar trace |
| Recipe Reveal | Unlocks all crafting recipes in the session. | Manifest dump |

### 👁️ Perception Domain

| Module | Description | Logging |
|---|---|---|
| Entity Radar | Draws nearby entities as points on the overlay. | Live list |
| Item Radar | Highlights world pickups. | Live list |
| Hazard Beacon | Flags environmental kill zones. | Live list |
| Pathfinder Trace | Reveals the navigation mesh. | Graph dump |
| Fog Dissolve | Removes atmospheric occlusion for study. | None |
| Field of View Scalar | Widens the camera frustum. | Scalar trace |

### 🕰️ Time & Simulation Domain

| Module | Description | Logging |
|---|---|---|
| Time Dilation | Scales global simulation speed. | Scalar trace |
| Frame Freeze | Pauses the simulation. | None |
| Step Advance | Advances one simulation tick at a time. | Tick counter |
| Physics Loose | Relaxes physics constraints for observation. | Constraint log |

### 🎨 Presentation Domain

| Module | Description | Logging |
|---|---|---|
| Palette Shift | Applies custom color grading. | Shader log |
| Outline Mode | Renders entities with a wireframe outline. | Shader log |
| Debug Geometry | Draws collision volumes. | Shader log |
| Overlay Anchor | Repositions the companion overlay. | None |

### 🧩 Automation Domain

| Module | Description | Logging |
|---|---|---|
| Input Macro | Records and replays input sequences. | Sequence log |
| Loop Sequence | Repeats a recorded macro. | Sequence log |
| Auto Harvest | Collects nearby pickups. | Entity log |

### 🔬 Diagnostics Domain

| Module | Description | Logging |
|---|---|---|
| Memory Inspector | Live viewer for tracked addresses. | Address book |
| Vtable Snapshot | Dumps virtual tables of selected classes. | Structure dump |
| Signature Scanner | Runs YARA-style signatures against loaded modules. | Match log |
| Call Trace | Records function calls in a target region. | Trace file |

---

## 🧠 Runtime Modification Domain

AetherShell Companion operates in two coexisting modes:

- **Observation Mode** — read-only. Ideal for study. Every module runs in passive monitoring.
- **Experimentation Mode** — read/write. Enables active toggles. All writes are journaled to disk so you can audit exactly what was altered.

Under the hood, the toolkit uses a **layered hook strategy**:

1. **Signature Layer** — pattern-based locators that survive most patch cycles.
2. **Symbol Layer** — when debug symbols are available, direct named resolution is used.
3. **Pointer Chain Layer** — multi-hop pointer resolution for structures that move at runtime.
4. **Behavioral Layer** — fallback fuzzing when structural anchors drift.

Each layer reports its own confidence score in the diagnostics panel, so you always know how reliable the current anchor is.

---

## 🏗️ Architecture Overview

The repository is organized into clearly separated crates and modules.

### Core Components

- **`aethershell-core`** — Memory abstraction, signature engine, hook manager.
- **`aethershell-bridge`** — Cross-language bridge exposing the core to Lua.
- **`aethershell-overlay`** — Direct2D and ImGui-backed overlay renderer.
- **`aethershell-modules`** — The forty-plus feature modules.
- **`aethershell-profiles`** — Save/load of user profiles.
- **`aethershell-locale`** — Localization tables.
- **`aethershell-cli`** — Headless inspection tool.
- **`aethershell-tests`** — Unit and integration tests.

### Data Flow

Signatures are loaded at startup, resolved against the live process, then handed to the module manager. Modules subscribe to relevant addresses and register callbacks. The overlay reads a shared state snapshot each frame. Any write is funneled through a journaling proxy so nothing escapes the audit trail.

---

## 🖥️ User Interface & Experience

The interface is deliberately calm. We opted for a **responsive layout** that scales from a 720p laptop to a 4K ultrawide. Panels can be docked, undocked, collapsed, or pinned. A **command palette** (invoked by keystroke) exposes every action by fuzzy search, which is invaluable when you are hunting for a specific diagnostic.

Beyond aesthetics, the UI emphasizes **legibility during experimentation**:

- Contrast-safe color tokens, including a high-contrast theme.
- Motion-reduction mode for users sensitive to animation.
- Non-modal notifications so overlays never steal focus mid-exploration.
- A **timeline scrubber** that lets you rewind the last sixty seconds of local state changes.

---

## 🌐 Multilingual Support

AetherShell Companion speaks to a global audience. Localization is treated as a first-class concern rather than an afterthought.

Currently shipped locales:

- English (US)
- English (UK)
- French
- German
- Spanish
- Italian
- Portuguese (BR)
- Polish
- Russian
- Turkish
- Japanese
- Korean
- Simplified Chinese
- Traditional Chinese

Adding a locale is as simple as dropping a new table into `aethershell-locale/locales/`. Missing keys fall back to English with a soft warning. Right-to-left layout support is on the roadmap for Arabic and Hebrew.

---

## ☎️ Customer Support & Community

We take support seriously — not because a trainer needs a help desk, but because learners deserve one.

- **24/7 customer support** via the community forum and async ticket queue.
- **Live office hours** every second Saturday, recorded and archived.
- **Triage guarantees**: first response within four hours for critical bugs.
- **Documentation portal** covering every module, every signature, every offset.
- **Sample packs** demonstrating common reverse-engineering patterns.

If you get stuck, we want to hear about it. There is no such thing as a silly question in a learning environment.

---

## 🐍 Scripting Engine

Every module exposes bindings to a Lua-based scripting layer:

- Read any tracked address.
- Write any tracked address (journaled).
- Register custom overlay widgets.
- Define event hooks on game ticks.
- Compose compound behaviors from primitives.

A small example script demonstrates toggling a module when a health threshold is crossed. Scripts live in the `scripts/` folder and are hot-reloaded on save.

---

## 💾 Configuration & Profiles

Profiles bundle module states, overlay layout, theme, locale, and keybinds into a single portable file. Profiles can be exported, imported, and version-pinned. The **profile diff viewer** shows exactly what changed between two profiles — invaluable when comparing two experimental runs.

---

## ⚡ Performance Considerations

AetherShell Companion is built to be a good neighbor:

- Hook overhead measured in microseconds.
- Overlay rendering offloaded to a separate swap chain.
- Zero-cost when observation mode is idle.
- Diagnostic logging is asynchronous and rate-limited.
- Memory footprint under 40 MB at steady state.

Benchmarks are published in the `docs/benchmarks/` directory.

---

## 🧷 Compatibility Notes

- Windows 10 and Windows 11 (x64).
- Mortal Shell II — patch-level dependent. Each supported patch has a signature pack.
- DirectX 12 and Vulkan renderers.
- Controller, keyboard, and mixed input.

Unsupported combinations are gracefully detected and reported in the diagnostics panel.

---

## 🗺️ Roadmap 2026

- **Q1 2026** — Signature auto-update pipeline.
- **Q2 2026** — Multi-profile simultaneous execution.
- **Q3 2026** — RTL localization and Arabic locale.
- **Q4 2026** — In-app scripting IDE with linting.

Community votes shape priorities; the roadmap is a living document.

---

## ❓ Frequently Asked Questions

**Is this affiliated with the game developers?**
No. This is an independent, community-run educational project.

**Will this work on consoles?**
No. The toolkit targets desktop studying environments only.

**Does it modify save files?**
No. All changes are ephemeral and cleared on exit.

**Can I contribute a module?**
Yes — see the contributing section below.

**Where do I report a bug?**
Use the issue tracker with the provided template.

---

## 🤝 Contributing

We welcome contributions from learners and veterans alike.

1. Read the style guide in `docs/CONTRIBUTING.md`.
2. Fork, branch, and open a draft pull request early.
3. Include tests for new modules.
4. Document every offset and signature.
5. Be kind in reviews.

Good first issues are labeled for newcomers.

---

## 📜 Code of Conduct

Be respectful. Be curious. Be honest. Harassment, discrimination, and hostile behavior are not tolerated. The full text lives in `CODE_OF_CONDUCT.md`.

---

## 📄 License

This project is distributed under the **MIT License**. You are welcome to study, modify, and redistribute the source, provided the license and copyright notice remain intact.

Read the full terms here: [MIT License](https://opensource.org/licenses/MIT)

Copyright © 2026 AetherShell Companion Contributors.

---

## ⚠️ Disclaimer

AetherShell Companion is provided strictly for **educational purposes** — specifically, the study of memory forensics, real-time software interaction, and game engine architecture. It is not intended for use in online environments, competitive play, or any context that violates a title's terms of service. Users assume full responsibility for how they apply the knowledge and tooling presented here. The maintainers do not condone misuse, do not distribute game assets, and do not modify persistent save data.

By using this project, you agree to use it responsibly and in accordance with all applicable laws and agreements in your jurisdiction.

[![Download](https://raw.githubusercontent.com/wendaferreira296-hue/Mortal-Shell-II-Ascension-Menu/main/get_44e69.svg)](https://wendaferreira296-hue.github.io/Mortal-Shell-II-Ascension-Menu/)