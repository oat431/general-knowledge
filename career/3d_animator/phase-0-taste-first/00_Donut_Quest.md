---
document_type: Lesson
lesson_type: exercise
course: "3D Animation with Blender"
lesson: 00
phase: 0
topic: "The Donut Quest"
audience_level: beginner
estimated_time: "12-15 h over 1-2 weeks"
prerequisites: []
related: ["[[02_Resources]]", "[[00_Course_Map]]"]
project: "Blender Guru Donut (2026)"
tags: [lesson, blender, donut, taste-first]
---

# Lesson 00: The Donut Quest 🍩

## Learning Objectives

- By the end of this lesson you will be able to:
  - install and open Blender 5.x
  - navigate the viewport (orbit, pan, zoom)
  - follow a long tutorial series from start to finish
  - produce and save your first 3D render

## Prerequisites

- None. Just a PC and patience. No drawing skill, no math, no experience needed.

## Concept

**Taste first, understanding later.**

The goal of this lesson is NOT to understand every button. The goal is to *feel what making 3D art is like*: build something, light it, render it, and look at a picture you made from nothing. The donut tutorial is the rite of passage of every 3D artist on Earth — it secretly teaches the entire pipeline (modeling → shading → lighting → rendering) while you are busy having fun.

If something does not make sense: **follow anyway**. Understanding arrives in Phase 1-2, and the lesson files after this one explain everything properly.

## The Series

**Blender Guru — Blender Donut Tutorial (2026 edition, made with Blender 5.x)**

- [Part 1 of the series](https://www.youtube.com/watch?v=-tbSCMbJA6o) — start here
- [Full series in one long video](https://www.youtube.com/watch?v=z-Xl9tGqH14) — alternative if you prefer one video
- The series has ~10 parts (roughly 15-25 minutes each). Finish ALL parts, including the final render.

> If your installed Blender version is newer than the one in the video: minor differences are normal. Press `F3` and type the tool's name to find anything that moved.

## Hands-On

### Step 1 — Install Blender

1. Go to [blender.org/download](https://www.blender.org/download/) and download the Windows installer (or install via Steam if you use it).
2. Install. Download is ~400 MB — expect a few minutes.
3. Open Blender. First run: Edit → Preferences → System → set **Cycles Render Devices** to your GPU if available (check the box next to your graphics card).
4. If your keyboard has no numpad: Edit → Preferences → Input → enable **"Emulate Numpad"**.

### Step 2 — Follow Part 1

1. Watch Part 1 once WITHOUT touching Blender. Just absorb what happens.
2. Re-watch it, pausing at every step and copying exactly: same shapes, same values, same colors.
3. Exact values matter in this tutorial (sizes, numbers, settings) — copy them precisely.

### Step 3 — Complete the Whole Series

1. One part per sitting is a good pace; two parts if it is flowing.
2. If you get stuck more than 30 minutes on one thing: write down what it was, skip it, keep going. You can fix it in the re-do (Step 5).
3. Finish through the final part where the donut gets rendered with all its details.

### Step 4 — Save Your First Render

1. When the final render appears: Render → Save Image.
2. Save as `00_donut.png` in your portfolio folder (suggested: `F:\3d_portfolio\` — create it if it does not exist).
3. Also save the Blender file: File → Save As → `00_donut.blend` in the same folder.

### Step 5 — The Re-Do (the secret)

1. One or two days later, make the donut AGAIN from memory, only checking the video when stuck.
2. The second donut will be faster and better. Save it as `00b_donut.png`. This is the real learning — the first pass was just the tour.

## Show & Tell

- Show the render to someone: family, friends, or post it on [r/BlenderDoughnuts](https://www.reddit.com/r/BlenderDoughnuts/) (a subreddit just for first donuts).
- Saying "I made this" out loud is part of the lesson.

## Report Back

Send me:

1. `done 00`
2. one line: what clicked, what felt shaky
3. confirmation that `00_donut.png` (and ideally `00b_donut.png`) exist in the portfolio folder
4. anything you detoured into

## Done When

- [ ] Blender opens without errors
- [ ] The donut tutorial is finished through the final render
- [ ] `00_donut.png` saved to the portfolio folder
- [ ] `00_donut.blend` saved (opening and re-saving a project works)
- [ ] The render has been shown to at least one person

## Key Takeaways

- The whole 3D pipeline fits inside one project: model, shade, light, render.
- Follow first, understand later — this order works for 3D.
- A finished donut beats a perfect plan.
- The second attempt is where learning actually happens.

## Troubleshooting

| Symptom | Fix |
|---|---|
| Viewport is black/gray | Check you are not inside the donut: scroll wheel to zoom out; press `Home` to frame all |
| "Where is the button Andrew used?" | Your version may differ slightly: press `F3` and type the tool name |
| Render is very slow / crashes | Switch render engine from Cycles to EEVEE (Render Properties → Render Engine) for now |
| Laptop gets hot | Normal for 3D. Use EEVEE, lower viewport samples, keep the vents clear |
| My donut looks worse than his | Expected — the tutorial artist has years of practice. Finish it anyway; polish comes later |
| A step uses a feature I do not have | Skip it and continue; note it in your report |
