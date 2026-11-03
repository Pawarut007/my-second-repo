# Simple Battle Simulator

This is a basic Python battle simulation between a heroic Knight and two enemies: a mischievous Goblin and a powerful Dragon.

The game demonstrates object-oriented programming principles such as classes, methods, and interaction between objects. It also includes a random damage system, where each attack deals between 30% and 90% of the character's initial attack power.

## File Structure

* `character.py`: Defines the `Character` class with attributes and methods for combat.
* `main.py`: Runs the battle simulation using one hero and two enemies.

## Character Class

Located in `character.py`, the `Character` class includes:

### Attributes

* `name` (str): The character's name.
* `hp` (int/float): Hit points (health).
* `attack_power` (int): The character's initial attack power.

### Methods

* `attack(other)`: Attacks another character and deals random damage between 30% and 90% of the character's initial attack power.
* `is_alive()`: Returns `True` if HP is greater than 0.
* `__str__()`: Returns a string representation of the character's current HP.

## How the Battle Works

The battle logic in `main.py` follows these steps:

1. Create three characters: Knight, Goblin, and Dragon.
2. Store both enemies in a list.
3. Print their initial stats.
4. Loop while the Knight is alive and at least one enemy is still alive:

   * Knight attacks each living enemy.
   * If an enemy survives, it attacks Knight back.
   * Print updated character stats.
5. The battle ends when Knight is defeated or both enemies are defeated.
6. Declare the winner.

## Running the Game

To run the simulation, execute `main.py`:

```bash
python main.py
```
