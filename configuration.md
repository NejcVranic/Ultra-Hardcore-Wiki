
| [Main Page](README.md)          | [Items](items.md)   | [Mobs](mobs.md)     | [Survival Systems](survival_systems.md) | [Vanilla Changes](vanilla_changes.md) |
| ----------------------------------- | ------------------- | ------------------- | --------------------------------------- | ------------------------------------- |
| [Beginner Guide](beginner_guide.md) | [Blocks](blocks.md) | [Bosses](bosses.md) | [Structures](structures.md)             | **Configuration**                     |

# Configuration
You can change the datapack's settings by using the scoreboard commands on below.
> Just go to your world and enter one of these command in the chat to change the settings. 
> (You need to have cheats enabled to use commands.)

Each setting uses a value. UNLESS SPECIFIED otherwise, the only allowed values are 0 and 1. 
- 0 = FEATURE DISABLED
- 1 = FEATURE ENABLED

<span style="color:rgb(255, 0, 0)">! WARNING !</span> 
After changing settings you need to RELOAD the datapack for the changes to take effect!
When the datapack is reloaded, it's active settings can be viewed by clicking the blue text written in chat.
> Datapacks can be reloaded by using `/reload` command.

> Examples:
> `/scoreboard players set hp_scales_with_experience UH_player_settings 0` - disable HP scaling with experience
> `/scoreboard players set natural_regeneration UH_player_settings 1` - enable natural regeneration
> `/scoreboard players set game_difficulty UH_player_settings 0` - sets game difficulty to PEACEFUL

---

### Health
HP SCALES WITH EXPERIENCE: Max health scales with experience levels
- command: `/scoreboard players set hp_scales_with_experience UH_player_settings <VALUE>`

NATURAL REGENERATION: Determines if natural generation is enabled.
- command: `/scoreboard players set natural_regeneration UH_player_settings <VALUE>`


### Punching blocks
PUNCHING LOGS WITHOUT AXE HURTS PLAYER
- command: `/scoreboard players set punching_wood_hurts UH_player_settings <VALUE>`

PUNCHING STONE WITHOUT PICKAXE HURTS PLAYER
- command: `/scoreboard players set punching_stone_hurts UH_player_settings <VALUE>`

PUNCHING CACTUS WITH EMPTY HAND HURTS PLAYER
- command: `/scoreboard players set punching_cactus_hurts UH_player_settings <VALUE>`


### Survival systems
HEAT SYSTEM: freeze during night if you have no suitable armor
- command: `/scoreboard players set heat_system UH_player_settings <VALUE>`

HYDRATION SYSTEM: Low hydration causes punishments. Disabling will also hide the bossbar.
- command: `/scoreboard players set hydration_system UH_player_settings <VALUE>`

INSANITY SYSTEM: Higher insanity causes more punishments
- command: `/scoreboard players set insanity_system UH_player_settings <VALUE>`

NUTRITION SYSTEM: Eating food impacts your nutrition stats. Your diet can have positive or negative effects.
- command: `/scoreboard players set nutrition_system UH_player_settings <VALUE>`

WOUND SYSTEM: Getting injured has a chance of leaving progressively worse wounds. Falling from heights can break your leg. 
- command: `/scoreboard players set wound_system UH_player_settings <VALUE>`


### Difficulty & Enhancements
GAME DIFFICULTY: Determines the game difficulty 
- in singleplayer you can also change this in game menu -> options -> difficulty, but it is reset on datapack reload
- ALLOWED VALUES: 0 = PEACEFUL, 1 = EASY, 2 = NORMAL, 3 = HARD
- command: `/scoreboard players set game_difficulty UH_player_settings <VALUE>`

BOSS ENHANCEMENTS: Enderdragon and Wither enhancements
- command: `/scoreboard players set mob_enhancements UH_player_settings <VALUE>`

MOB ENHANCEMENTS: Allow mob enhancements. 
- Disabling will completely disable all enhancements. (You can also disable individual mob enhancements instead)
- command: `/scoreboard players set mob_enhancements UH_player_settings <VALUE>`

SCALING MOB DIFFICULTY: Mob difficulty increases as players progress
- command: `/scoreboard players set scaling_mob_difficulty UH_player_settings <VALUE>`

Zombie enhancements 
- command: `/scoreboard players set zombie_enhancements UH_player_settings <VALUE>`

Skeleton enhancements 
- command: `/scoreboard players set skeleton_enhancements UH_player_settings <VALUE>`

Creeper enhancements 
- command: `/scoreboard players set creeper_enhancements UH_player_settings <VALUE>`

Spider enhancements 
- command: `/scoreboard players set spider_enhancements UH_player_settings <VALUE>`

Enderman enhancements (auto agro on proximity if player has high insanity)
- command: `/scoreboard players set enderman_enhancements UH_player_settings <VALUE>`

Slime enhancements 
- command: `/scoreboard players set slime_enhancements UH_player_settings <VALUE>`

Wither skeleton enhancements 
- command: `/scoreboard players set wither_skeleton_enhancements UH_player_settings <VALUE>`

Ghast enhancements
- command: `/scoreboard players set ghast_enhancements UH_player_settings <VALUE>`

Squid enhancements 
- command: `/scoreboard players set squid_enhancements UH_player_settings <VALUE>`

Wolf enhancements 
- command: `/scoreboard players set wolf_enhancements UH_player_settings <VALUE>`

Chance for Zoglin to spawn in overworld
- command: `/scoreboard players set spawn_zoglin_in_overworld UH_player_settings <VALUE>`

Chance for Zombie Brute to spawn instead of zombie during red moon
- command: `/scoreboard players set spawn_zombie_brute UH_player_settings <VALUE>`

Chance for zombie cave spider jockey to spawn instead of zombie
- command: `/scoreboard players set spawn_zombie_jockey UH_player_settings <VALUE>`

Chance for zombie horseman to spawn instead of zombie
- command: `/scoreboard players set spawn_zombie_horseman UH_player_settings <VALUE>`

Chance for nether golem to spawn instead of wither skeleton
- command: `/scoreboard players set spawn_nether_golem UH_player_settings <VALUE>`

Chance for nether shulker to spawn instead of piglin
- command: `/scoreboard players set spawn_nether_shulker UH_player_settings <VALUE>`

Chance for camel jockey to spawn instead of husk
- command: `/scoreboard players set spawn_husk_camel_jockey UH_player_settings <VALUE>`

Chance for rabbit jockey to spawn instead of husk
- command: `/scoreboard players set spawn_husk_rabbit_jockey UH_player_settings <VALUE>`


### Other
WITHERED SOIL: Withered soil spreads from neighboring blocks and players who have been infected with wither effect
- command: `/scoreboard players set withered_soil UH_player_settings <VALUE>`

TOGGLEABLE WEATHER: Blowing a goat horn while wearing a pumpkin on your head can change the weather
- command: `/scoreboard players set toggle_weather_w_goat_horn UH_player_settings <VALUE>`

ANIMAL CROWDING: Animals take random crowding damage if they are too close to each other
- command: `/scoreboard players set animal_crowding UH_player_settings <VALUE>`

ANIMAL REVENGE: When you hurt a cow or horse they hurt you back
- command: `/scoreboard players set animal_revenge UH_player_settings <VALUE>`
