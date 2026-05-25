# Frost
Frost is a [Survival System](../survival_systems.md) which adds conditions for freezing.

At night, the player will begin freezing if none of the following criteria is met:
- Player is wearing a piece of leather armor
- Player is wearing 4 pieces of armor
- Player is standing next to a source of heat
- Player's head is not in an air block (unintended)

> This mechanic has a side effect: a freezing players head will destroy blocks it is inside of. This is because there is no way to give the freezing effect to a player - instead, a powdered snow black is placed and destroyed every tick at the players location. (For example a freezing player will break an open door if the walk through it.) Normally the set powdered block would be visible and prevent the player from interacting with the world, but there exists a workaround by using a tick advancement. Another side effect of this is that the player can obtain powdered snow if they use a bucket while freezing.

Sources of heat include:
- lit campfire, soul campfire and [chiseled campfire](../blocks/chiseled_campfire.md),
- active furnace,
- Lava and
- Fire

The game checks for sources of heat within 3 blocks on the horizontal (XZ) plane and 2 blocks on the vertical (Y) axis.

> The datapack checks these conditions only every 2.5 seconds. Because of this there might be a short delay before a change is detected. 