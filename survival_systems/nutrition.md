# Nutrition
Nutrition is a [Survival System](../survival_systems.md) which tracks the quality of a player's diet and its impact on their health.

This system encourages the player to eat a varied diet of foods and can cause negative or positive effects.

A player’s diet quality is determined by three hidden nutrition scores: **Protein**, **Carbs**, and **Micronutrients**, each ranging from 0 to 200. Upon first spawning (and on respawn) all nutrition scores are set to 100. The scores are changed by eating any [food item](../items/foods.md).

Players can view their current nutrition scores by using a [nutrition monitor](../items/nutrition_monitor.md).

Consuming food alters all three diet scores, with a few exceptions. 
A food item will always change Protein and Carbs scores the same way when it is eaten. The scores are increased (or decreased) by the value of the food's protein and carb values (some foods are "balanced" and are an exception to this rule).
> Example: cooked beef (steak) values are 16 for Protein and -16 for carbs. Eating it will always increase the player's Protein by 16 and decrease their Carbs by 16. 

Each food item has a unique impact based on the hunger points it restores, its internal diet values, nutrition class and how frequently it is consumed. (The exact calculation is documented below.)

In general, a food’s impact on nutrition scales with the hunger points it restores. (Foods that restore more hunger have a greater effect on diet scores, while foods that restore less have a smaller effect.)

When eating food, a short message may appear above the hotbar:
- "<span style="color:rgb(130, 220, 120)">Yum!</span>" - the food is relatively new to the player's diet (low diet frequency score)
- "<span style="color:rgb(250, 0, 0)">Bleh...</span>" - the food is consumed frequently (high diet frequency score)
Foods eaten less often (indicated by the green message) always increase the micronutrients score, while foods eaten frequently (indicated by the red message) always decrease it.

---

### Diet Effects
The player is encouraged to keep their protein and micronutrient scores high and their carbs score balanced. 
Depending on the player's diet scores, the following effects may be applied:

Wither 1:
- when Protein is 0
- when Micronutrients are 0
- when Carbs are 200 or more

Nausea 1:
- random chance when sprinting, if Carbs are below 30

Speed 1 & Strength 1:
- when Protein and Micronutrients are above 170 and Carbs are between 30 and 170

---

### Balanced Foods
Balanced foods have no impact on Protein and Carb scores, unless the player's score is very high or very low:
- If Protein is low (30 or less) the score is increased by the hunger points the food restores
- If Carbs are low (30 or less) the score is increased by the hunger points the food restores
- If Carbs are high (70 or more) the score is reduced by the hunger points the food restores

> Balanced foods can be used to easily maintain Protein and Carb scores. This is useful to the player for maintaining the speed effect resulting from a healthy diet. 

Balanced food's impact on the micronutrients score is calculated the same way as for all other foods. All balanced foods belong to the NUTRITIOUS nutrition class, except for Glazed ham and Meat pie which are in the POOR class.

Below is a list of balanced foods:
- Apple Pie
- Pumpkin Pie
- Sweet Berry Pie
- Glow Berry Pie
- Goulash
- Rabbit stew
- Glazed ham
- Meat pie

---

### How micronutrient score is calculated
How the score changes after consuming a food depends on the hunger points the food restores, how frequently it is eaten and it's nutrition class.

Each food has its own diet score that keeps track of how often the food is eaten. (Some foods share their diet scores.)
> Example: Squid tentacle, Glow squid tentacle, Squid stew and Glow squid stew all share the same `UH_diet_squid` frequency score.

A food's nutrition class is either NUTRITIOUS, AVERAGE or POOR.

The table below shows how the micronutrient score is changed when a food is consumed (where `H` is hunger points the food restores):

| Diet frequency score / Nutrient class | NUTRITIOUS  | AVERAGE     | POOR        |
| ------------------------------------- | ----------- | ----------- | ----------- |
| 0 - 19 (eaten rarely)                 | `+ (2 x H)` | `+ H`       | `+ 2`       |
| 20 - 69                               | `+ H`       | `- H`       | `- H`       |
| 70 - 100 (eaten often)                | `- H`       | `- (2 x H)` | `- (2 x H)` |

---

### How diet frequency score are calculated
Whether a food is eaten rarely or often depends on it's diet frequency score.

When a player (re)spawns all their food's frequency scores are set to 0. 
The food frequency scores are are always between 0 and 100.

Each time a food is eaten it's score is increased by `5 x H` (where `H` is hunger points the food restores) and every food's score is decreased by `H`.
> (The food's frequency score is increased by `4 x H` and all other food's score are lowered by the `H`)
> Example: 
> 	If all frequency scores are 0 and the player eats 1 steak, their `UH_diet_beef` score will increase from 0 to 32 (`0 + 4 x 8`). Steak is now no longer rarely eaten (and doesn't display the green title).
> 	If the player then eats 2 bread their `UH_diet_bread` score will increase from 0 to 40 (`0 + 2 x (4 x 5)`) and their `UH_diet_beef` score will decrease from 32 to 22 (`32 - 2 x 5`). Bread is now no longer rarely eaten.
> 	If the player then eats 1 bread their `UH_diet_bread` score will increase from 40 to 60 (`40 + 4 x 5`) and their `UH_diet_beef` score will decrease from 22 to 17 (`22 - 5`). Steak is now rarely eaten (and will again show the green title the next time it is eaten).

