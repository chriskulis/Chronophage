# CHRONOPHAGE — The Time Devourer

![Three.js](https://img.shields.io/badge/Three.js-black?style=for-the-badge&logo=three.js&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![Web Audio API](https://img.shields.io/badge/Web_Audio_API-4285F4?style=for-the-badge&logo=google-chrome&logoColor=white)

> *A stylized 3D arena combat game where you are the last Guardian of the Temporal Sanctum, fighting against clock-like abominations that seek to devour all of time itself.*

---

## 🎮 Play Now

Simply open `index.html` in any modern browser. No installation required.

---

## 📖 Story

You are the **Last Guardian**, protector of the Temporal Sanctum — the place where all of time converges. The **Chronophages** have breached the sanctum walls. These twisted clock abominations feed on temporal energy, and they hunger for the moments that make up your existence.

Your sword is infused with crystallized time. Each strike steals seconds from your enemies. Build your temporal charge, unleash devastating time-manipulation abilities, and survive wave after wave of increasingly deadly foes.

**Time is your weapon. Time is your enemy. Time is running out.**

---

## 🕹️ Controls

| Action | Key |
|--------|-----|
| **Move** | W A S D |
| **Look / Aim** | Mouse |
| **Light Attack** | Left Mouse Button |
| **Heavy Attack** | Right Mouse Button |
| **Dash** | Space |
| **Sprint** | Shift (hold) |
| **Time Fracture** | Q (requires charge) |
| **Temporal Echo** | E (requires charge) |
| **Chronostasis** | R (requires full charge) |
| **Pause** | Escape |

---

## ⚔️ Combat System

### Basic Combat

- **Light Attack** — Fast sword swing. Low damage, quick recovery. Chain up to 3 hits.
- **Heavy Attack** — Slow but devastating overhead slam. Can be charged for AOE damage.
- **Dash** — Quick dodge with invincibility frames. Essential for survival.

### Stamina

All actions consume stamina. Manage it carefully:
- Light attacks: 12 stamina
- Heavy attacks: 30 stamina
- Dash: 25 stamina
- Sprint: 20/second

Stamina regenerates when not performing actions.

### Temporal Charge

Landing hits and killing enemies builds **Temporal Charge**. Higher charge levels unlock:

| Charge | Effect |
|--------|--------|
| 25% | +10% damage, blade glows brighter |
| 50% | +20% damage, attacks have small AOE |
| 75% | +30% damage, attacks leave lingering hitboxes |
| 100% | +50% damage, unlock Temporal Abilities |

### Temporal Abilities

- **Q — Time Fracture**: Create a zone that slows enemies by 70%
- **E — Temporal Echo**: Summon a ghost that mimics your attacks
- **R — Chronostasis**: Freeze time completely for 3 seconds (ultimate)

---

## 👾 Enemies

### Tick (Common)
*Fragments of broken pocket watches, animated by temporal corruption.*

- Spider-like clock creature
- Skitters toward you, lunges to attack
- **Tell**: Rears back before lunging
- **Points**: 100

### Tock (Flanker)
*Twin spirits bound to a grandfather clock's mechanism.*

- Two clock faces connected by brass spine
- Circles you, teleports, attacks in rapid combos
- **Tell**: Both faces lock to 6 o'clock
- **Points**: 200

### The Grandfather (Boss)
*A grandfather clock that witnessed centuries of death.*

- Massive walking grandfather clock
- Sweeping arm attacks, ground slams, arena-wide shockwave
- **Tell**: Arms raise, clock face glows
- **Points**: 1000

### The Pendulum (Ranged)
*The soul of a metronome, eternally counting beats.*

- Floating inverted pendulum
- Fires projectiles, creates buff zones for other enemies
- **Tell**: Pendulum freezes before firing
- **Points**: 300

### The Second Hand (Assassin)
*It exists in the moment when clock hands align at midnight.*

- Humanoid made of clock hands
- Silent, stalks you, strikes in rapid 3-hit combos
- **Tell**: Almost none — stay alert
- **Points**: 500

### Chronophage Prime (Final Boss)
*The source of corruption. A being from the end of time.*

- Massive fusion of all clock types
- Multiple attack phases
- **Kill it before the Final Toll countdown ends**
- **Points**: 10000

---

## 🌊 Wave System

| Wave | Enemies |
|------|---------|
| 1-2 | Ticks only (warmup) |
| 3-4 | Ticks + Tocks |
| 5 | **Boss: The Grandfather** |
| 6-7 | Mixed + Pendulums |
| 8-9 | All types + Second Hand |
| 10 | **Boss Wave** |
| 11-14 | Escalating difficulty |
| 15 | **CHRONOPHAGE PRIME** |

Between waves:
- 6 second rest
- 25% health regeneration
- Temporal charge restored

---

## 🏆 Scoring

- Base points per enemy × combo multiplier = score
- Combo builds with consecutive hits
- Getting hit resets combo
- Collect **Temporal Motes** (golden particles from kills) to extend combo timer

**Combo Multipliers:**
| Hits | Multiplier |
|------|------------|
| 0-9 | 1.0x |
| 10-24 | 1.5x |
| 25-49 | 2.0x |
| 50-99 | 3.0x |
| 100+ | 5.0x |

---

## 🛠️ Technical Details

### Built With

- **Three.js** — 3D rendering
- **Web Audio API** — Procedural sound generation
- **Vanilla JavaScript** — Game logic
- **Single HTML file** — No build process required

### Requirements

- Modern browser (Chrome, Firefox, Edge, Safari)
- WebGL support
- Keyboard + Mouse

### Performance

Target: 60 FPS

The game uses:
- Object pooling for particles
- Efficient shadow mapping
- Frustum culling
- Optimized geometry

---

## 📁 Project Structure

```
chronophage/
├── index.html          # The entire game (single file)
├── README.md           # You're reading it
└── screenshots/        # (optional) Game screenshots
```

---

## 🎨 Art Direction

- **Style**: Art deco meets cosmic horror
- **Palette**: Deep blues, gold/brass, white energy, void black
- **Motifs**: Clocks, gears, roman numerals, pendulums
- **Mood**: Eerie, otherworldly, the beauty of precision corrupted

---

## 🔊 Audio

All sounds are procedurally generated using Web Audio API:

- Metallic sword swings with temporal energy sizzle
- Mechanical enemy sounds (ticking, chiming, grinding)
- Satisfying impact feedback
- Dynamic ambient audio that scales with combat intensity

---

## 🚀 Development

### Vibe Coded

This game was created using **vibe coding** — AI-assisted development where the human provides creative direction and the AI generates implementation.

**Tools used:**
- Claude (Anthropic) for game design and code generation
- Three.js documentation
- Lots of iteration and playtesting

### Future Ideas (V2)

- [ ] Third-person follow camera (improved controls)
- [ ] Difficulty modes (Easy/Normal/Hard/Nightmare)
- [ ] Health regeneration system
- [ ] Weapon switching (sword, pistol, scythe)
- [ ] Enhanced post-processing (bloom, chromatic aberration)
- [ ] Upgraded HUD with custom fonts
- [ ] Dynamic music system

---

## 🐛 Known Issues

- Floor details may flicker during attacks (z-fighting)
- Camera can be disorienting in intense combat
- Performance may vary on integrated graphics

---

## 📜 License

This project is open source. Feel free to learn from it, modify it, and create your own versions.

---

## 🙏 Acknowledgments

- **Three.js** team for the incredible 3D library
- **Andrej Karpathy** for coining "vibe coding"
- Everyone pushing the boundaries of AI-assisted game development

---

## 📸 Screenshots

*Coming soon*

---

<div align="center">

**⏱️ TIME IS RUNNING OUT ⏱️**

*Can you survive the Chronophage?*

</div>
