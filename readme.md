# Resources for learning Godot for someone who already knows how to program

## Godot 2D Game Development Learning Path

A learning path for Godot 4.x 2D game development, aimed at someone who already knows Python. The language used throughout is **GDScript**, which is deliberately Python-like, so no C++ or C# is needed.

> **Note:** Make sure all tutorials you follow are for **Godot 4.x**. Many older resources cover Godot 3, which uses different syntax and node names.

---

## Phase 1: Get Oriented (about 1 week)

- [ ] Install Godot 4 (the standard version, not the .NET/C# build)
- [ ] Complete the official **"Your first 2D game"** tutorial at [docs.godotengine.org](https://docs.godotengine.org)
- [ ] Read the docs on **nodes and scenes** (the biggest mental shift from Python: games are built from small, reusable scenes made of nodes)
- [ ] Skim the GDScript reference, focusing on what differs from Python:
  - `var` and `func`
  - Optional static typing (`var speed: int = 200`)
  - `@export` and `@onready`
  - **Signals**

---

## Phase 2: Core 2D Skills (2-4 weeks)

Learn these by building tiny throwaway prototypes rather than only reading.

| Skill | Key nodes / concepts |
|-------|----------------------|
| Movement and input | `CharacterBody2D`, `Input` actions, `_physics_process` |
| Sprites and animation | `Sprite2D`, `AnimatedSprite2D`, `AnimationPlayer` |
| Collisions and physics | `Area2D`, collision layers and masks |
| Tilemaps | `TileMapLayer` |
| Signals | Godot's event system, used constantly |
| Cameras, UI, scene switching | `Camera2D`, `Control` nodes, `change_scene_to_file` |

### Recommended resources
- **GDQuest**: free tutorials, including the interactive "Learn GDScript From Zero" app
- **Brackeys**: Godot video series (verify it is for Godot 4)
- **HeartBeast** and **Chris' Tutorials**: well-regarded 2D content

---

## Phase 3: Build Small Complete Games (1-2 months)

Finishing games matters more than starting ambitious ones.

1. **Pong or Breakout**: input, collisions, scoring
2. **Simple platformer**: physics, tilemaps, enemies, pickups
3. **Top-down shooter or Zelda-like**: aiming, health, enemy AI, a basic state machine
4. **Small game with menus, save/load, and sound**: polish and game flow

Game jams such as **Godot Wild Jam** and **Ludum Dare** are great for forcing yourself to finish something.

---

## Phase 4: Level Up (ongoing)

- **Design patterns in Godot**
  - Autoloads (singletons)
  - Composition over inheritance
  - Custom `Resource` classes for data
  - State machines
- **Shaders** using Godot's shading language for visual effects
- **Export and publishing**: export to desktop or web and release on [itch.io](https://itch.io)
- **Study open-source projects** on GitHub to see how others structure their games

---

## Tips for Python Programmers

- Think of **scenes as objects**: a Player scene, an Enemy scene, a Bullet scene, instantiated as needed.
- Use **static typing** in GDScript for better autocomplete and earlier error detection.
- Use the **built-in docs** (press `F1` in the editor).
- Avoid building your own engine-like abstractions, since Godot already provides most of what you would write.
- Skip C# unless you later have a specific reason; community help and tutorials skew heavily toward GDScript.

