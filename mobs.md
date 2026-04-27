
| [Main Page](README.md)          | [Items](items.md)   | Mobs                | [Survival Systems](survival_systems.md) | [Vanilla Changes](vanilla_changes.md) |
| ----------------------------------- | ------------------- | ------------------- | --------------------------------------- | ------------------------------------- |
| [Beginner Guide](beginner_guide.md) | [Blocks](blocks.md) | [Bosses](bosses.md) | [Structures](structures.md)             | [Configuration](configuration.md)     |

# Mobs 
The datapack expands vanilla mobs with new variants, additional enemies, and a dynamic enhancement system. Mob behavior and strength scale with player progression, resulting in encounters that become progressively more difficult.

---
## Added Mobs
- [Nether Golem](mobs/nether_golem.md) 
- [Nether Shulker](mobs/nether_shulker.md) 
- [Zombie Brute](mobs/zombie_brute.md) 
---
## Mob Jockeys
Zombie Jockeys:
- Cave spider jockey
- Zombie Horseman

Husk Jockeys:
- Bunny jockey
- Husk Horseman
---
## Mob Enhancements
Mob Enhancements are part of the dynamic difficulty system, scaling hostile mobs based on player progression.

Each player has a **Difficulty Score** ranging from 1 to 5. This score increases over time and upon first entering the Nether. During a [Red Moon](miscellaneous/red_moon), the player’s difficulty is temporarily increased by 2.

When a mob spawns, it is assigned a **static difficulty level** based on the average Difficulty Score of the nearest three players within a 128-block radius. This value is fixed at spawn and determines the mob’s enhancements.

> There is no method for the player to find their difficulty score in survival. For those familiar with commands, the player difficulty scores are stored in the scoreboard `UH_player_difficulty`. You can bring it into view with `/scoreboard objectives setdisplay sidebar UH_player_difficulty` and remove it with `/scoreboard objectives setdisplay sidebar` 

---

==THIS PAGE IS A WORK IN PROGRESS==
> The exact enhancements are not documented. Zombies, Husks and Skeletons get armor, effects and weapons...

### Zombie
Base enhancements:
- Spawn with item in helmet slot which depends on the environment

| Helmet        | Environment                                 |
| ------------- | ------------------------------------------- |
| Dripleaf      | (default)                                   |
| Lilly pad     | Swamp biome                                 |
| Scaffolding   | Bamboo Jungle biome                         |
| Ice block     | Snowy biomes, standing on ice or snow block |
| Azalea leaves | Lush caves biome                            |

Scaling Enhancements:

| Difficulty | Effects |
| ---------- | ------- |
| 1          | -       |
| 2          | Speed 1 |
| 3          | Speed 1 |
| 4          | Speed 2 |
| 5          | Speed 2 |


### Squid
Base enhancements:
 - Attack the player when in close proximity and jump towards nearest player within 2.5 blocks
 - Latch onto players within 1 block. Latched squids apply wither effect and drag the player to the sea bed. A squid will never detach unless it is killed or the player is quickly moved away.

### Creeper 
==TODO==
Base enhancements:
- Jump towards nearby players
- Explodes if in proximity of player (within 3 block) for more than 3 seconds even without line of sight
- shorter fuse and larger explosion

### Skeleton
==TODO==
Base enhancements:
- switch between ranged and melee on nearest player proximity

### Spider
==TODO==
- They kill chickens
- Shoot spiderwebs at nearby players

### Piglin
==TODO==
- speed 1...

### Zombie Piglin
==TODO==
- speed 1...

### Zoglin
==TODO==
- Chance to spawn during a Red moons

### Zombie Villager
==TODO==
- Turn into Zombie Brute during a Red moon

### Ghast
==TODO==
- When a ghast is hurt and isnt killed, it will split into 5 Ghasts (which cannot split further).

### Wither Skeleton
==TODO==

### Wolf
==TODO==