# 🎮 Unreal Engine II – Game Design & Blueprint Practice

This repository contains a level design project created using **Unreal Engine 5**, focused on the use of **Blueprints** and the implementation of basic interactive mechanics within a first-person experience.

---

## 🧠 Project Objective

The goal of this practice is to apply **game design fundamentals** by prototyping a functional blockout using visual scripting in Unreal Engine. Emphasis is placed on modular design, clear logic through Blueprints, and a readable visual language.

---

## 🧱 Implemented Mechanics

### 🐱 Cat POV & Navigation
- First-person controller simulating the point of view of a cat.
- Character size, movement speed, and camera adjusted for feline scale.
- Collisions fine-tuned for navigating small spaces.
- Gravity and jump settings configured to simulate agile cat-like movement.

### 💡 Blueprint 1 – Light Switch
- A light changes when the player enters a trigger zone (Box Collision).
- Material changes to an emissive instance while inside the zone.
- Uses `OnComponentBeginOverlap` and `Cast To` for logic.

### 🚪 Blueprint 2 – Directional Door
- A door opens based on the player's approach direction.
- Controlled via `Timeline` and relative rotation.
- Direction calculated using vector math (`Actor Forward Vector`, `Normalize`, `==`).
- Interaction managed with `CanInteract` and `Direction` booleans.

---

## 🔷 Visual Design Language

A **color code** was used to define each area of the level and its purpose:

| Color           | Meaning                      |
|------------------|-------------------------------|
| 🟤 Brown         | Walkable surfaces              |
| 🔴 Red           | Entry/exit points               |
| 🔵 Blue          | Doors                  |
| 🟡 Green         | Structural elements            |
| ⚪ White         |  Floor             |

This approach improves level readability and supports rapid design iteration.

---

## 📐 Game Mode & Player Setup

- Custom `GameMode` (`BP_FirstPersonGameMode`)
- First-person character setup: `BP_FirstPersonCharacter_Cat`
- Camera FOV adjusted for a low POV (cat perspective)
- Collision capsule size reduced to navigate tight spaces
- Post-processing for stylized look (bloom, color grading, vignette)

---

## 🔥 Build & Delivery

- Project packaged and ready to run on Windows

