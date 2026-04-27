# Sanity
Sanity is a [Survival System](../survival_systems.md) which adds sanity stages.

The players sanity stage is announced to the player through the chat box when their sanity level changes. The sanity stage of a player is determined by a hidden score (between 0 and 120).

The hidden insanity score can be (temporarily) viewed by throwing a Corn Flower or Lapis Lazuli onto a lit campfire. The campfire will emit blue smoke and display the score for 3 seconds (if Corn Flower was used) or 10 seconds (if Lapis Lazuli was used).

Every condition that passively increases or decreases insanity is checked in a loop every half second, with a chance of 33%. (Every half second there is a 33% chance to check the conditions and increase/decrease the score.)

---

### Gaining insanity
The insanity score is increased every by:
- Getting hurt (`+2 insanity`)
- Losing experience levels (`+10 insanity`)
- (passively) standing in the dark for more than 5 seconds (Note: this isn't always reliable because there is no reliable way to detect light levels in Vanilla Minecraft.) (`+1 insanity`)
- (passively) being in proximity of Phantoms (`+1 insanity`)
- (passively) being below Y=0 (`+1 insanity`)
- (passively) being in End dimensions (`+1 insanity`)
- (passively) standing on withered soil (`+1 insanity`)

---

### Losing insanity
The insanity is decreased by:
- (passively) having the regeneration effect (`-1 insanity`)
- (passively) having the glowing effect (`-1 insanity`)
- (passively) being in proximity of 
	- Tamed Wolf (`-1 insanity for each`)
	- Horse (`-1 insanity for each`)
	- Tamed Cat (`-1 insanity for each`)
	- Axolotl (`-1 insanity for each`)
	- Snowman with the pumpkin removed (`-1 insanity for each`)
- (passively) having Totem of Undying in inventory (`-3 insanity`)
- (passively) having Bucket of Axolotl in inventory (`-1 insanity`)
- (passively) standing inside glow berries bushes (`-1 insanity`)
- Consuming foods:
	- Glow Berry (`-10 insanity`)
	- Glow Berry Pie (`-25 insantiy`)
	- Glazed ham (`-15 insanity`)
	- Honey (`-15 insanity`)
	- Golden carrot (`-10 insanity`)
	- Choccy Milk (`-10 insanity`)
	- Milk (`-5 insanity`)

---

### Sanity stages and punishments
Punishments are applied every half-second. The punishments have a cumulative effect. (If a player has a higher stage of insanity they also receive all punishment of lower stages.)

The sanity stage depends on the player's insanity score:

Calm (0 to 14)
- No effect

Uneasy (15 to 29)
- Hunger 1 effect

Scared (30 to 49)
- Hunger 2 effect
- 1% chance for Blindness 1 effect for 10 seconds

Terrified (50 to 74)
- 2% chance to teleport a short distance 
- Enderman will agro the player automatically
- about 6% chance to hear a sound (cave, creeper, elder guardianm, enderman stare or teleport)

Lost sanity (75+)
- blindness
- 10% chance to teleport player a short distance
- (80+) 4% chance to summon enderman behind or to the side of the player (if the blocks are empty)
- (100+) Wither 1 effect