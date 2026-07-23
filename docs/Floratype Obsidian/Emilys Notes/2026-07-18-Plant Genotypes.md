---
noteType: "[[00 Config/Note Templates/Folder Note Page Template|Folder Note]]"
created: 2026-07-18T23:56:35Z
user: "[[00 Config/00 Config|Emily Mohr]]"
parent:
  - "[[Floratype]]"
---
# Notes

## Table of traits

**Animal Crossing**

| Trait Name  | Number of bits | Number of Genes | Number of Outcomes | Outcomes                                                     | Trait Group |
| ----------- | -------------- | --------------- | ------------------ | ------------------------------------------------------------ | ----------- |
| Color       | 8              | 4               | 9                  | White, Yellow, Red, Orange, Pink, Purple, Green, Blue, Black | Apperance   |
| Flower Type | 3              | 1               | 8                  | Rose, Pansy, Cosmo, Hyacinth, Mum, Windflower, Lily, Tulip   | Apperance   |
| Growth      | 2              | 1               | 3                  | Bud, Growing/Picked, Grown                                   | Growth      |
| Total       | 13             | 6               | 9x8x3=216          | Up to 216, actually 54 ColorXFlower combos                   |             |
**Floratype**

| **Trait Name**                            | **Number of bits** | **Number of Genes** | **Number of Outcomes** | **Outcomes**                                               | **Trait Group** | **Notes**                                                                             |
| ----------------------------------------- | ------------------ | ------------------- | ---------------------- | ---------------------------------------------------------- | --------------- | ------------------------------------------------------------------------------------- |
| Flower Type                               | 4                  | 1                   | 16 (up to)             | Rose, Tulip, Daisy                                         | Appearance      |                                                                                       |
| Growth                                    | 2                  | 1                   | 4 (up to)              | Bud, Growing/Cut Back, Grown, Picked?                      | Appearance      |                                                                                       |
| **Subtotal**                              | 6                  | 2                   |                        |                                                            |                 |                                                                                       |
| Color                                     | 8                  | 4                   |                        |                                                            | Appearance      |                                                                                       |
| Double Flower                             | 2                  | 1                   | 2                      | Single, Double (recessive)                                 | Appearance      |                                                                                       |
| Petal Number                              | 2                  | 1                   | 2                      | n, n+1 (recessive)                                         | Appearance      | (could combine with Double Flower)                                                    |
| Albino                                    | 1 (or 2)           | 1                   | 2                      | Color, White, Faded palette?                               | Appearance      |                                                                                       |
| Leaf Shape                                | 1                  | 1                   | 2                      | pointed, smooth                                            | Appearance      |                                                                                       |
| Leaf Number                               | 1                  | 1                   | 2                      | n, n-1                                                     | Appearance      |                                                                                       |
| Growth Speed                              | 2                  | 1                   | 3                      | Slow, Med, Fast                                            | Plant Behavior  |                                                                                       |
| Take that Jack!                           | 1                  | 1                   | 2                      | V Fast when 111 w/ growth speed otherwise No Change        | Plant Behavior  |                                                                                       |
| Death Speed                               | 2                  | 1                   | 3                      | Slow, Med, Fast                                            | Plant Behavior  |                                                                                       |
| Deathless                                 | 1                  | 1                   | 2                      | Deathless when 000 w/Death speed otherwise No Change       | Plant Behavior  |                                                                                       |
| **Seasonality**                           | 4?                 | 2                   | 3 per season           | During season, dead, Slow Growth, Normal Growth            | Plant Behavior  | This implies each flower only has 1 season it grows in, **probably not what we want** |
| Pest Defense                              | 2                  | 1                   | 3                      | Prevents herbivory within 1-2 squares                      |                 |                                                                                       |
| Hearty Growth                             | 2                  | 1                   | 2                      | Grow over weeds and other plants                           |                 |                                                                                       |
| Weed Defense                              | 2                  | 1                   | 3                      | Weeds don't grow within 1-2 squares                        |                 |                                                                                       |
| Pollinator-Haver                          | 2                  | 1                   | 3                      | Provides polinators to plants within X (1-2?) squares      |                 |                                                                                       |
| Pollinator-Needer                         | 2                  | 1                   | 2                      | Flowers slower (or not at all) without a pollinator nearby |                 |                                                                                       |
| Can you smell what this plant is cooking? | 2                  | 1                   | 2                      | Plants within 2 squares breed at X increased rate          |                 |                                                                                       |
| Compatibility Group A                     | 1                  | 1                   | 2                      | Cannot grow within 2 squares of Compatibility Group B      |                 |                                                                                       |
| Compatibility Group B                     | 1                  | 1                   | 2                      | Cannot grow within 2 squares of Compatibility Group A      |                 |                                                                                       |
| Growth Format                             | 4?                 | 3                   | 5?                     | Vine, Bush, Tree, Stalk, Specimen                          |                 | Impacts regrowth rate and yield                                                       |
| Flower Yield                              | 2                  | 1                   | 3                      | n-1, n, n+1                                                |                 |                                                                                       |
| Seed Yield                                | 2                  | 1                   | 3                      | n-1, n, n+1                                                |                 |                                                                                       |
| Quality                                   | 2                  | 0                   | 4                      | None, Bronze, Silver, Gold                                 |                 | Non-heritable                                                                         |
| **Total**                                 |                    |                     |                        |                                                            |                 |                                                                                       |
## Storage Space
- From Chris
	- As I was thinking about the amount of storage space for the special orders (especially the text and portrait images), I determined that we can probably double the amount of space available for flower genes.
	- That makes the updated math: 64 bits total - 6 for flower type and age = 58 bits / 2 = 29 bits for one set of chromosomes. So that could be 29 genes with 2 alleles each, or fewer genes with some having more than 2 alleles (not sure that I'm using those genetics terms correctly, but hopefully you get the idea). Before doubling the space, we would have only room for 13 genes. Hopefully this is enough space for all of your genetics ideas.
## Animal Crossing Color
- ACNH's system can be thought of as trinary genes (0, 1, 2 per gene) 
	- This is how it's expressed in some of the breeding guides which can be confusing
		- But its 3 and 4 pairs of alleles where the order doesn't matter
	- because each gene is a _pair_ of alleles, each allele being one bit, and the combination of two bits gives three states: 00, 01, 11 (heterozygous is unordered, so 01 and 10 are the same). 
- bits for roses, 6  bits for others
- ![[2026-07-20-152255849-vR0aqlA.png|325]]
## Thinking about traits while at Dad's
- 32 total bits of genetic info
	- 5 occupied by other 
		- 3 for 8 flower types 
		- 2 for growth state 
	- 27 left 
- color
	- 3 bits (at least)
	- 8 colors 
		- red
		- white 
		- yellow 
		- pink
		- orange 
		- purple 
		- blue 
		- black 
		- green
		- gold 
	- at least 1 for albino 
	- true blue or blacks in flowers 
- could include albino in 3bit petal pattern 
	- depending on sprites possible 
- shape
	- double flower
		- probably not an option for all types 
		- petal number 
	- leaf number, shape and pattern 
- fast or slow growth 
		-  if you had something else like this you could do gradualism vs punctuated change 
			- I.e for every gene of three on increase by x vs when you have all three do x
- death/senesanse timing 
- growing season - weather/temp/drought/pest resistant 
	- scrambling to prep for a cold snap vs having flowers resistant from last year 
	- every thing is more expensive in winter 
		- buy stuff for more, but sell for more
- does the flower grow back after cutting? 
	- do more grow back? 
	- how fast do they regrow 
	- rose hips? 
		- post cut growth 
	- do they die every season? 
- when do these bloom? 
	- all at once, all in sync with others? 
- breeding /cloning pattern and group 
	- flowers are probably divided by group rather than type genetically even if colloquially we call them different flowers, here we just care if they can crossbreed 
	- it's like kinda interesting to discover new named flowers down the breeding chart 
- brainstorm
	- the great omelet 
		- daily wildflowers for harvest only? V
	- quince filler stems
		- use the flower and the stem, different regrowth/death
	- dried flowers 
		- saving and using later in the wintwr
		- wtf how do we do winter 
	- seed type 
	- fruit 
	- scent 
		- breeding rate? 
	- size, micro flower vs macro 
		- some of that may be doubles 
	- defense 
		- stops other groups (or pests) from growing near 
	- growth format 
		- stalk, bush, tree, vine, graft(?) 
			- trelese vines 
		- specimen flowers
			- single long stem rose 
			- reduced yield, more trimming, higher cost 
		- can you write restrictions like this flower will die if it's not like adjacent to a certain number of the same flower or different flower or empty spaces 
	- mutation rate
	- attracts pollinators 
		- near pollinators 
		- maybe don't sell well
		- reminds me of Evolution gams
	- defense against predators 
		- sacrificial 
	- annual vs perennial (what's it's death like)
		- annuals are mostly not for cut bouquets 
			- marigolds
				- because they won't come back after cut 
			- day lillies 
				- only good for a day
				- if you cut it, then it won't keep blooming
				- but would keep producing flowers from the same stalk 
				- hibiscus tree
	- yield 
		- flower or seed 
		- time to new flower 
	- finicky flowers
		- like orchids 
		- many variations, very specific conditions for cultivation 
	- no expectation of the phenotype to be continuous 
		- a category that is not so much about the flower as it is how people value it 
			- new members of different lineage arrive in the middle of other lineage 
			- floral design category could be one 
			- ![[2026-07-19-011150581-Pasted image 20260719011148.jpg]]
	- selection to new flowers 
		- maybe can't move along the path until in base stats
		- where does the variation come from?? 
		- we can recombine but what's new? 
		- ![[2026-07-19-004302660-Pasted image 20260719004300.jpg]]
	- fun genetics 
		- linked traits
		- epistasis 
		- pleiotropy 
	- novel ways to navigate the diversity space 
		- way of the white leaf
		- hgt
		- insertions, deletions
			- frame shift?? 
				- corn ykd allow targeted mutation but within a certain set of genes always causes a mutation in downstream genes 
		- 
- we need a weed. 
	- no value, no variation, only clone and take up space 
	- weed spray 
	- resistant plants (full farm spray)
		- resistant weeds
	- plants can grow over weeds 
	- weeds can't grow near plants 
# Tasks
