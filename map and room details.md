# Dungeon Map and Room Details 

## Dungeon Map

```plaintext
      ┌────────┐     ┌────────┐     ┌────────┐
      │Entrance│────▶│ Room 1 │────▶│ Room 2 │
      └────────┘     └────────┘     └────────┘
          │              │              │
          ▼              ▼              ▼
      ┌────────┐     ┌────────┐     ┌────────┐     ┌───────┐
      │ Room 3 │────▶│ Room 4 │────▶│ Room 5 │────▶│  Exit │
      └────────┘     └────────┘     └────────┘     └───────┘
          │              │              │
          ▼              ▼              ▼
      ┌────────┐     ┌────────┐     ┌────────┐
      │ Room 6 │────▶│ Room 7 │────▶│ Room 8 │
      └────────┘     └────────┘     └────────┘
```
# Room Details

## Entrance
- **Description**: The starting point of your adventure. The air is cool, and the walls are damp.
- **Exits**: North to Room 1, South to Room 3.

## Room 1
- **Description**: A small, dimly lit room with old, moss-covered walls.
- **Exits**: North to Room 2, South to Room 4, East to Room 2.
- **Monsters**: None
- **Treasures**: None
- **Trap**: No

## Room 2
- **Description**: A larger room with a high ceiling and flickering torches on the walls.
- **Exits**: West to Room 1, South to Room 5.
- **Monsters**: Goblin (Health: 20, Attack Strength: 5)
- **Treasures**: None
- **Trap**: No

## Room 3
- **Description**: A narrow corridor that smells of mildew and decay.
- **Exits**: North to Entrance, East to Room 4, South to Room 6.
- **Monsters**: None
- **Treasures**: Health Potion (+10 Health)
- **Trap**: Yes (Health -10 if triggered)

## Room 4
- **Description**: A small room with a broken chest in the corner.
- **Exits**: North to Room 1, East to Room 5, South to Room 7, West to Room 3.
- **Monsters**: Skeleton (Health: 15, Attack Strength: 7)
- **Treasures**: Iron Sword (+5 Attack Strength)
- **Trap**: No

## Room 5
- **Description**: A brightly lit room with a fountain in the center.
- **Exits**: North to Room 2, West to Room 4, East to Exit.
- **Monsters**: None
- **Treasures**: None
- **Trap**: No

## Room 6
- **Description**: A damp and cold room with a puddle of water on the floor.
- **Exits**: North to Room 3, East to Room 7.
- **Monsters**: None
- **Treasures**: Gold Coin (x10)
- **Trap**: No

## Room 7
- **Description**: A room with old paintings on the walls, depicting unknown landscapes.
- **Exits**: North to Room 4, East to Room 8, West to Room 6.
- **Monsters**: Giant Rat (Health: 10, Attack Strength: 3)
- **Treasures**: None
- **Trap**: Yes (Health -5 if triggered)

## Room 8
- **Description**: A dusty room with cobwebs hanging from the ceiling.
- **Exits**: West to Room 7.
- **Monsters**: None
- **Treasures**: Magic Scroll (Increases Health by 20)
- **Trap**: No

## Exit
- **Description**: The exit of the dungeon, leading to the outside world.
- **Exits**: West to Room 5.
- **Monsters**: None
- **Treasures**: None
- **Trap**: No

## Usage

Students can use this dungeon map and room details to implement the dungeon crawler game. Each room should be represented as a `Room` object, and the connections between rooms should be managed using pointers or references to other `Room` objects. Students should ensure that the player can navigate through the dungeon, encounter monsters, collect treasures, and handle traps as specified.



