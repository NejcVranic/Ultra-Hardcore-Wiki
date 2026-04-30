# Frost
Frost is a [Survival System](../survival_systems.md) which adds conditions for freezing.

At night, the player will begin freezing if none of the following criteria is met:
- Player is wearing a piece of leather armor
- Player is wearing 4 pieces of armor
- Player is standing next to a source of heat
- Player's head is not in an air block (unintended)

Sources of heat include:
- lit campfire, soul campfire and [chiseled campfire](../blocks/chiseled_campfire.md),
- active furnace,
- Lava and
- Fire

The game checks for sources of heat within 3 blocks on the horizontal (XZ) plane and 2 blocks on the vertical (Y) axis.

> The datapack checks these conditions only every 2.5 seconds. Because of this there might be a short delay before a change is detected. 