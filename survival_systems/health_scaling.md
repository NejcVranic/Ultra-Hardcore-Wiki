# Health
Health scaling is a [Survival System](../survival_systems.md) which scales player's max HP with their experience levels.

The player's experience level determines their max HP:
- Lvl 0-4 -> 2 health (1 heart) 
- Lvl 5-8 -> 16 health (2 hearts)
- Lvl 8-11 -> 6 health (3 hearts)
- Lvl 12-14 -> 8 health (4 hearts)
- Lvl 15-17 -> 10 health (5 hearts)
- Lvl 18-20 -> 12 health (6 hearts)
- Lvl 21-23 -> 14 health (7 hearts)
- Lvl 24-26 -> 16 health (8 hearts)
- Lvl 27-29 -> 18 health (9 hearts)
- Lvl 30+ -> 20 health (10 hearts)

> If you have another mod installed that changes or allows you to change max HP, it won't work as expected with this datapack, unless you disable this feature. Whenever your experience level interval changes your HP gets set to the static value documented above.
> If you disable max HP scaling with experience, the player's max HP will be set to 20 (10 hearts) and it won't be changed again, so it won't interfere with other mods / datapacks.