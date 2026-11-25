# TESS FPS Optimizer — free preview

**Live: https://pixelrush-ai.github.io/tess-fps-optimizer/**

A single-file, offline FPS diagnostic console for competitive shooters. Pick a game, CPU, GPU and
memory; it estimates the CPU and GPU ceilings separately, names the bottleneck, and shows an
estimated average, 1% low, frame time and a recommended frame cap — plus the 3 in-game rows that
move most on that exact build.

- 8 games (PUBG · VALORANT · War Dogs · CS2 · Apex Legends · Overwatch 2 · Call of Duty: Modern Warfare 4 · Delta Force)
- 25 CPUs (AMD AM4/AM5 + Intel 12th–14th, Core Ultra) and 31 GPUs (GeForce GTX 16/RTX 20–50, Radeon RX 6000/7000/9000)
- Brand tabs and generation groups keep the picker short on a phone
- 3 memory sizes, 3 refresh rates, 3 symptoms
- KR / EN in one page, responsive down to phone width
- Everything is computed in the browser. No account, no upload, no tracking

This repository hosts the **free preview**: the diagnosis and 3 in-game rows. The paid build adds
the remaining settings rows (in-game, driver, Windows) as a 20–25-row table and generates a Windows
`.bat` tailored to the selected spec, with a restore point and a full rollback.

Paid build: Kmong ₩9,900 (KR) · Ko-fi $9.99 (global) — https://ko-fi.com/s/d8d78fecea

---

## Free vs paid

| | Free preview (this page) | Paid build (single HTML file) |
| --- | --- | --- |
| Bottleneck / FPS / 1% low / cap | ✅ | ✅ |
| In-game rows | 3 | all |
| Driver + Windows rows | — | ✅ (20–25 rows total, by game) |
| Tailored `.bat` + rollback | — | ✅ |
| License | none | 1 key per purchase, works offline |

## What the paid `.bat` does — and does not

Changes: restore point → registry backup → power plan → Game Mode / background apps → GameDVR,
MPO → telemetry policy → Nagle → DNS. Menu: 1 apply / 2 restore / 3 exit.

Never touches: game files, anti-cheat (Vanguard · BattlEye · VAC · EAC · Ricochet · ACE), kernel drivers, Defender,
services, `bcdedit`, timer-resolution hacks.

## Accuracy

FPS values are model estimates built from public benchmarks and hardware indices. Real numbers
move ±10~15% (recent titles with thin public data: ±20%) with map, patch, driver and scene
complexity. No frame-gain number is promised — an average that rises while the 1% low falls makes
fights worse.

## Run it locally

Download `index.html` from this repository and open it in Chrome or Edge. No server, no build step,
no network calls other than the optional web font.

## Contact

Message the TESS shop on Ko-fi, or open an issue here for anything about this free page.
