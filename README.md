# Minecraft Projects — Screenshot Proofs

Screenshots from commercial Minecraft projects I built as a Java developer at
[cristalix.gg](https://cristalix.gg) between 2017 and 2022, and from a 2025 project. The source
code of these projects is private, so these photos are the proof of the work: minigames, custom
rendering, procedural generation and server-side optimization.

| Project | Years | What it is |
| --- | --- | --- |
| [ZombieMod](#zombiemod) | 2017 | Humans vs zombies survival minigame |
| [ColorControl](#colorcontrol) | 2018 | Team minigame |
| [SkyBlock](#skyblock) | 2021 | Procedurally generated dungeons and custom item systems |
| [HitTheMobs](#hitthemobs) | 2019–2022 | Mob arena with hundreds of configurable mobs per location |
| [Steal Brainrot](#steal-brainrot) | 2025 | Brainrot-stealing server with custom NPCs and shops |

---

## ZombieMod

*2017 · survival minigame (humans vs zombies)*

Rounds of infection gameplay with custom mob models, an in-game economy and leaderboards. The
leaderboard holograms were drawn with custom OpenGL code on top of NMS instead of the vanilla
scoreboard.

<img src="photos/zombiemod-2017-08-10.jpg" alt="ZombieMod gameplay with a custom-model zombie boss" width="900">

<img src="photos/zombiemod-with-custom-render-opengl-2017-12-06.jpg" alt="ZombieMod custom OpenGL leaderboard" width="900">

Custom OpenGL-rendered leaderboard hologram above the map (top players by balance) and the player
profile sidebar (group, balance, XP, online).

---

## ColorControl

*2018 · team minigame*

The minigame ran behind multiple BungeeCord proxies, with players distributed into teams and
moved between servers automatically.

<img src="photos/colorcontrol-2018-04-27.jpg" alt="ColorControl development debug screenshot" width="900">

Here I was testing synchronisation between multiple BungeeCord proxies.

<img src="photos/colorcontrol-2018-05-12.jpg" alt="ColorControl match start" width="900">

Match start: players joining, automatic team distribution and the start of the round on a colored
arena.

---

## SkyBlock

*2021 · ASkyBlock mechanics: procedural dungeons and custom items*

The SkyBlock world and its mechanics ran at up to 400 concurrent players on a single core after
profiling and optimization.

<img src="photos/procedural dungeon generation for skyblock-2021-08-02.jpg" alt="Generated dungeon layout, top-down view" width="700">

Top-down dump of a generated dungeon layout: connected rooms and caves produced by the procedural
generator.

<img src="photos/procedural dungeon generation  for skyblock-2021-08-29.jpg" alt="Generated dungeon corridor in game" width="900">

The same generator in game: a generated corridor with lanterns, mossy and cracked stone bricks and
iron-bar gates.

<img src="photos/skyblock-image-lore-2021-10-26.jpg" alt="Custom SkyBlock item GUI with requirements" width="700">

Custom item GUI: an item's upgrade chain with its rank and crafting requirements (collection
level, resources), implemented as a custom inventory UI.

---

## HitTheMobs

*2019–2022 · mob arena with many small locations*

Every location holds a large number of mobs whose stats are fully configurable through JSON
configs stored in git — game content is data, not code.

<img src="photos/hitthemobs-2019-03-22.jpg" alt="HitTheMobs hub" width="900">

The game hub: profile sidebar (level, XP, balance, skills), XP leaderboard, shops and NPCs.

<img src="photos/hitthemobs-2021-11-11.jpg" alt="HitTheMobs arena full of mobs" width="900">

An arena packed with mobs; chat shows activated boosters (Vitality, double money) and the sidebar
shows profile progress.

<img src="photos/hitthemobs-optimization-2022-02-17.jpg" alt="HitTheMobs stress test with stable TPS" width="900">

Stress test: hundreds of mobs on a single location while the server stays at 20.0 TPS (1m / 5m /
15m in the debug overlay) — the result of profiling and optimizing the server.

<img src="photos/hitthemobs-optimization-2022-02-18.jpg" alt="HitTheMobs custom-model mob wave" width="900">

Using custom NMS patches to spawn an EntityPlayer as a regular mob — still at 20 TPS.

---

## Steal Brainrot

*2025 · brainrot-stealing server*

Players steal meme characters from each other's bases while the owners try to defend them.

<img src="photos/steal-brainrot-2025-12-17.jpg" alt="Steal Brainrot base with custom NPC displays and prices" width="900">

A base area: custom character models with floating name tags and prices above them, alongside
players, pets and a profile overlay.

<img src="photos/steal-brainrot-2025-12-29.jpg" alt="Steal Brainrot fenced enclosure with slot platforms" width="900">

A fenced enclosure with slot platforms for placing characters.

---

*Screenshots are from private projects; the code is not public.*
