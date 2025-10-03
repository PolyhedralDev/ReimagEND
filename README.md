![ReimagEND](https://github.com/user-attachments/assets/c407dcf6-ae98-4a7b-8db8-36b41d3ee7d3)

## A Terra pack designed to reimagine the End with new biomes, features, and terrain to explore.

Part of this pack uses resources from 
 - Astrash's Aeropelago pack, found [here](https://github.com/Astrashh/Aeropelago).
 - Our Overworld pack, found [here](https://github.com/PolyhedralDev/TerraOverworldConfig).

ReimagEnd is currently a **WORK IN PROGRESS**. 

Expect frequent changes, which may be incompatible (i.e, cause chunk borders) with older versions of the pack.

Vanilla End Cites generate with their loot tables unaffected while Terra's custom structures don't have custom 
loot tables as loot table support for Terra has not been implemented yet.

### KNOWN ISSUES
#### Ender Dragon Respawn
Respawning the ender dragon will cause the original vanilla end dragon spikes/pillars
alongside those from Terra. It is designed this way for the moment to at least have the initial
dragon fight involve end crystals and memorable with special dragon pillars.

#### End Gateways
End gateways are currently manually placed by Terra, which allow for two-way gateways to be created by players
since block NBT support for Terra has not been implemented yet.

## Installation
Download a ReimagEnd release from the [releases page](https://github.com/PolyhedralDev/ReimagEND/releases) for a reliable pack version 
or from a ReimagEnd branch for changes that haven't been applied to the latest release yet.

Follow this [installation guide](https://terra.polydev.org/install/index.html) for your particular platform.

Fabric users will have to edit the `level.dat` in order to apply custom generation to the end dimension.

#### Bukkit.yml Quick Reference 
##### Affects just the Vanilla End Dimension
```
worlds:
  world_the_end:
    generator: Terra:REIMAGEND
```
##### More than One Config Pack for Multiple Worlds 
```
worlds:
  world:
    generator: Terra:OVERWORLD
  world_the_end:
    generator: Terra:REIMAGEND
```

## Biome Distribution

### Aether Pockets
Scattered across the outer end, Aether pockets surrounded by void that
resemble that of the overworld in the form of floating isles.

Aether pockets can be disabled with the `toggle-aether-pockets` setting in the `customization.yml`.

There are several different biome distribution presets available to be switched
to in the `pack.yml`. Aether pockets will generate in some presets by default.

Furthermore, there are settings in the `customization.yml` to tweak 
biome distribution.

Anything specific may require configuring biome distribution files.

### Presets

The Rings of Life preset is ReimagEnd's default biome distribution.

#### Rings Of Life
Rings of life distributes the outer end in concentric rings with each individual 
ring containing more life and vegetation as you venture further from the dragon island.

#### Normal
Normal distributes the outer end in a more typical fashion.

#### Vanilla-Ish
Vanilla-Ish distributes the outer end to mostly resemble vanilla's outer end.

#### BetterEnd
BetterEnd distributes the outer end to mostly resemble Dfsek's BetterEnd plugin.

#### Aether World
Aether World distributes the entire world as an Aether.

#### Biome Removal or Rarity Customization
Biomes can be removed from distribution by going to their distribution file 
and commenting them out with a # in front of the line dash.

You can adjust the rarity of biomes by tweaking the weight numbers attached 
to each biome.

Outer end biome distribution can be configured in `biome-distribution/stages/outer_end_distribution.yml`.

Aether biome distribution can be configured in `biome-distribution/stages/outer_end_distribution.yml`.

### Dragon Island

The Dragon Island has various features to liven up the atmosphere.

#### Dragon Pit
The size of the Dragon Pit that generates in the center of the dragon island 
can be tweaked with the `dragon-pit-radius` setting in the `customization.yml`.