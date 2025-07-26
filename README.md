# Text-Based Adventure Game

## Description
This is a text-based adventure game built in Python. It was one of my first projects in University. In this game, you explore diverse locations—from the Village to Dark Mines—and encounter enemies, puzzles, and NPCs. Your choices influence the outcome of the story, and you can interact with various items and characters along your journey.

## Features
- **Exploration:** Traverse multiple interconnected rooms and landscapes such as forests, lakes, and mines. See details and descriptions provided in [`map.py`](map.py) and the map visuals in [`mapa.txt`](mapa.txt).
- **Combat System:** Engage in dynamic battles using different weapons as implemented in [`combat.py`](combat.py) and detailed enemy configurations in [`enemies.py`](enemies.py).
- **Puzzles & Interactions:** Solve puzzles (see [`puzzles.py`](puzzles.py)) and interact with NPCs (see [`npcs.py`](npcs.py)) to receive quests and backstory.
- **Item Management:** Collect, inspect, and use items from your inventory. Check out [`items.py`](items.py) for item details and behavior.
- **Text Parsing:** Enjoy an immersive experience with a custom command parser defined in [`gameparser.py`](gameparser.py).

## How to Play
1. **Start the Game:** Run the game by executing the main file:
    ```sh
    python game.py
    ```
2. **Gameplay:**  
    - **Movement:** Use the `GO` command followed by a direction (e.g., `GO north`).
    - **Interacting with Objects:** Use `LOOK`, `INSPECT`, or `EXAMINE` commands to interact with items, NPCs, and surroundings.
    - **Combat:** When encountering enemies, use combat commands such as `ATTACK LIGHT` or `ATTACK HEAVY` as described in the combat tips from [`combat.py`](combat.py).
    - **Other Commands:**  
        - `TALK` to converse with NPCs.
        - `OPEN` to access doors (e.g., in the cabin or shack).
        - `USE` to interact with an item in your inventory.
        - `READ MAP` to view the game's map (requires the map item in your inventory).
        - `SPEAK` to vocalize a phrase that can affect the game world.
        - `HELP` for a list of available commands.

## File Structure
- **Gameplay & Logic:**  
  - [`game.py`](game.py) – Main game loop and overall gameplay management.
  - [`gameparser.py`](gameparser.py) – Functions to process and normalize user input.
- **World & Environment:**  
  - [`map.py`](map.py) – Data for the rooms and their connections.
  - [`mapa.txt`](mapa.txt) – ASCII map visualization.
  - [`surroundings.py`](surroundings.py) – Additional descriptions for in-game environmental features.
- **Items & Interactions:**  
  - [`items.py`](items.py) – Definitions for items available in the game.
  - [`puzzles.py`](puzzles.py) – Puzzle scenarios within the game world.
- **Characters & Enemies:**  
  - [`npcs.py`](npcs.py) – Non-player character definitions and dialogues.
  - [`enemies.py`](enemies.py) – Enemy definitions and stats.
- **Combat & Endings:**  
  - [`combat.py`](combat.py) – The combat system.
  - [`ending.py`](ending.py) – Various game endings based on your performance.
- **Player:**  
  - [`player.py`](player.py) – Player attributes, inventory, and status.

## Requirements
- Python3

## Running the Game
To start your adventure, run:
```sh
python game.py
```
