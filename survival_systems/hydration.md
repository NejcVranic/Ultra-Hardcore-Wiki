# Hydration
Hydration is a [Survival System](../survival_systems.md) which adds a hydration bar. It's designed to serve as an obstacle in the early game and doesn't need to be maintained, after the player has progresses far enough to obtain a [Hydrating Helmet](../items/hydrating_helmet.md).

The color of the bar indicates the severity of dehydration. Being dehydrated causes adverse effects:
- <span style="background-color:rgb(0, 100, 250);color:rgb(0,0,0)">Blue</span> = No adverse effects
- <span style="background-color:rgb(250, 200, 30);color:rgb(0,0,0)">Yellow</span> = Slower movement speed
- <span style="background-color:rgb(250, 0, 0);color:rgb(0,0,0)">Red</span> = Weakness and even slower movement speed

The hydration bar is hidden when the player's hydration is maxed out. 

Internally, hydration is a score between 0 and 6000. The player can view this score through the hydration bar at the top of their screen. The player dies if their hydration falls to 0.

---

### Losing hydration
Hydration is passively lost at a rate of 1 every 2.5 seconds (with no intervention the bar depletes in (about) 3 full in-game days or 1 hour). 

Sprinting increases the loss of hydration, also by 1 every 2.5 seconds.

Hydration is lost extremely quickly when the player is standing in lava, is on fire or is in the nether, if the player is not wearing a Hydrating Helmet.

---

### Gaining hydration
Hydration can be increased by eating various food items or drinking from water bottles, milk, potions or a Canteen.

Drinking from regular water bottles recovers 1200 hydration, but has a high chance of applying negative effects like hunger or poison.

Drinking from a filtered water bottle recovers 2000 hydration (and has no chance of applying negative effects).

[Foods](../items/foods.md) that increase hydration:
- Apple
- Beetroot soup
- Cactus juice
- Mushroom stew
- Squids stew
- Glow squid stew
- Golden apple
- Melon slice
- Sweet berries
- Hot cocoa

A player will very slowly regain hydration if they stand underneath Dripstone, which is dripping water.

If the player is wearing a Hydrating helmet they will passive gain 3 hydration. In practice this is usually enough for net gain of hydration, without having to increase it by other means.

---

### Drinking polluted water
When a player drinks an unfiltered bottle of water or bucket of milk which has not been pasturized, they game will attempt to apply negative effects:
- 33% chance for Hunger 3 for 21 seconds
- 33% chance for Hunger 7 for 11 seconds
- 33% chance for Hunger 10 for 9 seconds
- 33% chance for Poison 1 for 5 seconds

Bottles of water and buckets of milk can be boiled on a [campfire](../blocks/campfire.md) to turn into [Filtered Water Bottle](../items/filtered_water_bottle.md) and [Pasturized Bucked of Milk](../items/pasturized_bucket_of_milk.md), which are safe to drink and will not apply negative effects.


