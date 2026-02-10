
# Card Matching Memory Game (Unity)

A card matching memory game built in Unity with scalable layouts, animations, scoring, sound effects, and persistent progress saving.

---

## Features

- Smooth card flip and match animations  
- Continuous card flipping without waiting for card comparison  
- Dynamic grid layouts (2x2, 2x3, 5x6, etc.) with auto-scaling cards  
- Save & Load system to persist progress between sessions  
- Scoring system to track player performance  
- Sound effects for:
  - Card Flip  
  - Match  
  - Mismatch  
  - Game Over  
  - BG Music

---

## Technical Architecture

- **Scriptable Objects for Levels**
  - Level data (up to 10 levels) stored as Scriptable Objects
  - Each level supports different grid layouts
  - Easily editable and extendable without code changes

- **UI State Machine**
  - Used for UI pages (Main Menu, Gameplay, Game Over, etc.)
  - Designed for easy future page additions and UI flow modifications

- **Persistent Data Saving Using Local JSON**
  - User Data such as Cleared Levels and score has been writen in JSON and saved.
  - In Actual production, Either we can use Google play Games or Encrypt the JSON.

- **Audio System**
  - Audio Managed with help of separate Audio Manager Singleton for easy reach and single instance.
  - Audio Mixed used for overall audio control so in production, Easily add one more variable in JSON for Saving user music peferences.


---

## Tech Stack

- Unity Engine - 2021.3.45f2 LTS (As mention in assignment Doc)
- C#  

---

## How to Run

1. Clone the repository  
2. Open the project in Unity  
3. Open Assets/Scenes/Gameplay.unity
4. Press Play in the Unity Editor  

---

## Future Improvements

- Timer-based modes  
- Leaderboards  
- UI themes and animations  