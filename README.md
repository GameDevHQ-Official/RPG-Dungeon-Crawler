# RPG Dungeon Crawler

## Objective

Create a text-based RPG dungeon crawler in C++ where players navigate through different rooms using cardinal directions (North, South, East, West). Some rooms will contain monsters, some will be dead ends, and others may contain treasures or traps.

## Requirements

### Room Attributes

- Use a `struct` or `class` to define room attributes such as description, monsters, treasures, and connections to other rooms (North, South, East, West).
- Implement member functions to display and update room information.

### Player Attributes

- Use a `struct` or `class` to define player attributes such as health, inventory, and current location.
- Implement member functions to display and update player stats.

### Monster Attributes

- Use a `struct` or `class` to define monster attributes such as name, health, and attack strength.
- Implement member functions to display and update monster stats.
  
### Item Attributes

- Use a `struct` or `class` to define item attributes such as name
- Implement member functions to display item information.

### Actions

- Implement functions for actions such as moving between rooms, fighting monsters, collecting treasures, and encountering traps.

### Game Over Condition

- If the player’s health reaches zero, display a game over message and end the game.

## UML Design

### Room Class UML

```plaintext
+---------------------------------+
|             Room                |
+---------------------------------+
| - description: std::string      |
| - north: Room*                  |
| - south: Room*                  |
| - east: Room*                   |
| - west: Room*                   |
| - monsters: std::vector<Monster>|
| - treasures: std::vector<Item>  |
| - trap: bool                    |
+---------------------------------+
| + Room(description: std::string)|
| + displayInfo(): void           |
| + addMonster(monster: Monster): void |
| + addTreasure(item: Item): void |
+---------------------------------+
```

### Player Class UML

```plaintext
+---------------------------------+
|            Player               |
+---------------------------------+
| - health: int                   |
| - inventory: std::vector<Item>  |
| - location: Room*               |
+---------------------------------+
| + Player(health: int)           |
| + displayStats(): void          |
| + move(direction: std::string): void |
| + fight(monster: Monster): void |
| + collectTreasure(item: Item): void |
| + encounterTrap(): void         |
+---------------------------------+
```

### Monster Class UML

```plaintext
+---------------------------------+
|            Monster              |
+---------------------------------+
| - name: std::string             |
| - health: int                   |
| - attackStrength: int           |
+---------------------------------+
| + Monster(name: std::string, health: int, attackStrength: int) |
| + displayInfo(): void           |
| + attack(player: Player): void  |
+---------------------------------+
```

### Item Class UML

```plaintext
+---------------------------------+
|              Item               |
+---------------------------------+
| - name: std::string             |
| - effect: std::string           |
+---------------------------------+
| + Item(name: std::string, effect: std::string) |
| + displayInfo(): void           |
+---------------------------------+
```

# Steps

### 1. Set Up Project
- Create a new C++ project and set up your development environment.
- Include necessary headers (`<iostream>`, `<vector>`, `<string>`).

### 2. Define Room Class
- Create a Room class with attributes: `description`, `north`, `south`, `east`, `west`, `monsters`, `treasures`, and `trap`.
- Implement member functions to display and update room information.

### 3. Define Player Class
- Create a Player class with attributes: `health`, `inventory`, and `location`.
- Implement member functions to display and update player stats.

### 4. Define Monster Class
- Create a Monster class with attributes: `name`, `health`, and `attackStrength`.
- Implement member functions to display and update monster stats.

### 5. Define Item Class
- Create an Item class with attributes: `name` and `effect`.
- Implement member functions to display item information.

### 6. Implement Player Actions
- Implement functions for moving between rooms, fighting monsters, collecting treasures, and encountering traps.

### 7. Implement Game Logic
- Implement the main game loop where players can choose actions such as moving, fighting, collecting treasures, and encountering traps.
- Include a game over condition if the player’s health reaches zero.

## Example User Interaction

```plaintext
*****************************************************************
*                       Dungeon Crawler                         *
*****************************************************************

You are in a dark room. Exits are to the North and East.

Enter 'n' to go North, 'e' to go East, 's' to go South, 'w' to go West: n
You enter a room with a monster!

Monster Stats:
- Name: Goblin
- Health: 20
- Attack Strength: 5

Enter 'f' to fight, 'r' to run: f
Fighting the Goblin...
You defeated the Goblin! Your health decreased by 5.

Your Stats:
- Health: 95
- Inventory: None

You are in a room with a dead goblin. Exits are to the South.

Enter 'n' to go North, 'e' to go East, 's' to go South, 'w' to go West: s
You are back in the dark room. Exits are to the North and East.

Enter 'n' to go North, 'e' to go East, 's' to go South, 'w' to go West: e
You enter a room with a treasure chest!

Enter 'o' to open the chest: o
You found a health potion! Health increased by 10.

Your Stats:
- Health: 105
- Inventory: Health Potion

You are in a room with an open treasure chest. Exits are to the West.

Enter 'n' to go North, 'e' to go East, 's' to go South, 'w' to go West: w
You are back in the dark room. Exits are to the North and East.

Enter 'n' to go North, 'e' to go East, 's' to go South, 'w' to go West: q
*****************************************************************
*                      Thanks for playing!                      *
*****************************************************************
```
## Submission Details

### 1. Complete the project and ensure it is bug-free.

### 2. Add the completed project to your GitHub repository.

### 3. Submit the link to your repository through your program dashboard to continue the program.

### 4. A code review will be processed once the submission is received.




