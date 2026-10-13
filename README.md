# NBAStream

An original 3-on-3 arcade streetball game for PC (Steam), inspired by the feel of classic early-2000s streetball games. Features a roster of parody characters inspired by streamer culture.

> **Ground rules**
> - Gameplay ideas, genre and overall vibe are borrowed; **assets, code, names and trademarks are not.**
> - No extracted textures, models, animations, audio, code or data tables from any existing game go into this project, even edited.
> - Parody characters use new names, caricatured designs and original personas. No real handles, photos or logos, and no real names in marketing.
> - Research lives in a **separate folder/repo** from the game. Nothing is copied from research into the game.

---

## Implementation plan

### Phase 0: Foundation
- [ ] Write a one-page concept: core loop, modes, tone, platform (PC, controller-first).
- [ ] Draft the parody roster: new names, caricatured personas, and how each is transformed from its inspiration.
- [ ] Set up two separate folders/repos: **research** (notes, footage, RE findings) and **game** (this project).

### Phase 1: Study the original in PCSX2
- [ ] Extract the game's ELF (`SLUS_xxx.xx`) from your own ISO with 7-Zip.
- [ ] Play at full speed and record footage to judge feel and pacing. Use frame advance to break down dunks, tricks and camera moves.
- [ ] For each mechanic (start with the trick/game-breaker meter):
  1. Find its value in RAM with the PCSX2 debugger's memory search (or Cheat Engine).
  2. Set a write breakpoint to land on the code that changes it.
  3. Open that address in Ghidra with the Emotion Engine extension.
  4. Have Claude (via REA, or with exported functions) explain the logic.
  5. Write a design note in your own words. Close the tools.
- [ ] Use texture dumps only as style reference (resolution, palette, detail level). Never trace or edit them.

### Phase 2: Greybox prototype
- [ ] Build from design notes in Godot or Unity, with Claude Code helping on code.
- [ ] 3v3 with capsules on a flat court: movement, dribble, pass, shoot, steal/block, one trick, the meter, one special move.
- [ ] Simple AI opponents and local 2-player.
- [ ] Tune numbers by feel, not by copying the original's values.
- [ ] **Exit criterion:** it's fun with zero art.

### Phase 3: Art and audio direction
- [ ] Style guide: proportions, palette, court themes, UI.
- [ ] Concept art for 2–3 parody characters and one court, then one character in-engine.
- [ ] Base animations (run, dribble, shoot, dunk) plus custom trick animations.
- [ ] Original or licensed music and announcer.

### Phase 4: Vertical slice
- [ ] One court, 4–6 finished characters, full flow from menu to match to results.
- [ ] Use it for the trailer, demo and pitch material.

### Phase 5: Steam setup
- [ ] Steamworks account and Steam Direct fee.
- [ ] Store page once the slice looks good, to start collecting wishlists. No streamers' real names or images in marketing.
- [ ] AI-content disclosure if any generated assets ship.
- [ ] Demo for a Steam Next Fest.

### Phase 6: Full production and launch
- [ ] More courts, characters and modes (tournament, career, online later).
- [ ] Polish and playtesting.
- [ ] Marketing with short clips on TikTok, YouTube and X.
- [ ] Give the parodied streamers a friendly heads-up near launch.

---

## Tools

| Need | Tool |
|---|---|
| Emulator (research) | **PCSX2** 2.x, with your own disc dump |
| Extracting the ELF | **7-Zip** |
| Memory search, breakpoints | **PCSX2 debugger**, or **Cheat Engine** |
| Reading the code | **Ghidra** + **Emotion Engine extension** (ghidra-emotionengine-reloaded) |
| Explaining code | **REA** in Claude Code, or Claude with exported functions |
| Engine | **Godot** (free, no royalties) or **Unity** |
| Coding help | **Claude Code**, with Git + GitHub |
| 3D models | **Blender**; commission artists for hero characters |
| Animation | Blender, **Mixamo** for base motion; custom work for tricks |
| Textures and 2D | **Krita** or Photoshop, **Substance Painter** |
| Concept exploration | Generative tools (e.g. fal); disclose on Steam if any ship |
| Audio | **Reaper** or Audacity; commission or license music |
| Project tracking | **Todoist**, Trello or GitHub Projects |
| Release | **Steamworks** |
| Legal | Entertainment/IP lawyer familiar with Canadian and US law |
