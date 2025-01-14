# Included Custom Datapack Overview

Custom datapacks were made to modify the given experience in the modpack, mostly in order provide sustainable resource farming methods, but also for convenience, balance, and to help mitigate server lag.

This overview, outlines each datapack and what it either adds or changes. If you don't like what they do, you can simply remove it from your datapacks folder in Paxi under configs for singleplayer, or, not include them in the datapacks folder in your server world save folder. To further facilitate this, an attempt has been made to separate the various changes into multiple datapacks for easier cherry-picking.

<div align="center">

# Datapacks - Tweaks
</div>

<div align="center">

## <center>dragons beacon bases</center>
</div>

Adds over 100+ modded blocks as valid for use as beacon base blocks. The blocks are all variants of the vanilla equivalents, so iron_block, gold_block, diamond_block, emerald_block and netherite_block. This allows for more creative designs when building beacons. If you encounter blocks that are not included in this datapack, but you think they should, please report it as an issue.

<div align="center">

## <center>dragons create mechanical extruder</center>
</div>

The mechanical extruder is very useful for servers that want to reduce the server-strain induced by the Create mod, as you can easily add or adjust recipes using datapacks like this one. A few recipes were altered to be more generous, and some new ones were added for end-game resource farms for large builds. This should also reduce the need to destroy the underground of the overworld in the persuit of resources.

### *Recipes - Modified original*
- basalt
- cobblestone
- limestone
- scoria
- stone
Yields were increased from 1 into 4, reducing the amount of extruders needed.

### *Recipes - Dragon Claw Persistent*
- asurine
- crimsite
- ochrum
- veridium
Useful for crushing recipes into getting the various primary metals. Requires a full metal block of the matching ore, as well as a netherite block. It takes 64 bonks to make a stack of 64.

<div align="center">

## <center>dragons create oxidized</center>
</div>

Adds various Create-specific recipes related to turning copper into the various levels of oxidized versions by the use of water. Very convenient if you plan to do larger builds.

<div align="center">

## <center>dragons create stripping</center>
</div>

Adds compatibility recipes for stripping of various modded logs for the mechanical saw. Useful if you need a lot of stripped logs for bigger builds, or just want to use other logs in your automation setup for making casing and such.

<div align="center">

## <center>dragons create tweaks</center>
</div>

These tweaks are all about useful or convenient recipe additions for Create, that allow you to acquire various vanilla items or blocks through alternate means. This is mainly to extend your options for automation, but also to provide sustainable methods to acquire these for larger builds in a long-running server. 

### *Recipes - General*
- dcc_cobblestone_generator_mixing
<br /> Mix 500mb lava and 500mb water to make 32 cobblestone

- dcc_basalt_crushing
<br /> Crush basalt to get tuff in a 1:1 ratio

- dcc_coarse_dirt_mixing
<br /> Mix 16 gravel and 16 dirt to make 32 coarse dirt

- dcc_snow_washing
<br /> Wash 1 snow block to create 1 ice block

### *Recipes - Extended Washing for Metals*
- dcc_dirt_washing
<br /> Wash dirt for a 12% chance to get 4 copper nuggets

- dcc_clay_washing
<br /> Wash clay for a 12% chance to get 4 zinc nuggets

- dcc_flint_block_washing
<br /> (supplementaries) Wash 1 flint block for a 12% chance to get 1 iron nugget

- dcc_emerald_crushing
<br /> Crush 1 emerald to get 1 experience nugget

### *Recipes - Sustainable Filling*
- dcc_emerald_filling
<br /> Fill 500mb potion of healing onto 1 coal to create 1 emerald

- dcc_diamond_filling
<br /> Fill 500mb potion of regeneration onto 1 emerald to create 1 diamond

- dcc_lapis_filling
<br /> Fill 25mb potion of water breating onto 1 cinder flour to create 1 lapis lazuli

- dcc_nautilus_shell_filling
<br /> Fill 250mb potion of turtle master onto 1 prismarine crystals to create 1 nautilus shell

- dcc_heart_of_the_sea_filling
<br /> Fill 1000mb potion of turtle master onto 1 nether star to create 1 heart of the sea

### *Recipes - BetterEnd and BetterNether*
- dcc_end_stone_crushing
<br /> (betterend) Crush 1 end stone to create 1 endstone dust

- dcc_endstone_dust_washing
<br /> (betterend) Wash 1 endstone dust for a 12% chance to get 1 thallasium nugget

- dcc_soul_soil_washing
<br /> (betternether) Wash 1 soul soil for a 12% chance to get 1 cincinnasite

### *Recipes - Plants*
- dcc_big_dripleaf_mixing
<br /> Mix 1 big dripleaf with 250mb water to make 2 big dripleaf

- dcc_lily_pad_mixing
<br /> Mix 1 lily pad with 250mb water to make 2 lily pads

- dcc_small_dripleaf_mixing
<br /> Mix 1 small dripleaf with 250mb water to make 2 small dripleaf

### *Recipes - Bone Blocks and Coral*
- dcc_bone_block_crushing
<br /> Crush bone blocks for a 20% chance to get one of the coral blocks

- dcc_brain_coral_block_crushing
<br /> Crush brain coral block for a 50% chance to get either of the coral and/or coral fan "block"

- dcc_bubble_coral_block_crushing
<br /> Crush bubble coral block for a 50% chance to get either of the coral and/or coral fan "block"

- dcc_fire_coral_block_crushing
<br /> Crush fire coral block for a 50% chance to get either of the coral and/or coral fan "block"

