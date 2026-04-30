# Poor Farmland
Poor Farmland is a [block](../blocks.md), which can be used to plant crops, just like the Vanilla farmland block. In effect, crops grow slower on poor farmland compared to Vanilla farmland. It will grow weeds, which can be removed with [gardening shears](../items/gardening_shears.md).

<div style="display: flex; align-items: flex-start; gap: 24px;">  
<div style="flex: 1;">  
<p>Poor farmland looks mostly the same as Vanilla farmland, but has gray and green spots on its top texture.</p>
<p>Poor farmland is created when the player uses a hoe (without the fortune enchantment) to till the soil. If the hoe is enchanted with Fortune the chance of creating poor farmland, instead of Vanilla farmland, decreases with the Fortune level. At Fortune level 3 the hoe will always create Vanilla farmland.</p>
<p>When weeds are growing on the block, they appear as larger and larger oak leaves.</p>
<p>Every 2.5 seconds there is a 5% chance for poor farmland to run the following code:</p>
<p>There is a 1 in 30 chance the block reduces the growth stage of a crop growing on top of it, unless the crop has reached its final growth stage. There is also a 1 in 30 chance, for every adjacent farmland block with the same crop growing on it, for the growth stage to be reduced.</p>
<p> There is a 1 in 50 chance that a weed grows on the block. A block with a stage 3 weeds (fully grown weeds), has a 5% chance of turning the block into a grass block with a 20% chance for short grass growing on top. (This will destroy the farmland and any crops on the block.)</p>
</div>  
	
<div style="width: 250px; border: 2px solid #3a3a3a; font-family: sans-serif;">  
<!-- TITLE -->  
<div style="background-color: #3a3a3a; color: white; padding: 6px; font-weight: bold; text-align: center;">Poor Farmland</div>  

<!-- IMAGE -->  
<div style="text-align: center; padding: 10px;">  
<img src="images/poor_farmland.png" alt="poor_farmland" width="128" style="image-rendering: pixelated;">  
</div>  

<!-- BASIC INFO -->  
<div style="padding: 6px 8px; font-size: 14px;">  
<strong>Type:</strong> block<br>  
</div>  
		
<!-- DIVIDER & INFO -->  
<hr style="margin: 2px 0; border: 0; border-top: 1px solid #aaa;">  
<div style="padding: 4px 8px; font-size: 14px;">  
<strong>Obtainable as item:</strong> No<br>
</div>  
</div>  
</div>

### Behavior
Over time the weeds stage of a poor farmland block increases and the weeds seen on the block get bigger. Weeds have 4 stages, 0 to 3. During stage 0 no weeds can be seen growing. Each next stage the weeds grow larger. When weeds reach stage 3, there is a random chance they convert the block into a grass block, destroying the crops.

If bone meal is dropped on top of it, the outcome depends on if there are weeds growing on the block or not. If there are no weeds, the block will be converted into a Vanilla farmland block. However, if there are weeds growing, it will instead turn into a grass block.

If a weed is growing on the block, it can be removed with gardening shears.