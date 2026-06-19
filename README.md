# ClimbGame — COMP602 Unity 3D Project

> A 3D puzzle-platformer built in Unity where players navigate environments, solve spatial puzzles, and overcome obstacles through climbing mechanics.

**Course:** COMP602 — Software Development Practice  
**Institution:** Auckland University of Technology (AUT)  
**Year:** 2024  
**Engine:** Unity 2022.3.43f1 LTS  
**Language:** C#

---

## About the Game

ClimbGame is a third-person 3D platformer built entirely from scratch in Unity. The player navigates a series of environments by climbing, jumping, and solving spatial challenges. The focus was on building solid game architecture — responsive controls, physics-driven collision, and a clean state machine to manage player behaviour.

---

## Features

- **Player controller** — smooth movement, jump, and climb mechanics built with Unity's physics engine
- **Collision detection** — context-aware surface detection for grounded, airborne, and climbable states
- **State machine architecture** — C# state machine managing player states (Idle → Run → Jump → Climb → Fall)
- **Environment design** — multi-level layout with obstacles, ledges, and climbable geometry
- **Camera system** — follow camera with smooth interpolation

---

## Tech Stack

| Tool | Version |
|---|---|
| Unity | 2022.3.43f1 LTS |
| C# | .NET Standard 2.1 |
| Unity URP | Universal Render Pipeline |
| Git | Version control via GitHub |

---

## Getting Started

### Prerequisites

- [Unity Hub](https://unity.com/download) with Unity **2022.3.43f1 LTS** installed
- Git

### Option 1 — Play the game

```bash
git clone https://github.com/All-Missing/COMP602_Project10_New.git
```

1. Open **Unity Hub** → click **Add** → navigate to the cloned folder
2. Select the `COMP602_Project10_New` folder and open the project
3. Inside the project, locate and launch `ClimbGame` to play

> **Tip:** The `Release` branch contains the final, submission-ready build.

### Option 2 — Open in Unity editor (development / testing)

```bash
git clone https://github.com/All-Missing/COMP602_Project10_New.git
```

1. Open Unity Hub → **Add** → select the `Project10` folder
2. Unity will import all assets automatically
3. Open the main scene and press **Play** in the editor

---

## Project Structure

```
COMP602_Project10_New/
└── Project10/
    ├── Assets/
    │   ├── Scripts/        # C# game logic (player controller, state machine, camera)
    │   ├── Scenes/         # Unity scenes
    │   ├── Prefabs/        # Reusable game objects
    │   └── Materials/      # URP materials and shaders
    ├── .gitignore
    └── .gitattributes
```

---

## Key Implementation Details

**State Machine (C#)**  
Player behaviour is managed through a finite state machine. Each state (Idle, Running, Jumping, Climbing, Falling) encapsulates its own input handling, physics interactions, and transition conditions — keeping game logic clean and extensible.

**Collision & Physics**  
Surface detection uses Unity's `Physics.Raycast` and `CharacterController` to distinguish ground, walls, and climbable surfaces, enabling context-sensitive responses without hardcoding per-object logic.

---

## Repository

- **Main branch:** development history (157 commits, 9 branches)
- **Release branch:** final submitted build

---

## Author

**Josh Ma** — [github.com/All-Missing](https://github.com/All-Missing)  
Bachelor of Computer and Information Sciences (BCIS), AUT — Major: Software Development
