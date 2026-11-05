# 🧟 Zombie Smasher 3D

**A third-person, three-lane zombie endless runner built in Unity 6.6 with the Universal Render Pipeline (URP).**

Run through four post-apocalyptic worlds, dodge obstacles, outrun five kinds of zombies and grab power-ups while a pursuing horde chases you down.

Game Mechanics course project (23CS201PE407), School of Computer Science \& Artificial Intelligence, SR University.



## 🏆 Best run

|Theme|Distance|Score|
|-|-|-|
|🌲 Dense Zombie Forest|**845 m**|**2,654 points**|

\---

## ✨ Features

* **4 themed worlds**, each with its own scenery, 6 obstacle types, lighting, sky, fog, post-processing, music and ambience:

  * 🌲 **Dense Zombie Forest**: mud trail, fog and light shafts
  * 🏜️ **Desert**: cracked road, sandstorm and wrecked convoys
  * 🌃 **Spooky Dark City**: night, rain, neon and wet asphalt
  * 🏚️ **Abandoned City**: hazy ruins, fires and smoke columns
* **5 zombie types**: walkers, fast runners, brutes, hordes, and emergers that rise from the ground or step out of doorways.
* **Pursuing horde**: every stumble brings the horde right behind you for 6 seconds. Stumble again in that window and it catches you.
* **5 power-ups**: Magnet, Speed Boost, Shield, Double Coins and Health Protection.
* **Rising difficulty**: speed climbs from 11 to 25 m/s, and zombie density, zombie types and obstacle patterns scale with distance.
* **Scoring**: distance plus coins, a bonus every 500 m, and a saved best score per theme.
* **3 playable survivors**: Ranger, Medic and Mechanic.
* **Fully procedural content**: every model, texture, sound effect and music track is generated in code, so the project needs no third-party downloads.
* **One-click Setup Wizard** that builds the scenes, materials and build settings for you.
* **Performance work**: object pooling, chunk streaming, static mesh merging, a floating origin and Low / Medium / High / Auto quality tiers.

\---

## 🎮 Controls

|Action|Keyboard|Gamepad|Touch / mouse|
|-|-|-|-|
|Move left|A or ←|D-pad left|Swipe left|
|Move right|D or →|D-pad right|Swipe right|
|Jump|W, ↑ or Space|South button (A / Cross) or D-pad up|Swipe up|
|Slide (fast-fall in the air)|S or ↓|East button (B / Circle) or D-pad down|Swipe down|
|Pause|Esc or P|Start|Pause button on the HUD|

Jump and slide presses are buffered for 0.15 s, so a slightly early press still counts.

**How to survive:** jump over low obstacles, slide under high ones, and change lanes around full-height blocks. Hitting a low or high obstacle makes you stumble. Hitting a block or a zombie ends the run.

\---

## 📁 Repository structure

```
├── Assets/
│   └── ZombieRunner/
│       ├── Editor/          Setup Wizard (ZombieRunnerSetup.cs, ZRSetup.cs), ZRPlayModeInput.cs
│       ├── Resources/       ZRAssetRegistry.asset (created by the wizard)
│       ├── Scripts/
│       │   ├── Audio/         procedural sound and music synthesis, AudioManager
│       │   ├── Characters/    procedural humanoids, CharacterVisual
│       │   ├── Core/          themes, settings, scene flow, object pooling, RNG
│       │   ├── Environment/   chunk generator, prop factory, particle FX
│       │   ├── Gameplay/      player, input, spawner, zombies, power-ups, GameManager
│       │   ├── Rendering/     procedural textures, meshes, materials, lighting, quality
│       │   └── UI/            HUD and menus
│       ├── Scenes/          the six scenes
│       └── Imported/        optional third-party assets
├── Packages/                Unity package manifest (URP, uGUI, Input System)
├── ProjectSettings/         Unity project settings
├── docs/
│   ├── Zombie\_Smasher\_3D.pptx                  project presentation
│   ├── Zombie\_Smasher\_3D\_Project\_Report.pdf    project report
│   └── screenshots/                            gameplay screenshots
├── .gitignore               Unity .gitignore (Library/, Temp/, Logs/, Builds/ etc. are excluded)
└── README.md
```

## 👥 Team

|Hall ticket number|Role|
|-|-|
|2303A52429 |Team leader|
|2303A52431|Team member|
|2303A52155|Team member|
|2303A52314|Team member|

**Course:** Game Mechanics (23CS201PE407)
**Institution:** School of Computer Science \& Artificial Intelligence, SR University

\---