- dcc_horn_coral_block_crushing
<br /> Crush horn coral block for a 50% chance to get either of the coral and/or coral fan "block"

- dcc_tube_coral_block_crushing
<br /> Crush tube coral block for a 50% chance to get either of the coral and/or coral fan "block"

<div align="center">

## <center>dragons curios tweaks</center>
</div>

Adds a dedicated slot for a backpack and enderpack respectively, so you can wear a backpack and an elytra at the same time. The shortcut key for opening your backpack, prioritizes the one that is equipped. This was done to create better compatibility between the elytra being equipable with curios, across the various modded elytra that are added by mods.

<div align="center">

## <center>dragons heracles book</center>
</div>

Adds a custom recipe, so you can actually craft the quest book in case you lose it, and don't want to use a hotkey.

### *Recipes*
- dcc_heracles_quest_book (1 book and 3 paper in a specific pattern)

<div align="center">

## <center>dragons infinicore tweaks</center>
</div>

Being able to make items have infinite durability is quite powerful, so the recipe was altered to be more complex. Refer to the recipe ingame, or in the json file for what you need to make it.

### *Recipes*
- infinicore

<div align="center">

## <center>dragons packedup tweaks</center>
</div>

The packedup backpacks were configured to have different capacities in order to increase the challenge. The smallest backpack can be made in the usual way, but the recipes to upgrade it into a copper or iron-tier, has been altered to require a shulkerbox instead. This was done to retain the significance of exploring the End after defeating the dragon, and to require players to optain access to "nested" storage, which shulkerboxes are in vanilla. This means that you still have to overcome the same challenges as in vanilla, but that the reward for doing so, is also to be able to make much larger inventory expansions.

### *Recipes*
- copper_from_basic
- iron_from_basic

<div align="center">

## <center>dragons vanilla tweaks</center>
</div>

This adjusts and adds a few crafting recipes that are entirely based in vanilla. These can also be used alongside Create in automation setups.

### *Recipes - Sustainable Block Crafting*
- dcc_deepslate_crafting
3x3 crafting of 1 black dye and 8 cobblestone, to create 8 cobbled deepslate

- dcc_end_stone_crafting
3x3 crafting of 1 ender pearl and 8 cobblestone, to create 8 end stone

- dcc_guilded_blackstone_crafting
3x3 crafting of 1 gold nugget and 8 blackstone, to create 8 gilded blackstone

- dcc_netherrack_crafting
3x3 crafting of 1 nether wart and 8 cobblestone, to create 8 netherrack

- dcc_quartz_block_smelting
Smelt 1 quartz block into 1 calcite block

- dcc_spawner_crafting
3x3 crafting of 1 nether star, 4 netherite scrap and 4 obsidian, to create 1 empty spawner

### *Recipes - Various*
- dye_"colorname"_wool
All 16 colors of wool dying recipes have been altered to dye 8 wool per dye instead of 1

### *Loot Tables*
- budding_amethyst
Using the matching tool with silk touch will drop the block instead of destroying it

<div align="center">

# Datapacks - Disablers
</div>

<div align="center">

## <center>dragons bbb disabler</center>
</div>

Building But Better adds "layer" blocks for some vanilla block-types. Their crafting recipes have been disabled due to personal preference, and to potentially reduce client and server lag due to "over-detailing" of builds. If you want to still use "layer" blocks, consider enabling the Copycats+ layer blocks instead, as they can take on the visual appearance of any solid block. For reference, this is also why bbb was disabled in the Every Compat (Wood Good) config.

Since this concerns a little over 100 individual recipes, the exact list is not provided here.

<div align="center">

## <center>dragons copycat disabler</center>
</div>

Copycats+ did not properly remove the stonecutting recipes, even if the mod config had certain blocks disabled. This datapack solution was made to address this, and reflect the changes made in said config, by removing the stonecutting crafting recipes of the disabled blocks. This is done to avoid overcomplicating builds and contraptions.

### *Recipes*
- copycat_block
- copycat_board
- copycat_byte
- copycat_half_layer
- copycat_half_panel
- copycat_layer
- copycat_slice
- copycat_slope_layer
- copycat_vertical_slice

<div align="center">

## <center>dragons immersive aircraft disabler</center>
</div>

Immersive Aircraft normally adds some destructive and combat-oriented additions to the airships. These have been disabled, as they can be rather destructive to the game world, not to mention other players and their builds.

### *Recipes*
- bomb_bay
- heavy_crossbow
- rotary_cannon

<div align="center">

## <center>dragons macaw disabler</center>
</div>

Macaw's Lights and Lamps also adds a couple slabs for vanilla blocks, which also emit light. These have been disabled, as you should instead use Copycats+ to achieve the same result. The copycats also work on contraptions, so prioritizing those is favorable. To do this, the crafting recipes have just been removed.

### *Recipes*
- glowstone_slab
- redstone_lamp_slab
- sea_lantern_slab
- shroomlight_slab

<div align="center">

## <center>dragons small ships disabler</center>
</div>

The Small Ships mod adds a destructive cannon that has been disabled. This was done by simply remocing the craft recipes.

### *Recipes*
- cannon
- cannon_ball

<div align="center">

## <center>dragons tom disabler</center>
</div>

Tom's Simple Storage Mod adds a lot of useful utility blocks to manage large storage inventories in one place, but some features were disabled to promote the use of Create more. This was done by removing the crafting recipes.

### *Recipes*
- inventory_cable_connector_filtered
- inventory_hopper_basic
- item_filter
- poly_item_filter
- tag_item_filter





