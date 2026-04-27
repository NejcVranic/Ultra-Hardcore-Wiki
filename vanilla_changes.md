
| [Main Page](README.md)          | [Items](items.md)   | [Mobs](mobs.md)     | [Survival Systems](survival_systems.md) | Vanilla Changes                   |
| ----------------------------------- | ------------------- | ------------------- | --------------------------------------- | --------------------------------- |
| [Beginner Guide](beginner_guide.md) | [Blocks](blocks.md) | [Bosses](bosses.md) | [Structures](structures.md)             | [Configuration](configuration.md) |

# Vanilla Changes 
Below is a complete list of changes to Vanilla Minecraft introduced by Ultra Hardcore. 

## Recipes
Removed recipes:
- White and gray carpet (replaced by [Knitten Fabric](./items/knitten_fabric.md) and [Mattress](./items/mattress.md))
- Wooden and stone tools 
- Iron armor (replaced by [Steel](./material_tiers/steel_tier.md) armor)
- Gold armor & tools (replaced by [Blaze Gold](./material_tiers/blaze_gold_tier.md) armor & tools)
- Diamond armor & tools (must be forged in a [Deepslate Forge](./blocks/deepslate_forge.md) or [Nether Forge](./blocks/nether_forge.md))
- Diamond armor & tools cannot be upgraded to [Netherite](./material_tiers/netherite_tier.md) in a smithing table (Netherite items must be forged in [Nether Forge](./blocks/nether_forge.md))

Added recipes:
- Dirt, crafted from 4 brown dye
- Wooden planks, crafted from 4 wooden buttons of the same type
- Chainmail armor, crafted with with chains in standard armor recipe shapes
- [Trident](./items/trident.md), crafted with heart of the sea, iron and lightning rod
- Saddle
- Name tag
- stick, crafted from any sapling 
- cobblestone, crafted from 4 buttons
- [Experience Bottle](./items/experience_bottle.md) 
- bowl, crafted with 1 planks + flint

Changed recipes:
- [Beds](./blocks/beds.md) (3 mattresses are now required as well)
- [Campfire](./blocks/campfire.md) 
- [Chest](./blocks/chest.md) 
- [Crafting Table](./blocks/crafting_table.md) 
- [Eye of Ender](./items/eye_of_ender.md)
- [Furnace](./blocks/furnace.md) 
- [Loom](./blocks/loom.md) 
- [Torch](./items/torch.md) (Vanilla Torch recipe now crafts [Unlit Torch](./items/unlit_torch.md))
- Smelting raw iron in a furnace produces an iron nugget (but when using a blasting furnace you still get an iron ingot)

 Added [Campfire](./blocks/campfire.md) recipes:
- Clay ball -> Brick
- Wooden log -> Charcoal
- Stick -> -nothing- (used only to fuel [Chiseled Campfire](./blocks/chiseled_campfire.md))

---

## Loot tables
- Shipwreck storage: 60% chance to find Ocean Monument map
- Treasure: Removed iron and increased other loot, added enchanted books with Trident-specific enchants 

---

## Mining & block breaking
- Punching wood, stone & cactus hurts
- Grass and dirt blocks drop brown dye when mined without using a shovel
- Mining a log with a wooden axe or a stone axe will drop items and replace the block with a fence of the same wood type
- Wooden log drop loot depends on the type of axe used:
	- flint hatchet (`minecraft:wooden_axe`): wooden button
	- copper, iron & steel axe (`minecraft:stone_axe` & `minecraft:iron_axe`): wooden plank
	- blaze gold, diamond & netherite axe: wooden log (full block)
- Fences also drop wooden buttons if broken with hand, flint hatchet or copper axe. If a better axe is used they drop the item like normal.
- Iron pickaxes (`minecraft:stone_pickaxe`) cannot mine deepslate
- Breaking tall grass has a high chance of dropping (without needing to use shears)
- Clay drops 1 clay ball by default. Using shovels of higher tiers increases the amount dropped:
	- no shovel & Copper shovel (`minecraft:wooden_shovel`): 1 clay ball
	- Iron shovel (`minecraft:stone_shovel`): 1-2 clay ball
	- Steel shovel (`minecraft:iron_shovel`): 1-3 clay ball
	- Blaze Gold Shovel (`minecraft:golden_shovel`): 2-4 clay ball 
	- Diamond, Netherite shovel: 4 clay ball

---

## Miscellaneous
- Players HP scales with their experience (view [Health Scaling](./health_scaling.md) for more)
- Hard mode is always turned on automatically on datapack reload
- Villages removed
- Untamed wolves agro the player at night
- Cow, Donkeys and Horses kick the player when hurt by them
- Every full moon is a [Red Moon](./miscellaneous/red_moon.md) (More info in [Mobs](./mobs.md) tab)
- Stews are now stackable!
- (Unfertilized) farmland has a random chance of reversing the growth stage of a crop placed upon it. In addition there is a random chance for a weed to grow, which has a random chance to replace the farmland with a grass block. In combination they make it impossible to grow crops on soil that has not been fertilized.
- Drinking from (unfiltered) water bottles and (unpasturized) bucket of milk has a high chance of applying negative effects like hunger and poison.
- Every full moon is a [Red Moon](./miscellaneous/red_moon.md).
- [Netherite](./material_tiers/netherite_tier.md) armor has increased armor toughness
