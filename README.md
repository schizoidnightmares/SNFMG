# Schizoid Nightmares' Fantasy Map Generator
This is a fork of Azgaar's Fantasy Map Generator, with the primary addition being a revamped biome system. Maps saved with Azgaar's version should be able to be loaded in this fork (from 0.7–1.66). However, keep in mind that the two versions are not cross compatible. When saving a map using this fork, consider saving it under a different file name. It is also recommended you regenerate biomes if importing a map from Azgaar's.

## Differences between the fork and upstream
* Revamped biome system: 92 new biomes (including montane variants)
* Rivers generate more generously and more uniform in width
* Designed with 100k maps in mind
* Mountain relief icons generate more conservatively, hills are representated by smaller mountains
* Two new styles: Terra & Plain (both are intended to be used)
* One new template: Terra
* Dry lakes are now referred to as hypersaline lakes
* Lava lakes and sinkholes appear less rarely
* New lake type: hot lake
* Taklamakan template is not available

### Files that deviate from upstream
(this list is currently a WIP)
* modules/ui/options.js
* modules/ui/style.js
* modules/heightmap-templates.js
* modules/load.js
* modules/relief-icons.js
* modules/river-generator.js
* .gitignore
* index.html
* main.js
* README.md

## Known bugs
### Relief icons generate excessively
I'll be fixing this hopefully soon.

## Features possibly misinterpreted as bugs
### Biome colouring
The biomes are coloured in a "naturalistic" fashion, meant to blend into each other or simulate the appearance of eco-tones (transitory biomes). Compared to upstream, it is harder to tell the difference between the biomes. This reflects reality, where the average colours of biomes can appear very similar.

### Biome article links
As there are 92 total biomes (not including the 'marine' biome), it is not feasible to include an article to every single one. If a Wikipedia article exists with the exact same name of the biome, it will be automatically redirected to it. Otherwise, the article will not be found.

## Helpful tips
### How to regenerate biomes
1. Click on Tools
2. Click on Biomes under *Click to configure*
3. Click on *Restore the defaults* (the button to the left of the tree icon near the bottom of the Biomes Editor)

## Other information
### What are wastelands?
Wastelands are land biomes that are warmer than 35 degrees Celsius (95 degrees Fahrenheit). They are intended for worlds with inhospitable temperatures at the equator. No plants can grow in wastelands, no matter how much rainfall they receive; wastelands cannot support a human population.

### What are hot lakes?
Hot lakes are the lake equivalent of wastelands. They are effectively "dead lakes." Compared to hypersaline lakes, they have a more intense green appearance.

### What is the difference between a rainforest and a jungle?
A rainforest is a biome that receives a lot of rainfall (self-explanatory) but has less dense vegetation than a jungle. Often in the real world, a jungle will be on the border of a rainforest and a river (or water body), giving the appearance of extremely thick vegetation within. Once the jungle barrier between the river and the rainforest is crossed however, the vegetation is much more passable.
